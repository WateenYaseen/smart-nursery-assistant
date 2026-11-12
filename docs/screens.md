# Smart Nursery Assistant — Application Screens

**Status:** Updated after Task 04 UI Design and Backlog

## Overview

The Smart Nursery Assistant MVP consists of six main application screens. The interface is designed to help the nursery owner manage individual plant records, inspect plants, review results, and communicate with an AI assistant.

The application uses a mobile-first design with Arabic as the primary language and English as a secondary language.

## Screen 1: Home Dashboard

The main screen provides an overview of the nursery and quick access to the application's main features.

**Main elements:**
- Welcome section.
- Nursery overview.
- Quick access to My Plants.
- Recent activity or inspections.
- Navigation to the main application sections.

**Main actions:**
- Open the plant collection.
- Add a new plant.
- Access the AI Assistant.

## Screen 2: My Plants

Displays the plants saved in the user's nursery.

**Main elements:**
- List or grid of saved plants.
- Plant images and names.
- Basic plant information.
- Search or filtering options.

**Main actions:**
- View a plant's details.
- Select a plant record.
- Add a new plant.

The user selects the plant record manually. The application does not automatically match uploaded photos to existing plant records.

## Screen 3: Add Plant

Allows the user to create an individual plant record.

**Main elements:**
- Plant image upload.
- Plant name.
- Plant type or category.
- Optional notes.

**Main actions:**
- Enter plant information.
- Upload a plant image.
- Save the plant record.

## Screen 4: Plant Details

Displays the saved information for one selected plant.

**Main elements:**
- Plant image and name.
- Plant information.
- Care information.
- Inspection history.
- Previous care actions.

**Main actions:**
- Start a new inspection.
- Review previous inspections.
- Record a care action.
- Open the AI Assistant with the selected plant context.

## Screen 5: Plant Inspection / Results

Allows the user to upload a photo of the selected plant and review the AI-generated inspection result.

**Main elements:**
- Selected plant information.
- Image upload area.
- Inspection progress.
- Possible plant condition or disease results.
- Care and watering recommendations.

**Main actions:**
- Upload a plant image.
- Start an inspection.
- Review the generated result.
- Save the inspection to the plant's history.

The results provide possible conditions and guidance, not a guaranteed medical or agricultural diagnosis. Watering recommendations are qualitative and are not based on actual soil sensor measurements.

## Screen 6: AI Assistant Chat

Provides a conversational interface for asking questions about plants and their care.

**Main elements:**
- Chat message area.
- Message input.
- Send action.
- Selected plant context when available.

**Main actions:**
- Ask plant-care questions.
- Discuss inspection results.
- Request watering and general care guidance.
- Continue discussing a previously selected plant using its saved record and available history.

## Navigation Summary

The six screens are connected through the main application navigation and plant-specific actions.

The user can move from the Home Dashboard to My Plants, create a plant record, open its details, inspect it, review results, and access the AI Assistant.

## Scope Limitations

- No automatic photo matching between uploaded images and saved plant records.
- No IoT sensors or automatic irrigation in the MVP.
- No guaranteed disease diagnosis.
- No automatic watering or treatment execution.
- AI-generated recommendations are guidance for the user to review and confirm.