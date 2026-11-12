# Smart Nursery Assistant — Data Model

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Status:** Conceptual Data Model  
**Last Updated:** 2026-11-12  
**Update:** After Task 04 — Design and Backlog Preparation

This document describes the main information the Smart Nursery Assistant needs to store and how the information is related.

It defines the conceptual data structure only. It does not define database tables, SQL statements, ORM models, or migrations. The final implementation structure will depend on the selected database and technology.

## 1. Plant

Represents one individual plant registered by the owner.

**Fields:**

- **Plant ID:** Unique identifier for the individual plant.
- **Common Name:** Recognized or owner-provided common name, when available.
- **Plant Type:** Plant category or type, when available.
- **Registration Date:** Date the plant was added.
- **Location:** Optional description of where the plant is placed in the nursery.
- **Notes:** Additional information entered by the owner.
- **Current Status:** Current recorded status of the plant, when available.

**Relationships:**

- One plant can have many inspections.
- One plant can have many care actions.
- One plant can have many recommendations.
- One plant can have one or more related assistant conversations.

Each individual plant must have its own record, even if several plants have the same common name.

The owner selects an existing plant or creates a new record before starting an inspection. The system does not automatically match uploaded images to individual plant records in the first version.

## 2. Inspection

Represents one image-based inspection performed for an individual plant.

**Fields:**

- **Inspection ID:** Unique identifier for the inspection.
- **Plant ID:** Identifies the plant being inspected.
- **Inspection Date:** Date and time of the inspection.
- **Image References:** References to the submitted image or images.
- **Predicted Plant Name:** Predicted common name, when available.
- **Identification Confidence:** Confidence information for plant identification, when available and supported by the model.
- **Possible Conditions:** Supported possible diseases or visible problems.
- **Supporting Symptoms:** Visible signs associated with the assessment.
- **Water-Need Estimate:** Qualitative watering guidance, when supported by available information.
- **Care Guidance:** Relevant care instructions provided for the plant.
- **Assessment Notes:** Uncertainty, limitations, or additional information.
- **Inspection Status:** Current processing or result status, such as pending, completed, or failed.

**Relationships:**

- Each inspection belongs to one plant.
- One plant can have many inspections.
- An inspection may have multiple associated recommendations.
- An inspection may be referenced in an assistant conversation.

An inspection result represents an AI-assisted assessment, not a guaranteed diagnosis. The system should communicate uncertainty when the available image or information is insufficient.

## 3. Care Action

Represents a care action the owner confirms was actually performed on an individual plant.

**Fields:**

- **Action ID:** Unique identifier for the care action.
- **Plant ID:** Identifies the plant receiving care.
- **Action Type:** Type of care, such as watering, treatment, cleaning, or other care.
- **Action Date:** Date and time the action was performed.
- **Action Details:** Additional information entered by the owner.
- **Related Recommendation ID:** Optional reference to the recommendation that led to the action.

**Relationships:**

- Each care action belongs to one plant.
- A care action may be associated with one recommendation.

Only actions explicitly entered or confirmed by the owner are stored as performed actions. Displaying a recommendation does not automatically create a care-action record.

## 4. Recommendation

Represents an action suggested by the system for an individual plant.

**Fields:**

- **Recommendation ID:** Unique identifier for the recommendation.
- **Plant ID:** Identifies the related plant.
- **Related Inspection ID:** Inspection that led to the recommendation, when applicable.
- **Suggested Action:** Recommended next step.
- **Reason:** Explanation for the recommendation.
- **Priority:** Relative attention priority, when available.
- **Creation Date:** Date the recommendation was generated.
- **Status:** Current status, such as pending, completed, or dismissed, according to owner confirmation.

**Relationships:**

- Each recommendation belongs to one plant.
- A recommendation may be linked to one inspection.
- A recommendation may be linked to a care action when the owner confirms that the suggested action was performed.

A recommendation must not be marked as completed merely because it was displayed. Completion requires owner confirmation.

## 5. Plant Care Knowledge

Represents reference information used to provide plant-care guidance and support the assistant.

**Fields:**

- **Knowledge ID:** Unique identifier for the knowledge entry.
- **Plant Type:** Plant type or common name the information relates to.
- **Watering Guidance:** General watering method and guidance.
- **General Care:** Relevant care information.
- **Common Conditions:** Supported common diseases or problems.
- **Symptoms:** Associated visible symptoms.
- **Treatment Guidance:** Available treatment information.
- **Information Source:** Source of the reference information.
- **Language:** Language of the information, when available.

**Relationships:**

- Plant-care knowledge can be used when generating inspection explanations and recommendations.
- Plant-care knowledge can be used by the conversational assistant when answering plant-related questions.

Reference information should be based on suitable sources. The system should not present unsupported treatment advice as confirmed fact.

## 6. Assistant Conversation

Represents a conversation between the owner and the AI plant-care assistant.

**Fields:**

- **Conversation ID:** Unique identifier for the conversation.
- **Plant ID:** Optional reference to the individual plant related to the conversation.
- **Creation Date:** Date and time the conversation started.
- **Last Updated:** Date and time of the most recent conversation activity.
- **Conversation Title:** Optional short title or description.
- **Conversation Status:** Current status, such as active or archived.

**Relationships:**

- A conversation may be associated with one plant.
- One plant can have many related conversations.
- One conversation contains many messages.

The owner should be able to return to previous conversations when conversation history is available.

A conversation without a selected plant may still be used for general nursery or plant-care questions.

## 7. Assistant Message

Represents one message exchanged within an assistant conversation.

**Fields:**

- **Message ID:** Unique identifier for the message.
- **Conversation ID:** Identifies the conversation containing the message.
- **Sender:** Indicates whether the message was written by the owner or generated by the assistant.
- **Message Content:** Text content of the message.
- **Message Date:** Date and time the message was created.
- **Related Inspection ID:** Optional reference to an inspection discussed in the message.
- **Related Image Reference:** Optional reference to an image submitted during the conversation.

**Relationships:**

- Each message belongs to one conversation.
- A conversation can contain many messages.
- A message may reference an inspection or image when relevant.

Messages should remain associated with their original conversation so the assistant can use available context when continuing the discussion.

## 8. Image Reference

Represents a stored image associated with a plant inspection or assistant conversation.

**Fields:**

- **Image ID:** Unique identifier for the image.
- **Plant ID:** Related plant, when applicable.
- **Inspection ID:** Related inspection, when applicable.
- **Conversation ID:** Related conversation, when applicable.
- **Image Location:** Reference or path to the stored image.
- **Upload Date:** Date and time the image was uploaded.
- **Image Type:** Purpose of the image, such as inspection image or conversation attachment.

**Relationships:**

- An image may be associated with one plant.
- An image may be associated with an inspection.
- An image may be associated with a conversation.

The actual image file may be stored separately from the main application data. The database will retain the reference needed to retrieve it.

## 9. Relationship Summary

- **Plant → Inspections:** One-to-many.
- **Plant → Care Actions:** One-to-many.
- **Plant → Recommendations:** One-to-many.
- **Plant → Assistant Conversations:** One-to-many or none.
- **Inspection → Recommendations:** One-to-many or none.
- **Recommendation → Care Action:** One-to-zero-or-one, when the owner confirms a related action.
- **Conversation → Assistant Messages:** One-to-many.
- **Plant Care Knowledge → Inspection Assessment:** Reference information used when relevant.
- **Plant Care Knowledge → Assistant Responses:** Reference information used when relevant.
- **Inspection → Images:** One-to-many or none.
- **Conversation → Images:** One-to-many or none.

## 10. Data Handling Rules

The following rules describe how the application should handle its information:

1. Each individual plant must have a separate record.
2. Every inspection must be associated with the plant selected by the owner.
3. Previous inspection results and related images should remain associated with the relevant plant.
4. Care actions must only be stored as performed after owner confirmation.
5. Recommendations must remain separate from completed care actions.
6. Assistant messages must belong to their original conversation.
7. Conversations should use plant-specific context when a plant is selected and relevant.
8. Optional information may remain empty when it is not available.
9. Uncertain AI results must not be stored or displayed as guaranteed diagnoses.
10. Image references must point to the corresponding stored files.

## 11. Scope and Implementation Notes

This is a conceptual data model for the first version of Smart Nursery Assistant.

The model supports the planned application screens:

- **Home Dashboard:** Uses plant records, current status, and pending recommendations.
- **My Plants:** Uses registered plant records.
- **Add Plant:** Creates a new individual plant record.
- **Plant Details:** Uses plant information, inspection history, recommendations, and care actions.
- **Plant Inspection / Results:** Uses inspection records, image references, assessment results, and recommendations.
- **AI Assistant Chat:** Uses conversations, messages, plant context, inspection history, and plant-care knowledge.

The model does not require IoT sensor records, automatic irrigation data, employee management, inventory, sales, or accounting features in the first version.

The final database technology, image-storage method, and detailed implementation structure have not yet been selected. These will be finalized during development.