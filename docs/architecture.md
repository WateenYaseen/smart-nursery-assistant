# Smart Nursery Assistant — System Architecture

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Status:** Updated proposed architecture

## 1. System Overview

Smart Nursery Assistant is planned as a responsive web application, primarily accessed through an Android smartphone browser.

The owner interacts with the application to register individual plants, submit images, receive AI-assisted assessments, access plant-care information, communicate with a conversational assistant, and manage plant records.

The architecture is divided into the following main components.

## 2. Main Components

### 2.1 User Interface
Provides the screens through which the owner can:
- View registered plants.
- Add an individual plant.
- Select a plant for inspection.
- Submit plant images.
- View assessment results and care guidance.
- Communicate with the conversational assistant in Arabic or English.
- Review plant history and record performed care actions.

The interface must communicate uncertainty and limitations clearly.

### 2.2 Image Input
Receives images submitted by the owner and associates them with the selected plant record.

The owner must select an existing plant record or create a new one before inspection.

The component must not automatically match an image to an individual plant record.

### 2.3 AI Assessment
Processes submitted images to support:
- Plant identification within supported categories.
- Assessment of supported visible plant conditions.
- Identification of possible overlapping conditions when supported.
- Qualitative watering-need assessment when sufficient information is available.

The component must communicate uncertainty and must not claim to measure actual soil moisture from an ordinary image.

### 2.4 Plant Knowledge
Provides relevant reference information, including:
- Plant-care guidance.
- Watering methods.
- Common diseases and visible symptoms.
- Available treatment guidance.

Information should be based on documented sources and should not be invented when unavailable.

### 2.5 Conversational Assistant
Allows the owner to ask plant-related questions and receive explanations and care guidance in Arabic or English.

The assistant should use relevant available context, such as:
- The selected plant's information.
- Its latest inspection results.
- Previous inspection history.
- Owner-entered care actions.
- Documented plant-care knowledge.

The assistant should distinguish between recorded facts, AI predictions, and general reference information.

It must not invent missing information, present uncertain predictions as confirmed diagnoses, or guarantee treatment outcomes.

When information is insufficient, it should communicate the limitation and may request relevant additional information or images.

### 2.6 Recommendation Component
Uses available inspection results, plant information, and history to suggest possible next actions and prioritize plants that may need attention.

It must provide reasons for recommendations when available.

It must not guarantee treatment results or mark suggested actions as completed.

### 2.7 Plant Records
Stores and retrieves:
- Individual plant records.
- Previous inspection results and associated images.
- Owner-entered care actions.
- Recommendations and their confirmation status.
- Relevant information needed to maintain each plant's history.

Information must remain associated with the correct individual plant.

## 3. Main Communication Flow

### 3.1 Plant Inspection Flow

1. The owner opens the web application.
2. The owner selects an existing plant record or creates a new one.
3. The owner submits an image for the selected plant.
4. The Image Input component associates the image with the selected record.
5. The AI Assessment component processes the image.
6. Plant Knowledge provides relevant care information.
7. The Recommendation component prepares suggested next actions when possible.
8. The interface displays the assessment, limitations, and guidance.
9. Plant Records stores the inspection and makes the plant's history available.
10. The owner can explicitly record any care action they perform.

### 3.2 Conversational Assistant Flow

1. The owner opens the assistant from the inspection results or plant details.
2. The owner asks a plant-related question in Arabic or English.
3. The system retrieves relevant information for the selected plant, when available.
4. The Conversational Assistant uses the available plant context and documented knowledge to prepare a response.
5. The interface displays the answer and communicates uncertainty or missing information when necessary.
6. The owner may continue the conversation or provide additional information.

## 4. Architecture Diagram in Words

**Inspection flow:**

Owner → Web Interface → Image Input → AI Assessment → Plant Knowledge → Recommendation → Web Interface

**Conversational flow:**

Owner → Web Interface → Conversational Assistant → Plant Records and Plant Knowledge → Conversational Assistant → Web Interface

**Plant Records** stores and retrieves individual plant information, inspection history, images, care actions, and recommendations throughout the workflow.

## 5. Constraints and Open Decisions

- The first version will be a responsive web application.
- The primary device for initial use and testing is an Android smartphone through a web browser.
- The owner manually selects the individual plant record before inspection.
- The system will use only documented supported plant and condition categories.
- Ordinary images cannot provide actual soil-moisture measurements.
- The conversational assistant must use available information and communicate uncertainty.
- IoT and sensor integration are deferred.
- The final database, image-storage method, model deployment method, conversational AI approach, and hosting platform are still undecided.