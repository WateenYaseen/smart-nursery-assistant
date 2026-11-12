# Smart Nursery Assistant

An AI-powered web application that helps nursery owners monitor individual plants, understand visible plant problems, and access practical plant-care guidance.

## Project Overview

Smart Nursery Assistant is designed around a real nursery environment. It helps the owner keep plant records, inspect plants using images, review possible conditions, and receive care recommendations through an AI-powered assistant.

The application is designed primarily for mobile use while remaining responsive on other screen sizes.

## Main Features

- **Plant Identification:** Suggests the common name of supported plants from uploaded images.
- **Plant Condition Assessment:** Identifies possible visible problems, symptoms, or diseases, while communicating uncertainty.
- **Plant Care Guidance:** Provides practical care recommendations, including watering guidance.
- **Individual Plant Records:** Keeps a separate record for each plant, even when multiple plants belong to the same type.
- **Inspection History:** Saves inspection results and related images for future reference.
- **AI Care Assistant:** Allows the owner to ask plant-care questions in Arabic or English, with plant context when available.
- **Care Action Tracking:** Records care actions only after the owner confirms that they were performed.
- **Recommendations:** Organizes suggested next steps with reasons and priorities.

## Important Scope Decisions

- The owner manually selects an existing plant record or creates a new one before starting an inspection.
- The application does not automatically match uploaded photos to plant records.
- Image-based results are guidance, not guaranteed diagnoses.
- Watering guidance is qualitative; the application does not measure actual soil moisture.
- IoT devices, sensors, and automatic irrigation are outside the current MVP scope.
- Arabic is the primary interface language, with English as a secondary option.

## Technology and Implementation

The project is currently in the design and development-planning stage. The technology stack and AI implementation details will be finalized as development progresses.

No trained AI model or completed application is claimed at this stage.

## Current Status

- Project idea, target user, and MVP scope defined.
- Task 03 documentation prepared and refined.
- Six application screens designed in Canva.
- Task 04 design documentation and development backlog prepared.
- Ten development tickets organized in implementation order.
- Next step: begin implementation with T01, T02, and T03, one ticket at a time.

## Documentation

Project documentation is available in the `docs/` folder:

| File | Description |
|---|---|
| `brief.md` | Project overview and problem definition |
| `plan.md` | Project plan and current development direction |
| `progress.md` | Completed work and next steps |
| `research.md` | Research and supporting information |
| `requirements.md` | Functional and non-functional requirements |
| `screens.md` | Main application screens |
| `design.md` | Screen design details and UI states |
| `data-model.md` | Conceptual data model |
| `architecture.md` | Proposed application architecture |
| `stack.md` | Technology stack considerations |
| `rules.md` | Project rules and development guidelines |
| `decisions.md` | Project decision log |
| `workflow.md` | Project workflow |
| `tickets/README.md` | Development backlog and implementation order |

## Project Structure

```text
smart-nursery-assistant/
├── README.md
└── docs/
    ├── architecture.md
    ├── brief.md
    ├── data-model.md
    ├── decisions.md
    ├── design.md
    ├── plan.md
    ├── progress.md
    ├── research.md
    ├── requirements.md
    ├── rules.md
    ├── screens.md
    ├── stack.md
    ├── workflow.md
    └── tickets/
        ├── README.md
        ├── T01-application-structure.md
        ├── T02-navigation-and-routes.md
        ├── T03-plant-data-model-and-storage.md
        ├── T04-add-plant-screen.md
        ├── T05-my-plants-screen.md
        ├── T06-plant-details-screen.md
        ├── T07-image-upload-and-inspection.md
        ├── T08-inspection-results-and-history.md
        ├── T09-ai-assistant-chat.md
        └── T10-care-actions.md
```

## Project Status Note

This repository contains the project's planning, design, requirements, and development backlog. Implementation will be documented as development tickets are completed.