# Smart Nursery Assistant — Decision Log

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Last Updated:** 2026-11-12  
**Update:** After Task 04 — Design and Backlog Preparation

This document records the confirmed project decisions, design choices, rejected ideas, deferred features, and remaining open decisions for Smart Nursery Assistant.

## 1. Confirmed Project Decisions

### D1. Image-Based Plant Inspection
**Decision:** The first version will use plant images as the main input for AI-assisted plant identification and visible condition assessment.

**Reason:** Images provide a practical starting point for inspecting plants without requiring additional physical equipment.

### D2. Common Plant Name
**Decision:** The system will display the plant's common name. A full botanical name is not required in the first version.

**Reason:** Common names are more practical for the intended nursery workflow.

### D3. Visible Condition Assessment
**Decision:** The system will identify possible supported diseases or visible plant problems and explain the symptoms observed.

**Reason:** The owner needs useful information about what may be affecting a plant and how to respond.

### D4. Multiple Possible Conditions
**Decision:** The system may display more than one possible disease or condition when visible symptoms overlap.

**Reason:** A single image may not provide enough evidence to distinguish between similar problems.

### D5. No Disease Severity Scoring
**Decision:** Disease severity percentages or numerical severity scores are not required in the first version.

**Reason:** The initial focus is identifying possible problems and providing useful guidance rather than estimating disease severity.

### D6. Follow-up Questions and Images
**Decision:** The assistant may ask relevant follow-up questions or request additional images when the available information is insufficient.

**Reason:** Additional information may help clarify uncertain assessments.

### D7. Separate Individual Plant Records
**Decision:** Every individual plant will have its own record, even when multiple plants belong to the same species.

**Reason:** The owner needs to track the inspection and care history of each individual plant separately.

### D8. Manual Plant Selection
**Decision:** Before an inspection, the owner will select an existing plant record or create a new one.

**Rejected for v1:** Automatically matching an uploaded image to an individual plant record.

**Reason:** Manual selection keeps each inspection associated with the intended plant.

### D9. Plant Inspection History
**Decision:** The system will retain previous inspection results and associated images for each plant.

**Reason:** Previous inspections help the owner review changes in the plant's condition over time.

### D10. Explicit Care-Action Logging
**Decision:** The owner must explicitly record care actions that have actually been performed.

**Reason:** A suggested action must not be confused with an action that has already happened.

### D11. Recommended Next Actions
**Decision:** The system will suggest relevant next actions and help prioritize plants that may need attention, with explanations.

**Reason:** The owner needs help deciding which plants to inspect or handle first.

### D12. Qualitative Water-Need Assessment
**Decision:** Watering guidance may be provided qualitatively when supported by visible signs and available information. The system will not claim to measure actual soil moisture from an image.

**Reason:** An ordinary plant image cannot reliably measure moisture inside the soil.

### D13. Limited Supported Categories
**Decision:** The first version will support only plant types and conditions for which suitable data and evaluation are available.

**Reason:** The system should not claim recognition capabilities that have not been supported and evaluated.

### D14. Responsive Web Application
**Decision:** The first version will be a responsive web application, primarily accessed through an Android smartphone browser.

**Rejected for v1:** A native Android application.

**Reason:** A responsive web application is the selected delivery format. Android is the primary device for initial use and testing, not the application platform.

### D15. Conversational Plant-Care Assistant
**Decision:** The first version will include a conversational assistant that allows the owner to ask plant-related questions and receive explanations and care guidance in Arabic or English.

The assistant should use available plant records, inspection results, plant history, and documented plant-care knowledge when relevant.

**Reason:** The project is intended to provide ongoing assistance, not only a one-time image classification result.

### D16. Integrated Assistant Screen
**Decision:** The current design includes six main screens, including a dedicated AI Assistant Chat screen. The assistant will also be accessible from relevant plant details and inspection-result workflows.

**Reason:** A dedicated chat interface provides a clear place for ongoing questions while keeping the assistant connected to individual plant records.

### D17. Arabic-First Interface
**Decision:** Arabic will be the primary interface language, with English as a secondary language.

**Reason:** The application is intended for use in a Jordanian nursery, so Arabic accessibility is important.

### D18. Individual Plant Context in Chat
**Decision:** The assistant should use the selected plant's information and available history when the conversation is related to that plant.

**Reason:** Plant-specific context makes the guidance more relevant and avoids treating every question as unrelated to previous inspections.

### D19. Save Inspection Records
**Decision:** Inspection results and related images should be saved and associated with the selected plant record.

**Reason:** The owner needs to review previous findings and compare the plant's condition over time.

### D20. Recommendations Are Not Completed Actions
**Decision:** AI recommendations will remain suggestions until the owner confirms that an action has been performed and records it.

**Reason:** The system must keep recommendations separate from actual nursery activities.

## 2. UI and Design Decisions

### D21. Six Main Application Screens
**Decision:** The first-version interface will contain six main screens:

1. Home Dashboard
2. My Plants
3. Add Plant
4. Plant Details
5. Plant Inspection / Results
6. AI Assistant Chat

**Reason:** These screens cover the main workflow from viewing nursery status and adding plants to inspecting them, reviewing results, and asking the assistant for guidance.

### D22. Mobile-First Responsive Layout
**Decision:** The interface will prioritize mobile usability while remaining responsive to larger screens.

**Reason:** The owner is expected to use the application mainly through a smartphone browser.

### D23. Simple and Clear Interface
**Decision:** The interface will use clear navigation, readable Arabic text, simple actions, and consistent screen layouts.

**Reason:** The application should be practical for everyday nursery use and should not require advanced technical knowledge.

### D24. Visual Design Direction
**Decision:** The interface will use a calm, nature-inspired visual style with a cream background, green accents, and purple/lavender supporting colors.

**Reason:** These colors support a clear plant-care identity while keeping the interface comfortable and visually organized.

### D25. Consistent Screen States
**Decision:** Each of the six screens will document four interface states: Empty, Loading, Error, and Full.

**Reason:** Documenting these states clarifies how each screen should behave when data is missing, being loaded, unavailable, or successfully displayed.

### D26. Design Documentation
**Decision:** The six screen designs will be maintained in Canva, while their purposes, elements, data sources, actions, and four states will be documented in `docs/design.md`.

**Reason:** The visual design and implementation details need to be documented separately and clearly.

## 3. Development and Backlog Decisions

### D27. Small Implementation Tickets
**Decision:** Development work will be divided into small, independently understandable tickets, each intended to fit approximately one working day.

**Reason:** Small tickets make the solo development process easier to plan, implement, test, and review.

### D28. Implementation Order
**Decision:** Development will begin with the application structure, navigation, and plant data model before implementing the main plant-management and AI features.

**Reason:** The core application structure and data model are needed before the remaining features can work consistently.

### D29. One Ticket at a Time
**Decision:** Tickets will be implemented in the documented order, with progress reviewed before moving to the next ticket.

**Reason:** This reduces overlapping changes and makes problems easier to identify and fix.

### D30. First Development Priorities
**Decision:** The first three planned development tickets are:

1. T01 — Application Structure
2. T02 — Main Navigation and Routes
3. T03 — Plant Data Model and Storage

**Reason:** These tasks establish the foundation required for the remaining application features.

## 4. Rejected or Deferred Ideas

| Idea | Decision | Reason |
|---|---|---|
| Disease severity percentages | Not included in v1 | Not required for the initial goal |
| Actual soil-moisture measurement | Deferred | Requires physical measurement capabilities |
| IoT sensors | Deferred | Outside the first version |
| Automatic watering system | Deferred | Outside the first version |
| Automatic individual-plant image matching | Rejected for v1 | The owner will select the plant record |
| Native Android application | Not selected | Responsive web application chosen |
| Recognition of every possible plant or disease | Rejected | Support depends on suitable data and evaluation |
| Guaranteed AI diagnosis | Rejected | Image-based assessment may be uncertain |
| Automatic logging of care actions | Rejected | The owner must confirm performed actions |
| Continuous nursery camera monitoring | Deferred | Not required for the first version |
| Offline-first functionality | Not confirmed | Requires further technical evaluation |
| Employee, inventory, sales, and accounting management | Outside v1 | Not part of the core plant-care objective |

## 5. Fresh-Chat Test Findings and Corrections

A fresh-chat review was performed using the twelve project documentation files prepared for Task 03.

The review correctly understood the project's main purpose, intended user, individual plant records, image-based assessment, care guidance, recommendations, and scope limitations.

It identified inconsistencies in the earlier documentation:

1. The BRD described an Android-focused application, while the architecture and technology documents selected a responsive web application.
2. The BRD described automatic image matching, while the decision log and architecture required manual plant selection.
3. The conversational assistant needed to be stated more clearly as a core project capability.

**Corrections made:**

- Updated the project description to specify a responsive web application primarily accessed through an Android smartphone browser.
- Removed automatic individual-plant image matching from the first-version scope.
- Clarified manual plant selection before inspection.
- Added the conversational assistant as a core capability.
- Clarified the relationship between the assistant, individual plant records, inspection results, and plant history.
- Updated the relevant requirements, screen descriptions, and architecture documentation.

## 6. Decisions Still Open

The following decisions have not yet been finalized:

- Exact plant types and disease categories supported in the first version.
- Final training and evaluation datasets.
- Dataset suitability, label quality, licensing, and coverage.
- Final AI model and model framework.
- Conversational AI implementation approach.
- Database technology.
- Image-storage method.
- Deployment and hosting approach.
- Offline-access requirements.
- Detailed recommendation prioritization rules.
- Detailed plant-record editing and deletion rules.
- Final evaluation metrics and acceptance thresholds.
- Exact method for retaining and retrieving conversation history.

These decisions will be finalized during implementation and testing when technical feasibility and available resources are clearer.

## 7. Current Project Status

At the time of this update:

- The six main application screens have been prepared in Canva.
- The design documentation is being prepared in `docs/design.md`.
- The development backlog is being organized into ten implementation tickets under `docs/tickets/`.
- The implementation architecture and data model still require review during development.
- No final AI model has been selected or trained.
- No complete application implementation has been completed yet.

This decision log will be updated whenever a major project decision changes or a previously open decision is finalized.