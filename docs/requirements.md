# Smart Nursery Assistant — Requirements

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Status:** Updated after Task 03 Fresh-Chat Test

## 1. Must Do Requirements

### R1. Plant Identification
The system must identify the common name of a plant from an image when the plant belongs to the supported categories.

**Done when:** A supported plant image produces a predicted common name and confidence information when available.

### R2. Plant Condition Assessment
The system must assess visible plant conditions and identify possible supported problems from the submitted image.

**Done when:** The result displays supported possible problems, or clearly states that no supported visible problem was detected. It must not claim that the plant is definitely healthy.

### R3. Multiple Possible Conditions
The system must be able to show more than one possible disease or condition when visible symptoms overlap.

**Done when:** The result can display multiple possible conditions with their names and supporting visible symptoms, and explain differences when reliable information is available.

### R4. Plant Care Information
The system must provide relevant information about the identified plant, including its common name, watering method, general care, common diseases, and available treatment guidance.

**Done when:** The plant result includes available care information relevant to that supported plant.

### R5. Qualitative Water-Need Assessment
The system must provide a qualitative indication of possible watering needs when visible signs and available information support an assessment.

**Done when:** The result provides a cautious indication with an explanation, or states that the image and available information are insufficient. It must not present an image-based estimate as an actual soil-moisture measurement.

### R6. Follow-up Questions and Additional Images
The system may ask relevant follow-up questions or request another image when the submitted information is insufficient for a useful assessment.

**Done when:** The system can request additional information when needed and use the response to improve or clarify the assessment.

### R7. Individual Plant Records
The system must maintain a separate record for each individual plant, even when multiple plants belong to the same type.

**Done when:** Each registered plant has a unique ID and its own record.

### R8. Plant Inspection History
The system must retain previous inspection results and their associated images for each individual plant.

**Done when:** The owner can open a plant record and view its previous inspections and available images.

### R9. Care and Treatment Logs
The system must allow the owner to record actions actually performed on a plant, such as watering, treatment, or other care.

**Done when:** An owner-entered action is saved with its date and details and appears in the correct plant's history.

### R10. Recommended Next Actions
The system must suggest relevant next actions based on the available inspection results and plant information.

**Done when:** The result includes suggested actions with a reason when sufficient information is available.

### R11. Follow-up Prioritization
The system must help the owner identify which plants may need attention first.

**Done when:** Plants with suggested follow-up actions can be displayed in a priority order with an explanation for each priority.

### R12. Limited Supported Categories
The first version must only identify plant types and conditions that are supported by the selected and evaluated data.

**Done when:** The supported categories are documented, and unsupported inputs are handled without fabricated predictions.

### R13. Plant Selection
Before inspecting a plant, the owner must select its existing individual record or create a new plant record.

**Done when:** An inspection is associated with the plant record selected or created by the owner. The system does not automatically match an image to an individual plant record.

### R14. Conversational Plant-Care Assistant
The system must allow the owner to communicate with an assistant, ask plant-related questions, and receive explanations and care guidance in Arabic or English.

The assistant should use relevant available information about the selected plant, including its inspection results, history, and documented plant-care knowledge.

**Done when:** The owner can ask relevant questions about a selected plant and receive responses based on available records and documented knowledge. The assistant must communicate when information is unavailable or uncertain.

## 2. Must Never Do Requirements

### N1. No Fabricated Information
The system must never invent plant names, diseases, symptoms, sources, or care instructions.

**Done when:** Unsupported information is reported as unknown or unavailable instead of being invented.

### N2. No Unsupported Certainty
The system must never present an uncertain AI prediction as a guaranteed diagnosis.

**Done when:** Uncertain or ambiguous results are clearly communicated as possibilities.

### N3. No False Water Measurements
The system must never claim that an ordinary image provides an actual soil-moisture measurement.

**Done when:** Water-need results are described as qualitative estimates, not measured values.

### N4. No False Care Records
The system must never automatically record a suggested action as an action already performed.

**Done when:** Care history only contains actions explicitly entered or confirmed by the owner.

### N5. No Guaranteed Treatment Results
The system must never guarantee that a suggested treatment will cure a plant.

**Done when:** Treatment guidance is presented with appropriate limitations and does not promise recovery.

### N6. No Unsupported Recognition
The system must never claim reliable recognition for plant types or conditions outside its documented supported categories.

**Done when:** Unsupported inputs receive a clear limitation message instead of an unsupported result.

### N7. No Automatic Individual-Plant Matching
The system must never automatically assign a submitted image to an individual plant record based on visual similarity in the first version.

**Done when:** The owner selects the individual plant record before submitting an inspection.

### N8. No Unsupported Conversational Answers
The conversational assistant must not invent answers when plant information, reliable sources, or inspection evidence is unavailable.

**Done when:** The assistant communicates uncertainty or missing information instead of presenting unsupported claims as facts.

## 3. Deferred Scope

The following features are not part of the first version:

- IoT sensors and actual soil-moisture measurements.
- Quantitative water-need measurement.
- Automated watering or physical nursery control.
- Disease severity percentages or scoring.
- Automatic matching of an individual plant from its image.
- Native Android application.
- Advanced commercial nursery-management features.