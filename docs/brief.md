# Smart Nursery Assistant
## Business Requirements Document (BRD)

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Project Stage:** Planning and Documentation  
**Document Status:** Updated after Task 03 Fresh-Chat Test

## 1. Project Overview

Smart Nursery Assistant is an AI-assisted, responsive web application designed to help nursery owners inspect, understand, and manage individual plants.

The application combines image-based plant identification, visible condition assessment, plant-care information, a conversational assistant, individual plant records, and recommendations.

The primary device for the initial version is an Android smartphone, accessed through a web browser. The project is not a native Android application.

The first version will focus on a real nursery workflow and support only plant types and conditions that can be reasonably supported by available data and evaluation.

## 2. The Problem

Managing a nursery requires continuous attention to individual plants. The owner needs to inspect plants, recognize possible problems, decide whether watering or treatment may be needed, and follow up on their condition.

These tasks can take time, especially when the owner cannot visit the nursery every day or needs information about a plant problem that is not immediately clear.

Relying only on personal experience or searching for information separately may make it difficult to identify a problem or choose an appropriate next step.

The project aims to provide one accessible assistant that helps the owner inspect plants, understand possible problems, access relevant care guidance, and maintain individual plant histories.

## 3. Target Users

### Primary User

The primary user is the owner of a family nursery in Jordan.

The nursery includes a greenhouse and plants kept in individual pots. The owner is responsible for plant inspection, watering, treatment, cleaning, arranging plants, and following up on their condition. A worker may assist with nursery tasks.

The owner uses an Android smartphone and can take pictures of plants. However, the time and frequency of nursery visits may vary.

The application should therefore be simple to use through a mobile browser and should support the owner's practical daily workflow.

### Potential Future Users

The project may later be useful for:
- Other small nursery owners.
- Individual farmers.
- Small agricultural businesses.

These are potential future users, not the primary target of the first version.

## 4. Proposed Solution

The application will provide the following capabilities.

### 4.1 Plant Identification

The owner selects an individual plant record and submits an image.

The system identifies the plant's common name when it belongs to a supported category and provides confidence information when available.

The first version does not require the full botanical name.

### 4.2 Plant Condition Assessment

The system analyzes visible signs in the submitted image and identifies possible supported diseases or plant problems.

It may show more than one possible condition when symptoms overlap. It should explain the visible symptoms supporting each possibility when reliable information is available.

The system must communicate uncertainty and must not present an AI prediction as a guaranteed diagnosis.

### 4.3 Plant-Care Information

The system provides relevant information about the identified plant, including:
- Common name.
- Watering method.
- General care instructions.
- Common diseases and visible symptoms.
- Available treatment guidance.

Information must be based on available and documented knowledge.

### 4.4 Conversational Plant-Care Assistant

The owner can communicate with the assistant in Arabic or English and ask relevant questions about a selected plant.

The assistant should use the plant's available identification, inspection results, history, and documented care information to provide relevant explanations and guidance.

Examples of possible questions include:
- What could be causing these symptoms?
- How should I care for this plant?
- How should I apply the suggested treatment?
- What should I check next?

The assistant must not invent missing information, guarantee a diagnosis, or provide unsupported treatment claims.

### 4.5 Water-Need Assessment

The system may provide a qualitative indication of possible watering needs when visible signs and available information support an assessment.

An ordinary image cannot provide an actual soil-moisture measurement. Sensor-based measurements and quantitative watering calculations are outside the first version.

### 4.6 Individual Plant Records

Every individual plant must have a separate record, even if multiple plants belong to the same type.

The owner selects an existing plant record before an inspection or creates a new record.

The system stores previous inspection results and associated images, as well as care actions explicitly entered or confirmed by the owner.

Automatic matching of an image to an individual plant is not included in the first version.

### 4.7 Recommendations and Follow-up

The system suggests possible next actions based on available inspection results, plant information, and history.

It may prioritize plants that need attention and explain the reason for each recommendation.

Suggested actions must remain separate from actions actually performed by the owner.

## 5. First-Version Scope

### Included

- Responsive web application.
- Mobile-browser use, primarily on an Android smartphone.
- Individual plant registration and selection.
- Image-based identification of supported plant types.
- Assessment of supported visible plant conditions.
- Multiple possible conditions when supported by the evidence.
- Confidence and uncertainty information when available.
- Plant-care and treatment guidance.
- Conversational assistant in Arabic and English.
- Qualitative watering-need guidance.
- Individual plant records and inspection history.
- Owner-entered care-action logs.
- Suggested next actions and follow-up prioritization.

### Excluded or Deferred

- Native Android application.
- Automatic matching of images to individual plant records.
- Recognition of every plant species or disease.
- Guaranteed disease diagnosis or treatment outcomes.
- Disease severity percentages or scoring.
- Actual soil-moisture measurement from ordinary images.
- Quantitative watering measurements.
- IoT sensors and automatic irrigation.
- Continuous camera monitoring.
- Employee management, inventory management, sales, and accounting.
- Complex commercial farm-management features.

## 6. Constraints and Success Considerations

The project is an individual eight-week mentorship prototype, with approximately 3–8 working hours per week.

The first version must remain limited to a realistic set of plant types and conditions supported by suitable data and evaluation.

Public datasets may be investigated as potential sources, but their labels, image quality, licensing, coverage, and suitability must be checked before selection.

The system's performance must be evaluated rather than assumed. Local nursery images may be reserved for independent evaluation.

The prototype should demonstrate a practical workflow: registering an individual plant, inspecting it, receiving an assessment and care guidance, communicating with the assistant, recording performed care, and reviewing the plant's history.

The project is considered useful when it helps the owner access relevant plant information more easily, understand possible problems, and organize follow-up actions.