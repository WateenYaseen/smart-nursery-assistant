# Smart Nursery Assistant — Data Model

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Status:** Conceptual data model

This document describes the main information the application needs to store and how the information is related. It does not define database tables, SQL, ORM models, or migrations.

## 1. Plant

Represents one individual plant registered by the owner.

**Fields:**
- Plant ID — unique identifier for the individual plant.
- Common Name — recognized or owner-provided common name, when available.
- Registration Date — date the plant was added.
- Current Status — current recorded status of the plant, when available.

**Relationships:**
- One plant can have many inspections.
- One plant can have many care actions.
- One plant can have many recommendations.

Each individual plant must have its own record, even if several plants have the same common name.

## 2. Inspection

Represents one inspection performed for an individual plant.

**Fields:**
- Inspection ID — unique identifier for the inspection.
- Plant ID — identifies the plant being inspected.
- Inspection Date — date of the inspection.
- Image Reference — reference to the submitted image or images.
- Predicted Plant Name — predicted common name, when available.
- Identification Confidence — confidence information for the plant prediction, when available.
- Possible Conditions — supported possible diseases or visible problems.
- Supporting Symptoms — visible signs associated with the assessment.
- Water-Need Estimate — qualitative estimate, when supported.
- Assessment Notes — uncertainty, limitations, or additional information.

**Relationships:**
- Each inspection belongs to one plant.
- An inspection may be associated with recommendations.

## 3. Care Action

Represents an action the owner confirms they performed on a plant.

**Fields:**
- Action ID — unique identifier for the action.
- Plant ID — identifies the plant receiving care.
- Action Type — watering, treatment, or other care.
- Action Date — date the action was performed.
- Action Details — additional information entered by the owner.

**Relationships:**
- Each care action belongs to one plant.

Only actions explicitly entered or confirmed by the owner are stored as performed actions. Suggested actions are not automatically added to this record.

## 4. Recommendation

Represents an action suggested by the system for an individual plant.

**Fields:**
- Recommendation ID — unique identifier for the recommendation.
- Plant ID — identifies the related plant.
- Related Inspection ID — inspection that led to the recommendation, when applicable.
- Suggested Action — recommended next step.
- Reason — explanation for the recommendation.
- Priority — relative attention priority.
- Status — pending, completed, or dismissed, according to owner confirmation.

**Relationships:**
- Each recommendation belongs to one plant.
- A recommendation may be linked to one inspection.

A recommendation must not be marked as completed merely because it was displayed. Completion requires owner confirmation.

## 5. Plant Care Knowledge

Represents reference information used to provide plant-care guidance.

**Fields:**
- Plant Type — plant type or common name the information relates to.
- Watering Guidance — general watering method and guidance.
- General Care — relevant care information.
- Common Conditions — supported common diseases or problems.
- Symptoms — associated visible symptoms.
- Treatment Guidance — available treatment information.
- Information Source — source of the reference information.

**Relationships:**
- Plant-care knowledge can be used when generating information and recommendations for inspections.

## 6. Relationship Summary

- Plant → Inspections: one-to-many.
- Plant → Care Actions: one-to-many.
- Plant → Recommendations: one-to-many.
- Inspection → Recommendations: one-to-many or none.
- Plant Care Knowledge → Plant Assessment: reference information used when relevant.

**Important:** This is a conceptual model. The final database technology and detailed implementation structure have not yet been selected.