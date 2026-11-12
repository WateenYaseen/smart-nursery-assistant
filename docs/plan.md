# Project Plan

**Last Updated:** 2026-11-12

## 1. Project Goal

Build a responsive, Arabic-first web application that helps a nursery owner manage individual plant records, inspect plants using images, understand possible visible problems, and receive practical plant-care guidance through an AI assistant.

The MVP will focus on the real needs of the nursery and will be developed incrementally.

## 2. Target User

The primary user is the nursery owner.

The application should make it easy to:
- Register and manage individual plants.
- Inspect a selected plant using an uploaded image.
- Review possible conditions and visible symptoms.
- Access plant-care and watering guidance.
- Ask questions through the AI assistant.
- Review previous inspections and recorded care actions.

## 3. Agreed MVP Scope

### Included
- Responsive web application with a mobile-first layout.
- Arabic as the primary language and English as a secondary language.
- Six main application screens.
- Separate records for individual plants.
- Manual plant-record selection before inspection.
- Image-based plant identification for supported plants.
- Assessment of possible visible problems and symptoms.
- Qualitative watering and care recommendations.
- Saved inspection records and history.
- Conversational AI assistant with plant context when available.
- Owner-confirmed care-action tracking.

### Excluded from the MVP
- Automatic matching of uploaded images to existing plant records.
- Guaranteed disease diagnosis or treatment outcomes.
- Actual soil-moisture measurement.
- IoT sensors and automatic irrigation.
- Native Android application.
- Recognition of every plant type or disease.

## 4. Project Phases

| Phase | Focus | Status |
|---|---|---|
| Task 01 | Project idea and problem definition | Completed |
| Task 02 | Initial research and project planning | Completed |
| Task 03 | Requirements and project documentation | Completed |
| Task 04 | UI design and development backlog | Prepared |
| Task 05 | Initial application implementation | Next |

## 5. UI Design Plan

The application has six main screens:

1. **Home Dashboard:** Overview of plants and items that need attention.
2. **My Plants:** List of registered individual plants.
3. **Add Plant:** Form to create a new plant record.
4. **Plant Details:** Information, inspection history, recommendations, and care actions for one plant.
5. **Plant Inspection / Results:** Upload an image and review the inspection result.
6. **AI Assistant Chat:** Ask plant-care questions and use plant context when available.

Each screen should support four UI states:
- **Empty:** No relevant data is available yet.
- **Loading:** Data or an operation is being processed.
- **Error:** Something failed, with a clear recovery action when possible.
- **Full:** The screen displays its available content.

Detailed screen behavior and states are documented in `design.md`.

## 6. Development Backlog

Development is organized into ten small tickets, each intended to fit within approximately one working day.

| Order | Ticket | Priority |
|---|---|---|
| T01 | Application Structure | High |
| T02 | Main Navigation and Routes | High |
| T03 | Plant Data Model and Storage | High |
| T04 | Add Plant Screen | High |
| T05 | My Plants Screen | High |
| T06 | Plant Details Screen | High |
| T07 | Image Upload and Inspection Flow | High |
| T08 | Inspection Results and History | High |
| T09 | AI Assistant Chat Interface | Medium |
| T10 | Owner-Confirmed Care Actions | Medium |

The full ticket descriptions, completion criteria, and implementation order are available in `docs/tickets/README.md`.

## 7. Immediate Development Plan

The first three tickets are planned as the next development steps:

1. **T01 — Application Structure:** Set up the project, basic folder structure, entry point, and responsive foundation.
2. **T02 — Main Navigation and Routes:** Create navigation and routes for the six application screens.
3. **T03 — Plant Data Model and Storage:** Establish individual plant records with unique IDs and basic create/retrieve operations.

Each ticket will be implemented and checked separately before moving forward.

## 8. Technical Planning

The final technology choices will be confirmed during implementation.

The project still needs to evaluate:
- Suitable plant-image datasets and their licensing.
- Dataset quality, labels, and coverage of relevant plants.
- AI model and inference approach.
- Conversational assistant integration.
- Database and image storage.
- Hosting and deployment.

No specific dataset, trained model, or external service should be treated as finalized until it has been evaluated.

## 9. Development Principles

- Keep the MVP focused on the nursery owner's actual needs.
- Prefer simple, understandable user flows.
- Keep each plant's record separate.
- Require manual plant selection before inspection.
- Communicate uncertainty in AI-generated results.
- Distinguish recommendations from care actions confirmed by the owner.
- Test each ticket before starting the next.
- Record important scope or technical changes in `decisions.md`.

## 10. Current Project Status

Planning, requirements, initial research, UI design, and backlog preparation have been completed or prepared.

The next stage is to begin implementation with T01, followed by T02 and T03.