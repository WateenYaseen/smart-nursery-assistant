# Smart Nursery Assistant — Decision Log

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Date:** 2026-11-05

This document records the main project decisions made during Task 03, including clarified requirements, rejected ideas, and features deferred to a later stage.

## 1. Confirmed Decisions

### D1. Image-Based Plant Inspection
**Decision:** The first version will use plant images as the main input for AI-assisted identification and condition assessment.

**Reason:** Images provide a practical starting point for inspecting plants without requiring additional physical equipment.

### D2. Common Plant Name
**Decision:** The system should display the plant's common name. A full botanical name is not required in the first version.

**Reason:** The common name is more practical for the intended nursery workflow.

### D3. Visible Condition Assessment
**Decision:** The system should identify possible supported diseases or visible problems and explain the relevant symptoms.

**Reason:** The owner needs useful information about what may be wrong with a plant and how to respond.

### D4. Multiple Possible Conditions
**Decision:** The system may display multiple possible diseases or conditions when symptoms overlap.

**Reason:** A single image may not provide enough evidence to distinguish between similar problems.

### D5. No Disease Severity Scoring
**Decision:** Disease severity percentages or scoring are not required in the first version.

**Reason:** The initial focus is identifying possible problems and providing handling guidance, rather than estimating severity.

### D6. Follow-up Questions and Images
**Decision:** The system is allowed to ask relevant questions or request additional images when the available information is insufficient.

**Reason:** Additional information may help clarify an uncertain assessment.

### D7. Separate Individual Plant Records
**Decision:** Every individual plant must have its own record, even when multiple plants belong to the same species.

**Reason:** The owner needs to track the inspection and care history of each plant separately.

### D8. Owner Selects the Plant
**Decision:** The owner will select an existing plant record before inspection or create a new record.

**Reason:** Automatic matching of an image to an individual plant is not part of the first version.

### D9. Plant History
**Decision:** The system will retain previous inspection results and associated images for each plant.

**Reason:** Previous inspections help the owner review changes over time.

### D10. Explicit Care-Action Logging
**Decision:** The owner must explicitly record care actions that were actually performed.

**Reason:** A suggested action must not be confused with an action that has already happened.

### D11. Recommended Next Actions
**Decision:** The system should suggest next actions and prioritize plants that may need attention, with explanations.

**Reason:** The system should help the owner decide what to check or handle next.

### D12. Qualitative Water-Need Assessment
**Decision:** Watering needs may be described qualitatively when supported by visible signs and available information. Actual soil-moisture measurement is not included.

**Reason:** An ordinary image cannot reliably measure the moisture level inside the soil.

### D13. Limited Supported Categories
**Decision:** The first version will support only plant types and conditions for which suitable data and evaluation are available.

**Reason:** The system should not claim recognition capabilities that have not been supported and evaluated.

### D14. Responsive Web Application
**Decision:** The first version will be developed as a responsive web application.

**Rejected alternative:** A native Android application as the initial delivery format.

**Reason:** A responsive web application is the selected initial direction.

## 2. Rejected or Deferred Ideas

| Idea | Decision | Reason |
|---|---|---|
| Disease severity percentages | Not included in v1 | Not required for the initial goal |
| Actual soil-moisture measurement | Deferred | Requires measurement capabilities beyond ordinary images |
| IoT sensors and automatic watering | Deferred | Outside the first version |
| Automatic individual-plant image matching | Rejected for v1 | Owner will select the plant record |
| Native Android application | Not selected | Responsive web application chosen |
| Recognition of every possible plant or disease | Rejected | Support must depend on suitable data and evaluation |

## 3. Arguments and Clarifications During Planning

- The meaning of the follow-up input requirement was clarified: the system **may** request another image or ask relevant questions when necessary.
- The initial idea of including disease severity was removed. Identifying possible diseases and explaining how to handle them is the priority.
- Water-need assessment was limited to qualitative guidance, not actual moisture measurement.
- Individual plant records were kept separate instead of grouping all plants of the same type together.
- Suggested care actions were separated from owner-confirmed actions to avoid inaccurate history records.

## 4. Decisions Still Open

The following choices have not been finalized:

- Exact plant types and disease categories supported in the first version.
- Final training and evaluation datasets.
- Final AI model and model framework.
- Database technology.
- Image-storage method.
- Deployment and hosting approach.
- Final evaluation metrics and acceptance thresholds.