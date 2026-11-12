# T03 — Plant Data Model and Storage

**Priority:** High  
**Estimate:** 1 working day  
**Status:** Planned

## Why

The application needs a consistent way to create, identify, and retrieve individual plant records.

## Done When

- The initial plant-record structure is implemented.
- Each plant has a unique identifier.
- A plant record supports a common name.
- A plant record supports a registration date.
- Optional plant information, such as an image reference, location, and notes, can be stored when available.
- The application can create a plant record.
- The application can retrieve the saved plant records.
- Multiple plants with the same common name can exist as separate records.
- The owner can identify an individual plant through its unique record.

## Touches

- Plant data model.
- Initial storage layer.
- Plant creation operation.
- Plant retrieval operation.
- Related application types or interfaces.

## Notes

This ticket focuses on the initial plant-record foundation only. Inspection history, recommendations, conversations, and care-action storage will be handled in their related tickets.

The final database technology should follow the project's selected technology stack. Do not assume a database provider before it has been confirmed.