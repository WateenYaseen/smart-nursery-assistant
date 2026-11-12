# T10 — Owner-Confirmed Care Actions

**Priority:** Medium  
**Estimate:** 1 working day  
**Status:** Planned

## Why

The owner needs to record care actions that have actually been performed so the plant's history remains accurate.

## Done When

- The owner can access a way to record a care action for a selected plant.
- The care-action form includes an action type.
- The owner can enter optional action details.
- The action date is recorded.
- The action is associated with the correct individual plant.
- A saved care action appears in the plant's care history.
- A related recommendation can be linked when applicable.
- A confirmation message is displayed after successful saving.
- Validation or saving errors are displayed clearly.
- Recommendations are not automatically recorded as completed actions.

## Touches

- Plant Details screen.
- Care-action form or component.
- Care Action data model.
- Care-action storage operation.
- Plant care history display.
- Recommendation status handling.

## Notes

Only actions explicitly entered or confirmed by the owner may be stored as performed actions.

The system must distinguish between a suggested action and an action that has actually happened.

This ticket does not include automatic watering, IoT control, or sensor-based care tracking.