# T07 — Image Upload and Inspection Flow

**Priority:** High  
**Estimate:** 1 working day  
**Status:** Planned

## Why

The owner needs to submit an image of a selected plant to begin an AI-assisted inspection.

## Done When

- The inspection screen follows the approved UI design.
- The selected plant's name is displayed.
- The owner can select or upload a plant image.
- The selected image can be previewed before analysis.
- The owner can change the selected image before starting.
- The Start Inspection action validates that an image has been selected.
- A loading state is displayed while the inspection request is processed.
- Duplicate submissions are prevented while a request is in progress.
- Upload or processing errors are displayed clearly.
- The inspection request remains associated with the plant selected by the owner.

## Touches

- Plant Inspection / Results screen.
- Image upload component.
- Image preview component.
- Selected plant context.
- Inspection request flow.
- Loading and error states.

## Notes

This ticket covers the image submission and inspection workflow. It does not require a fully trained or validated AI model.

If the final AI service is not yet available, use a clearly identified placeholder or mock response for interface testing. Do not present mock results as real AI predictions.

The system must not automatically match an image to an individual plant record.