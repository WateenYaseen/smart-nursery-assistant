# Smart Nursery Assistant — Development Tickets

This folder contains the implementation backlog for the Smart Nursery Assistant MVP.

The tickets are organized in a practical development order. Each ticket is intended to represent a small task that can be completed, tested, and reviewed independently, approximately within one working day.

## 1. Development Order

| Order | Ticket | Title | Priority |
|---|---|---|---|
| 1 | T01 | Application Structure | High |
| 2 | T02 | Main Navigation and Routes | High |
| 3 | T03 | Plant Data Model and Storage | High |
| 4 | T04 | Add Plant Screen | High |
| 5 | T05 | My Plants Screen | High |
| 6 | T06 | Plant Details Screen | High |
| 7 | T07 | Image Upload and Inspection Flow | High |
| 8 | T08 | Inspection Results and History | High |
| 9 | T09 | AI Assistant Chat Interface | Medium |
| 10 | T10 | Owner-Confirmed Care Actions | Medium |

## 2. Why This Order?

The development starts with the basic application structure and navigation so that the main screens have a stable foundation.

The plant data model and storage are implemented before plant-management features because the application needs a consistent way to create and retrieve individual plant records.

The Add Plant and My Plants screens establish the basic plant-management workflow. Plant Details then brings together the information and history associated with an individual plant.

Image upload and inspection flow are implemented before displaying inspection results and history.

The assistant interface follows the plant and inspection foundations so it can use relevant plant context and available records.

Finally, owner-confirmed care-action logging connects recommendations with actions that were actually performed.

## 3. First Three Tickets

The first three planned development tasks are:

1. **T01 — Application Structure:** Set up the basic application project and folder organization.
2. **T02 — Main Navigation and Routes:** Add navigation between Home, My Plants, and Assistant, with access to the other screens.
3. **T03 — Plant Data Model and Storage:** Define and implement the initial plant-record structure and basic storage operations.

These tasks provide the foundation for the remaining implementation work.

## 4. Definition of Done

A ticket is considered complete when:

- Its stated requirements have been implemented.
- The listed acceptance conditions can be tested.
- The affected screens or components work as expected.
- No unrelated functionality has been added.
- Relevant documentation is updated when necessary.
- The changes are reviewed before moving to the next ticket.

## 5. Scope Notes

- The first version is a responsive, Arabic-first web application.
- The interface is mobile-first and supports right-to-left Arabic layout.
- Each individual plant has a separate record.
- The owner selects the plant before starting an inspection.
- AI results are possible visual assessments, not guaranteed diagnoses.
- Recommendations are separate from owner-confirmed care actions.
- IoT sensors, automatic irrigation, and actual soil-moisture measurement are outside the MVP.
- AI model training and final model selection are not assumed to be completed by these interface and foundation tickets.

The tickets may be refined during implementation if technical findings require changes. Any major scope or architecture change should be documented in `docs/decisions.md`.