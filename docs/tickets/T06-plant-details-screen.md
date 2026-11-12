# T06 — Plant Details Screen

**Priority:** High  
**Estimate:** 1 working day  
**Status:** Planned

## Why

The owner needs to review the information and available history of one selected plant in a single place.

## Done When

- The Plant Details screen follows the approved UI design.
- The selected plant's information is retrieved using its unique identifier.
- The screen displays the plant name and available image.
- Available notes and current follow-up information are displayed.
- The latest inspection information is displayed when available.
- Available inspection history is displayed.
- Recorded care actions are displayed when available.
- Related recommendations are displayed when available.
- A Start Inspection action opens the inspection flow for the selected plant.
- An Ask Assistant action opens the assistant with the selected plant context when supported.
- An empty state is displayed when the plant has no inspection or care history.
- A loading state is displayed while related information is retrieved.
- An error state provides a clear message and Retry action.

## Touches

- Plant Details screen.
- Plant data model.
- Plant retrieval operation.
- Inspection history display.
- Recommendation display.
- Care-action history display.
- Navigation to inspection and assistant screens.

## Notes

All displayed history must belong to the selected individual plant. Information from another plant must not be mixed into its record.