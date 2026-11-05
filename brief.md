# Smart Nursery Assistant

## Business Requirements Document (BRD)

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Project Status:** Week 2 — Planning and documentation. No trained model or implemented application yet.

---

## 1. The Problem

Managing a nursery requires continuous attention to individual plants. Nursery owners need to inspect plants, identify possible problems, decide whether treatment or watering is needed, and monitor changes over time.

These tasks can take significant time, especially when the owner manages many plants. Identifying an unfamiliar plant or understanding the reason behind visible changes may require searching websites, watching YouTube videos, consulting other people, or relying on personal experience.

These methods are not always convenient or reliable. An expert may not be available when needed, online information may not match the plant's actual condition, and an incorrect decision may lead to unnecessary treatment, watering, or further damage.

The proposed **Smart Nursery Assistant** aims to provide an AI-based system that helps nursery owners identify plants, assess supported visible plant conditions from images, access relevant care information, and maintain records for individual plants.

The system is intended to support decision-making, not replace agricultural experts or guarantee that every plant problem can be identified.

## 2. Who Has This Problem?

### Primary user

The primary user for the initial version is the owner's father, who manages a medium-sized family nursery in Jordan. The nursery includes one greenhouse and plants kept in pots around it.

His responsibilities include:

- Inspecting plants and checking their condition.
- Identifying possible plant problems.
- Deciding whether plants need watering or treatment.
- Cleaning, arranging, and moving plants.
- Following up on plants over time.
- Supervising a worker who may assist with nursery tasks.

He usually spends a long time at the nursery, often from the morning, but his visits are not necessarily at the same time every day. Sometimes he may be unable to visit.

He can use an Android smartphone and take photos of plants.

### Secondary users

The broader intended audience may include:

- Small nursery owners.
- Individual farmers.
- Small agricultural businesses.
- Early-stage agricultural entrepreneurs.

However, the initial prototype will focus on the primary user's needs rather than attempting to support every type of agricultural operation.

## 3. Today, Without It

Currently, the primary user relies mainly on personal experience, online searches, videos, and asking other people for advice.

When he encounters an unfamiliar plant or a possible problem, he may:

- Search for information on websites.
- Watch YouTube videos about the plant.
- Ask someone with agricultural knowledge, when available.
- Make decisions based on his own experience.
- Use treatments or vitamins that may not be necessary.
- Water plants based on an assumption that they lack water.

He has also tried a plant-care application in the past but found that it did not meet his needs and deleted it. He could not recall its name.

These approaches can make plant-care decisions time-consuming and may not always provide information relevant to the specific plant.

The proposed system aims to reduce the time spent searching for plant-care information by allowing users to ask questions and receive guidance through one assistant.

## 4. What Success Looks Like

The initial prototype will be considered useful if it can demonstrate the following capabilities:

1. **Plant identification:** Identify supported plant types from uploaded images and provide the available plant information.

2. **Visible condition assessment:** Recognize selected visible plant conditions or symptoms when they are supported by the available training data.

3. **Care guidance:** Provide relevant, cautious care information based on the identified plant and supported condition. The assistant should ask follow-up questions when the available image or information is insufficient.

4. **Individual plant records:** Automatically generate a unique identifier for each registered plant and maintain a separate record for each individual plant, even when multiple plants belong to the same species.

5. **Plant history:** Preserve previous records and observations so the user can follow changes in an individual plant over time.

6. **Photo matching:** Attempt to match a new photo to an existing plant record. When the system is uncertain, it should ask the user to confirm the match rather than automatically assigning the photo.

7. **Conversational interaction:** Allow users to ask questions and interact with the assistant in Arabic, with English as a secondary language.

### Evaluation

The prototype will be evaluated using:

- Separate training and testing data.
- Unseen images that were not used during model training.
- Local nursery images reserved for independent evaluation.
- Appropriate evaluation metrics for plant identification and condition assessment as separate tasks.
- Practical tests of individual plant records and photo-matching confirmation.
- A comparison of the time needed to find relevant plant-care information using the user's current approach and the proposed assistant.
- Task-completion observations to assess whether users can obtain and understand the information they need.

No specific accuracy percentage or time-saving result is assumed before testing.

## 5. Scope

### In Scope — Initial Version

The initial prototype is expected to include:

- An Android-focused application interface.
- Arabic as the primary language and English as a secondary language.
- Image-based identification for a limited set of plant types supported by available data.
- Image-based assessment of selected visible plant conditions supported by available data.
- An intelligent assistant that provides cautious plant-care information.
- Follow-up questions when additional information is needed.
- Automatic generation of unique IDs for individual plants.
- Separate records for individual plants, including plants of the same species.
- Persistent plant records and observation history.
- Photo matching with user confirmation when the match is uncertain.

### Out of Scope — Initial Version

The following features are not part of the initial prototype:

- Identifying every plant species.
- Detecting every plant disease or possible condition.
- Guaranteed disease diagnosis or treatment recommendations.
- Measuring soil moisture or other environmental conditions from an ordinary photo.
- Automatic irrigation or direct control of watering systems.
- IoT devices, sensors, or additional hardware.
- Camera integration or continuous monitoring.
- Employee and worker management.
- Inventory, sales, accounting, or financial management.
- Guaranteed identification of the same individual plant across all photos.
- Supporting large commercial agricultural operations with complex management requirements.

### Technical and Project Constraints

- The project will be developed individually.
- The implementation period is eight weeks.
- Available working time is approximately 3–8 hours per week.
- The project should not require additional paid services or equipment.
- Public datasets, including possible Kaggle datasets, will be investigated as potential data sources.
- Dataset selection will depend on image quality, labels, licensing, class coverage, and relevance to the intended plants and conditions.
- Jordanian agricultural relevance will be prioritized where suitable data is available.
- Local nursery images may be collected for evaluation when possible.
- Training, validation, and testing data must be separated appropriately. Images reserved for independent local evaluation must not be used for model training or tuning.
- If suitable data is unavailable for some plant types or conditions, those categories will be excluded from the initial version and considered for future development.

## 6. Risks and Unknowns

Several issues must be investigated before the system can be considered reliable:

### Dataset Availability and Quality

Suitable public datasets may not cover the plants commonly found in Jordanian nurseries. Some datasets may also contain limited images, inaccurate labels, class imbalance, or licensing restrictions.

**Mitigation:** Investigate multiple datasets before selecting the supported plant types and condition categories. Prioritize data quality and relevance over the number of supported categories.

### Model Reliability

A plant may look different depending on lighting, camera quality, growth stage, or environmental conditions. Similar symptoms may also have different causes.

**Mitigation:** Evaluate plant identification and condition assessment separately, use unseen images, and avoid presenting uncertain predictions as confirmed results.

### Care Information Reliability

Incorrect care guidance may cause unnecessary watering, treatment, or damage to plants. An ordinary image cannot reliably reveal every factor affecting a plant, such as actual soil moisture.

**Mitigation:** Provide cautious guidance, ask follow-up questions when necessary, explain limitations, and avoid unsupported treatment recommendations.

### Individual Plant Recognition

Matching photos of the same plant across different occasions may be difficult because its appearance changes over time or because photos are taken from different angles.

**Mitigation:** Use automatically generated plant IDs and ask the user to confirm uncertain photo matches.

### Project Time and Scope

Developing plant identification, condition assessment, conversational guidance, and persistent records within eight weeks may be challenging.

**Mitigation:** Prioritize a reliable prototype with a limited number of supported plant types and conditions. Additional features will only be considered if time and data availability allow.

### Practical Usefulness

It is not yet confirmed whether the proposed system will save enough time or provide sufficiently useful guidance for nursery owners.

**Mitigation:** Compare the time required to find plant-care information using the current approach with the time required using the prototype. Observe task completion and collect feedback during practical testing.

---

**Current Decision:** Proceed with a limited-scope prototype, subject to dataset suitability, model evaluation, and practical usefulness. The supported plant types and condition categories will be finalized after dataset research.

**Document Note:** This BRD reflects the project owner's current requirements and the outcomes of a simulated critical review. It does not represent external manager approval, completed user testing, or verified model performance.