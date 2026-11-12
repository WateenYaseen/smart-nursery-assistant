# T08 — Inspection Results and History

**Priority:** High  
**Estimate:** 1 working day  
**Status:** Planned

## Why

The owner needs to review inspection results and keep saved inspection records associated with the correct individual plant.

## Done When

- The inspection result area follows the approved UI design.
- The screen can display an inspection result associated with the selected plant.
- Available possible conditions or visible problems are displayed.
- Supporting symptoms are displayed when available.
- Care guidance and recommendations are displayed when available.
- An uncertainty notice is displayed with the results.
- The owner can choose to save an inspection result.
- A saved inspection is associated with the correct plant record.
- The saved inspection includes its date and available image reference.
- Saved inspections can be retrieved as part of the plant's inspection history.
- A clear message is displayed when no result is available or saving fails.

## Touches

- Plant Inspection / Results screen.
- Inspection data model.
- Inspection storage and retrieval operations.
- Image references.
- Plant Details screen.
- Inspection history component.
- Recommendation display.

## Notes

Inspection results are possible visual assessments, not guaranteed diagnoses.

The system must not claim that an image measures actual soil moisture.

An inspection result is saved only when the owner chooses to save it. Displaying a recommendation does not mean that the owner has performed the suggested action.

If the AI model or service is not ready, use clearly identified test data only for interface and workflow testing.