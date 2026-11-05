# Smart Nursery Assistant — System Architecture

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Status:** Proposed architecture

## 1. System Overview

Smart Nursery Assistant is planned as a responsive web application. The owner interacts with the application through a user interface, submits plant images, receives AI-assisted assessments, and accesses plant records and care recommendations.

The architecture is divided into the following main components.

## 2. Main Components

### 2.1 User Interface
Provides the screens through which the owner can:
- View registered plants.
- Add an individual plant.
- Select a plant for inspection.
- Submit plant images.
- View assessment results and care guidance.
- Review plant history and record performed care actions.

The interface must communicate uncertainty and limitations clearly.

### 2.2 Image Input
Receives images submitted by the owner and associates them with the selected plant record.

It must not automatically identify which individual plant was photographed.

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

### 2.5 Recommendation Component
Uses available inspection results, plant information, and history to suggest possible next actions and prioritize plants that may need attention.

It must not guarantee treatment results or mark suggested actions as completed.

### 2.6 Plant Records
Stores and retrieves:
- Individual plant records.
- Previous inspection results and associated images.
- Owner-entered care actions.
- Recommendations and their confirmation status.

Information must remain associated with the correct individual plant.

## 3. Main Communication Flow

1. The owner opens the web application.
2. The owner selects an existing plant record or creates a new one.
3. The owner submits an image for that selected plant.
4. The Image Input component associates the image with the selected record.
5. The AI Assessment component processes the image.
6. Plant Knowledge provides relevant care information.
7. The Recommendation component prepares suggested next actions when possible.
8. The interface displays the assessment, limitations, and guidance.
9. Plant Records stores the inspection and retrieves the plant's previous history when needed.
10. The owner can explicitly record any care action they perform.

## 4. Constraints and Open Decisions

- The first version will be a responsive web application.
- The system will use only documented supported plant and condition categories.
- Individual plant selection is performed by the owner.
- Ordinary images cannot provide actual soil-moisture measurements.
- IoT and sensor integration are deferred.
- The final database, image-storage method, model deployment method, and hosting approach are still undecided.

## 5. Architecture Diagram in Words

**Owner → Web Interface → Image Input → AI Assessment → Plant Knowledge → Recommendation → Web Interface**

**Plant Records** stores and retrieves plant information, inspection history, images, care actions, and recommendations throughout the workflow.