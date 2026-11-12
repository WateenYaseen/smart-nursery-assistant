# Smart Nursery Assistant — UI Design

## 1. Design Overview

Smart Nursery Assistant is a responsive, Arabic-first web application designed to help a nursery owner monitor individual plants, review possible plant problems, receive care recommendations, and ask an AI assistant questions.

The interface follows a mobile-first approach because the main user is expected to access the application through a mobile browser.

### Design Principles

- Arabic is the primary language, with right-to-left (RTL) layout.
- Use simple, clear, and gender-neutral wording.
- Keep the interface easy to understand and navigate.
- Display AI recommendations clearly without presenting results as guaranteed diagnoses.
- Keep a separate record for each individual plant.
- Use consistent navigation and visual components across all screens.
- Provide clear feedback when an action succeeds, fails, or is in progress.

## 2. Screen 1 — Home Dashboard

### Purpose

Provide a quick overview of the nursery and highlight plants that may need attention.

### Main Elements

- Welcome message.
- Total number of registered plants.
- Plants that need follow-up.
- Recently added plants.
- Quick actions: Add Plant and Start Inspection.
- Recent plant activity.
- Main navigation.

### Data Sources

- Registered plant records.
- Latest inspection records.
- Owner-confirmed care actions.
- Pending recommendations.
- Saved plant records and their latest available statuses.

### User Actions

- Open a plant's details.
- Add a new plant.
- Start an inspection.
- Open the AI Assistant.
- Navigate to My Plants.

### UI States

- **Empty:** No plants are registered. Show a short welcome message and an "Add First Plant" action.
- **Loading:** Show loading indicators while retrieving plant counts, follow-up information, and recent activity.
- **Error:** Show a clear message if dashboard data cannot be loaded, with a Retry action.
- **Full:** Display plant counts, follow-up reminders, recent activity, and quick actions using available records.

## 3. Screen 2 — My Plants

### Purpose

Display all registered plants and allow the owner to find and open an individual plant record.

### Main Elements

- Screen title.
- Plant list.
- Plant name and optional image.
- Short status or follow-up indicator.
- Last inspection date, when available.
- Search or filter controls, if implemented.
- Add Plant action.
- Main navigation.

### Data Sources

- Saved plant records.
- Latest inspection associated with each plant.
- Available recommendations and follow-up information.

### User Actions

- Open an individual plant record.
- Search or filter plants, if available.
- Add a new plant.

### UI States

- **Empty:** No plant records exist. Show an explanation and an Add Plant action.
- **Loading:** Show placeholder cards while the plant list is retrieved.
- **Error:** Show a message explaining that the plant list could not be loaded and provide Retry.
- **Full:** Display the saved plants with their available images, names, and latest follow-up information.

## 4. Screen 3 — Add Plant

### Purpose

Allow the owner to create a separate record for an individual plant.

### Main Elements

- Screen title.
- Plant image upload option.
- Plant name field.
- Optional notes field.
- Save Plant action.
- Cancel or Back action.

### Data Sources

- Information entered by the owner.
- Uploaded plant image, when provided.

### User Actions

- Upload or select a plant image.
- Enter a plant name.
- Add optional notes.
- Save the new plant record.
- Cancel and return to the previous screen.

### UI States

- **Empty:** Display the blank form and explain which information is required.
- **Loading:** Show a saving indicator while the plant record and optional image are being saved.
- **Error:** Display a clear validation or saving error and allow the owner to try again without losing entered information.
- **Full:** Display the completed form with the entered plant information, ready for submission. After successful saving, show a confirmation message and provide access to the new plant record.

## 5. Screen 4 — Plant Details

### Purpose

Show the information and history associated with one selected plant.

### Main Elements

- Plant name and image.
- Current follow-up indicator, if available.
- Plant notes.
- Care summary.
- Latest inspection information.
- Inspection history.
- Recorded care actions.
- Related recommendations.
- Start Inspection action.
- Ask Assistant action.

### Data Sources

- Selected plant record.
- Inspection history linked to that plant.
- Care actions confirmed by the owner.
- Care recommendations generated for the selected plant.
- Related assistant conversations, when available.

### User Actions

- Start a new inspection for this plant.
- View a previous inspection.
- Ask the AI Assistant about this plant.
- Review care recommendations.
- Record a care action after it has been performed.
- Review available plant history.

### UI States

- **Empty:** The plant record exists, but no inspection or care history is available. Show the available plant information and actions to get started.
- **Loading:** Show placeholders while plant details and related records are retrieved.
- **Error:** Show a clear message if plant details or related records cannot be retrieved, with a Retry action.
- **Full:** Display the plant information, latest inspection, care summary, recommendations, and available history.

## 6. Screen 5 — Plant Inspection / Results

### Purpose

Allow the owner to submit a plant image and review possible visible problems and care recommendations.

### Main Elements

- Selected plant name.
- Image upload or change option.
- Start Inspection action.
- Inspection result.
- Possible problems or diseases.
- Visible symptoms.
- Explanation of uncertainty.
- Care and follow-up recommendations.
- Save Inspection Result action.

### Data Sources

- Selected plant record.
- Uploaded image.
- AI image-analysis output.
- Plant-care knowledge source, when available.

### User Actions

- Select or change the image.
- Start image analysis.
- Review possible issues and visible symptoms.
- Read suggested care actions.
- Save the inspection result to the selected plant's history.

### UI States

- **Empty:** No image has been selected. Show an image-upload area and a short instruction.
- **Loading:** Show a progress indicator while the image is being analyzed. Prevent duplicate submissions where appropriate.
- **Error:** Show a message if the image upload or analysis fails, with an option to retry.
- **Full:** Display the uploaded image, possible issues, visible symptoms, uncertainty notice, and care recommendations.

### Important Notes

- Results are visual possibilities, not guaranteed diagnoses.
- The system must communicate uncertainty when the image does not provide enough evidence.
- Recommendations should not imply that soil moisture has been measured.
- The owner decides whether to perform a recommended action.
- An inspection result is saved only when the owner chooses to save it.
- Every inspection must be associated with the plant selected by the owner.
- Saving an inspection does not automatically mark recommended care actions as completed.

## 7. Screen 6 — AI Assistant Chat

### Purpose

Provide a conversational assistant for plant-care questions, using the selected plant's context when available.

### Main Elements

- Conversation area.
- Selected plant context, when applicable.
- Suggested example questions.
- Message input field.
- Send action.
- Assistant responses.
- Clear indication when the assistant is uncertain.
- Available conversation history.

### Data Sources

- User messages.
- Assistant responses.
- Selected plant record, if one is selected.
- Relevant saved inspection and care history.
- Available plant-care knowledge source.
- Saved conversation history and related messages.

### User Actions

- Ask a plant-care question.
- Send a message.
- Continue an existing conversation.
- Ask about the selected plant.
- Open a plant record when needed.
- View previous conversations, when available.

### UI States

- **Empty:** No messages exist yet. Show a welcome message and a few example questions.
- **Loading:** Show an assistant typing or response-loading indicator after a message is sent.
- **Error:** Show a message if sending or receiving a response fails, with an option to retry.
- **Full:** Display the conversation history, assistant responses, and the message input area.

### Important Notes

- The assistant should use the selected plant's context when relevant.
- Previous conversation messages should remain associated with their original conversation.
- The assistant should communicate uncertainty when reliable information is unavailable.
- Plant-care guidance should use available reference information when relevant.

## 8. Navigation and Consistency

The six screens use a consistent navigation structure:

- Home
- My Plants
- Assistant

Other screens are reached through actions from these main sections.

The interface should maintain:

- Consistent colors, typography, spacing, and buttons.
- Clear Arabic labels and RTL alignment.
- Visible feedback after important actions.
- Readable error and empty-state messages.
- Responsive behavior on mobile and desktop browsers.
- Consistent plant information and navigation across related screens.

## 9. Design Scope and Limitations

The current design represents the planned MVP interface. It does not imply that the application or AI model has already been implemented.

The MVP does not include:

- IoT sensors or automatic irrigation.
- Actual soil-moisture measurement.
- Continuous camera monitoring.
- Guaranteed plant disease diagnosis.
- Automatic recording of care actions that the owner has not confirmed.
- Automatic matching of uploaded images to individual plant records.
- Employee, inventory, sales, or accounting management.

The six visual screen designs are provided in the Canva design:

**Smart Nursery Assistant — Mobile App UI**

[Open the Canva design](https://www.canva.com/design/DAHatncfoL4/C4oqAlofNMjiIzYQ-hxwAA/edit)

## 10. Design and Implementation Notes

This document describes the intended interface behavior and the information required by each screen.

The four UI states are documented for each screen to guide future implementation and testing.

The visual designs are maintained separately in Canva. The application structure, database implementation, and AI integration will be developed in later implementation tasks.

The design may be refined during development when technical limitations or usability testing reveal necessary changes.