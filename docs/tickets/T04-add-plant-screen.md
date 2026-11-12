# T04 — Add Plant Screen

**Priority:** High  
**Estimate:** 1 working day  
**Status:** Planned

## Why

The owner needs to register each individual plant before managing its details or starting an inspection.

## Done When

- The Add Plant screen follows the approved UI design.
- The screen includes a plant name field.
- The screen includes an optional notes field.
- The owner can select or upload an optional plant image.
- Required fields are validated before saving.
- The Save Plant action creates a separate plant record.
- A successful save displays a confirmation message.
- The owner can access the newly created plant record.
- Validation or saving errors are displayed clearly.
- Entered information is not lost when a saving error occurs.

## Touches

- Add Plant screen.
- Plant form component.
- Plant data model.
- Plant creation and storage operation.
- Image upload component, if available.
- Form validation and feedback.

## Notes

Each submission creates a new individual plant record. The system must not automatically match the uploaded image to an existing plant record.

The plant image is optional during registration.