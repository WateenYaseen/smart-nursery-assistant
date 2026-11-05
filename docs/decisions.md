# Smart Nursery Assistant — Decision Log

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Date:** 2026-11-05  
**Update:** After Task 03 Fresh-Chat Test

This document records the main project decisions, clarified requirements, rejected ideas, and features deferred to a later stage.

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
**Decision:** The owner will select an existing plant record or create a new record before inspection.

**Rejected for v1:** Automatic matching of a submitted image to an individual plant record.

**Reason:** Manual selection keeps each inspection associated with the intended individual plant.

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
**Decision:** The first version will be a responsive web application, primarily accessed through an Android smartphone browser.

**Rejected for v1:** A native Android application.

**Reason:** The selected delivery format is a responsive web application. Android is the primary device for initial use and testing, not the application platform.

### D15. Conversational Plant-Care Assistant
**Decision:** The first version will include a conversational assistant that allows the owner to ask plant-related questions and receive explanations and care guidance in Arabic or English.

The assistant should use available plant records, inspection results, history, and documented plant-care knowledge.

**Reason:** The project is intended to provide ongoing assistance, not only display a one-time image classification result.

### D16. Integrated Conversation Interface
**Decision:** The conversational assistant will be accessible from the inspection results and plant details screens. A separate seventh screen is not required in the current screen plan.

**Reason:** This provides conversational support within the existing plant workflow.

## 2. Rejected or Deferred Ideas

| Idea | Decision | Reason |
|---|---|---|
| Disease severity percentages | Not included in v1 | Not required for the initial goal |
| Actual soil-moisture measurement | Deferred | Requires measurement capabilities beyond ordinary images |
| IoT sensors and automatic watering | Deferred | Outside the first version |
| Automatic individual-plant image matching | Rejected for v1 | Owner will select the plant record |
| Native Android application | Not selected | Responsive web application chosen |
| Recognition of every possible plant or disease | Rejected | Support must depend on suitable data and evaluation |
| Separate conversational screen | Not currently planned | Conversation is integrated into existing screens |

## 3. Fresh-Chat Test Findings and Corrections

A fresh-chat review was performed using the twelve documentation files.

The review correctly understood the project's main purpose, intended user, individual plant records, image-based assessment, care guidance, recommendations, and scope limitations.

It identified two inconsistencies in the earlier documentation:

1. The BRD described an Android-focused application, while the architecture and technology documents selected a responsive web application.
2. The BRD described automatic image matching, while the decision log and architecture required manual plant selection.

**Corrections made:**
- Updated the BRD to describe a responsive web application primarily accessed through an Android smartphone browser.
- Removed automatic individual-plant image matching from the first-version scope.
- Updated the requirements, screens, and architecture to reflect these decisions.

The review also identified that the conversational assistant needed to be stated more clearly as a core project capability.

**Correction made:**
- Added a dedicated conversational-assistant requirement.
- Updated the BRD, screens, and architecture to describe its role and interaction flow.

## 4. Decisions Still Open

The following choices have not been finalized:

- Exact plant types and disease categories supported in the first version.
- Final training and evaluation datasets.
- Final AI model and model framework.
- Conversational AI implementation approach.
- Database technology.
- Image-storage method.
- Deployment and hosting approach.
- Offline-access requirements.
- Detailed recommendation prioritization rules.
- Detailed plant-record editing and deletion rules.
- Final evaluation metrics and acceptance thresholds.