# Project Scope — Smart Nursery Assistant

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Duration:** 8 weeks  
**Team:** One student  
**Working title:** Smart Nursery Assistant  
**Status:** Proposed scope; dataset and technical feasibility not yet verified.

---

## 1. Project objective

Build a limited AI-powered prototype that helps a nursery owner identify supported plant types, assess selected visible plant conditions, and maintain separate histories for individual potted plants.

The prototype will combine:
- A model trained by the student using a prepared dataset.
- A conversational assistant.
- Persistent individual plant records.
- Cautious, evidence-based explanations and care guidance.

The project must remain achievable within eight weeks and must produce a working live demonstration.

## 2. Primary user and use case

**Primary user:** Nursery owner.

**Main use case:** The owner photographs one plant, receives an analysis, asks questions about its condition, and saves the observation to that plant's history.

The system should support future follow-up questions about the same plant without requiring the owner to explain its entire history again.

## 3. Functional requirements

### FR-01: Single-plant image input

- Accept a photograph of one plant at a time.
- Reject or request another image when the input is unsuitable.
- Avoid analyzing several plants in one photograph as if they were a single subject.

### FR-02: Trained plant-type classification

- Train a classification model using a dataset prepared by the student.
- Use only plant categories supported by the selected dataset.
- Evaluate the model on data not used for training.
- Display the predicted class and available confidence information.
- Provide an uncertain result when the prediction is not reliable enough.

Plant identification is a separate task from disease or condition classification.

### FR-03: Visible condition assessment

This feature is conditional on dataset availability.

If the dataset contains suitable, reliable labels, the project may include a model for a limited number of visible conditions.

Requirements:
- Use only supported condition classes.
- Show uncertainty when appropriate.
- Avoid claiming that a prediction is a confirmed diagnosis.
- Do not invent causes that are not supported by the available information.

If a suitable condition dataset cannot be found, this feature must be reduced or removed rather than replaced with unsupported predictions.

### FR-04: Conversational assistant

The user should be able to ask written questions about the current plant and its previous observations.

The assistant should:
- Explain classification results.
- Present possible interpretations cautiously.
- Ask for missing information.
- Give limited care guidance based on supported information.
- Avoid claiming certainty when evidence is insufficient.
- Retrieve the correct individual plant history for follow-up questions.

The assistant is not intended to be an unrestricted agricultural chatbot. Its responses should be grounded in the model outputs, stored observations, and a reviewed knowledge source or predefined guidance.

### FR-05: Individual plant records

Each tracked pot must have its own record.

A record may contain:
- Automatically generated plant ID.
- Predicted plant type.
- Initial registration date.
- Photographs or image references.
- Analysis results.
- User-provided observations.
- Follow-up answers.
- Dates of previous observations.
- Previous guidance and actions recorded by the user.

Two pots of the same plant type must have separate records.

### FR-06: Automatic record creation and retrieval

- Generate an ID automatically when a new plant record is created.
- Do not require the owner to manually enter an ID every time.
- Allow the system to retrieve an existing record when the same plant is photographed again.
- Keep the histories of different pots separate.

**Important technical limitation:** Recognizing an individual pot from a new photograph is not the same as recognizing its plant species. It may require image similarity or another matching approach and can fail when the angle, lighting, background, or plant appearance changes.

Therefore:
- Automatic matching must be tested before it is treated as reliable.
- If matching is uncertain, ask the user to confirm the suggested record or create a new one.
- Do not silently attach an observation to the wrong plant.

### FR-07: Persistent memory

The system should retain plant records between sessions and retrieve them in later conversations.

This requires a database or another persistent storage mechanism connected to the application.

The conversational model's temporary context alone is not sufficient.

### FR-08: Watering and care guidance

Watering guidance is an exploratory feature, not a guaranteed image-classification result.

The system may:
- Identify visible signs that could be related to watering.
- Ask questions about the soil, recent watering, and other relevant observations.
- Present possible explanations.
- Recommend checking the plant before watering or applying treatment.

The system must not:
- Claim to measure soil moisture from a photograph.
- Give an exact watering quantity based only on an image.
- Treat wilting or yellowing as proof of a single cause.
- Recommend unnecessary vitamins, fertilizers, or treatments as if they were required.

If the evidence is insufficient, the correct response is to explain the uncertainty and ask for more information.

---

## 4. Proposed technical structure

The project is expected to contain the following logical components:

1. **Image input:** receives and validates the plant photograph.
2. **Plant identification model:** predicts a supported plant type.
3. **Condition model:** optionally classifies supported visible conditions if the dataset allows.
4. **Assistant layer:** handles user questions, explanations, and clarification.
5. **Plant record manager:** creates, retrieves, and updates individual plant histories.
6. **Persistent storage:** stores plant records and observation history.
7. **Care guidance layer:** provides limited, reviewed guidance and uncertainty messages.

The models and the assistant should not be treated as one undifferentiated AI component. Each task needs its own evaluation and limitations.

## 5. Dataset and model requirements

### 5.1 Dataset source

Planned source: **Kaggle**.

No specific dataset has been selected.

Before committing to a dataset, inspect:
- Dataset licence and permitted use.
- Plant categories and condition labels.
- Number of images in each class.
- Class imbalance.
- Image resolution and quality.
- Duplicate or near-duplicate images.
- Label reliability.
- Differences between dataset images and actual nursery photographs.

### 5.2 Model tasks

The initial model task is plant-type classification.

Condition or disease classification is a separate proposed task and will only be included if a suitable dataset is available and the timeline permits.

Watering need assessment is not assumed to be a reliable image-only classification task.

### 5.3 Training and evaluation

The student must:
- Prepare and inspect the dataset.
- Define the supported classes.
- Create training, validation, and test sets.
- Prevent duplicate or near-duplicate images from leaking across splits.
- Train the model.
- Evaluate it on held-out data.
- Report per-class performance and confusion between classes.
- Test it on images that differ from the training examples.

A high test score on a public dataset does not automatically prove that the model will work reliably in the actual nursery.

### 5.4 Model selection

The model architecture will be selected after dataset inspection.

A lightweight image-classification approach or transfer learning may be considered, depending on available tools and computing resources.

No guaranteed GPU or paid training service should be assumed.

---

## 6. Non-functional requirements

### Usability
- Simple smartphone-friendly interface.
- Short, understandable results.
- Minimal manual entry.
- Clear follow-up questions.

### Reliability
- Do not present uncertain predictions as confirmed facts.
- Do not silently mix the histories of different pots.
- Handle missing or invalid images.
- Preserve previously saved records.

### Transparency
- Distinguish model predictions from user observations.
- Display uncertainty where appropriate.
- Explain the limits of image-based analysis.

### Privacy
- Avoid collecting unnecessary personal information.
- Store only the data required for the plant records.
- Do not upload private nursery images to external services without understanding the service's data handling and obtaining appropriate permission.

---

## 7. Must-have features vs. optional features

| Feature | Priority | Decision |
|---|---|---|
| One plant per image | Must-have | Include |
| Trained plant-type classifier | Must-have | Include |
| Model evaluation | Must-have | Include |
| Written assistant | Must-have | Include |
| Individual plant records | Must-have | Include |
| Automatically generated IDs | Must-have | Include |
| Persistent history | Must-have | Include |
| Follow-up questions | Must-have | Include |
| Separate histories for same-type pots | Must-have | Include |
| Condition/disease classification | Conditional | Include only if data supports it |
| Automatic matching of individual pots | Conditional | Test; confirmation fallback |
| Watering guidance | Limited / exploratory | No image-only guarantees |
| Advanced visual dashboards | Optional | Exclude initially |
| Voice interaction | Optional | Exclude |
| Arabic voice recognition | Optional | Exclude |
| Multiple users and staff accounts | Optional | Exclude |
| Mobile application deployment | Optional | A simple web prototype is sufficient |

---

## 8. Out of scope

The following features are excluded from the eight-week project:

- Monitoring the nursery continuously.
- Integration with the existing nursery camera.
- IoT sensors or new hardware.
- Automatic irrigation or water control.
- Measuring soil moisture from photographs.
- Guaranteed disease diagnosis.
- Identification of every plant species.
- Detection of every plant disease.
- Guaranteed prediction of plant survival or recovery.
- Automatic treatment or fertilizer application.
- Replacing agricultural specialists.
- Worker management or attendance tracking.
- Nursery inventory management.
- Sales, accounting, and financial management.
- Automated purchasing of agricultural supplies.
- Notifications and complex scheduling systems.
- A full commercial nursery-management platform.

These features may be considered in a future version, but they are not commitments for this mentorship project.

---

## 9. Main risks and mitigation

### Risk 1: Dataset does not match the nursery

**Why it matters:** A model trained on clean, controlled images may perform poorly on photographs taken in the nursery.

**Mitigation:**
- Inspect the dataset before choosing the model.
- Test with different backgrounds and lighting.
- Use separate real-world test images where available.
- Limit the supported classes.

### Risk 2: Plant type and disease classification are confused

**Why it matters:** Identifying a plant species does not establish whether it is diseased.

**Mitigation:**
- Treat the tasks separately.
- Use suitable labels for each task.
- Evaluate each model independently.
- Remove condition classification if suitable data is unavailable.

### Risk 3: Incorrect individual plant matching

**Why it matters:** Two pots may contain the same plant type, and photographs may look similar.

**Mitigation:**
- Keep individual records separate.
- Test automatic matching.
- Ask for confirmation when confidence is insufficient.
- Never silently merge different plant histories.

### Risk 4: Persistent storage is more complicated than expected

**Why it matters:** The assistant must retrieve old observations correctly, even after a new session.

**Mitigation:**
- Start with a simple structured database.
- Define the plant record schema early.
- Test creating, retrieving, and updating records independently of the AI model.

### Risk 5: Unsupported care recommendations

**Why it matters:** Incorrect watering or treatment advice could harm a plant.

**Mitigation:**
- Use reviewed guidance.
- Ask for missing context.
- Express uncertainty.
- Avoid exact watering or treatment instructions without sufficient evidence.

### Risk 6: Time limitations

**Why it matters:** Dataset preparation, model training, assistant integration, and record management are separate tasks.

**Mitigation:**
- Build a small working vertical slice first.
- Limit the number of plant classes.
- Prioritize the trained classifier and persistent plant records.
- Remove optional condition classification or automatic matching if they threaten completion.

---

## 10. Success criteria

The project will be considered successful as a limited prototype if it can demonstrate:

1. A trained model predicting plant types within its supported classes, with evaluation results reported honestly.
2. A user photographing one plant and receiving an understandable result.
3. A conversational assistant explaining the result and asking for missing information rather than guessing.
4. A separate record being created for each tracked pot, including two pots of the same plant type.
5. A saved plant history being retrieved in a later session and updated with a new observation.

If condition classification is included, it must also have its own held-out evaluation.

If automatic plant matching is not reliable, the demonstration must show the confirmation fallback rather than pretending that matching works.

---

## 11. Minimum viable demonstration

If time becomes limited, the smallest useful version should contain:

- A small set of plant classes supported by the selected dataset.
- One trained image-classification model.
- One-plant image input.
- A simple written assistant that explains the prediction.
- Automatic creation of an individual plant record.
- Persistent storage and retrieval of that record.
- A second observation added to the same record through a confirmation step.

Condition classification, advanced watering guidance, and fully automatic plant matching can be removed without making the minimum demonstration meaningless.

The project must still include a model trained by the student. A ready-made chatbot alone does not satisfy the project requirement.

---

## 12. Project status and assumptions

| Item | Status |
|---|---|
| Agriculture selected as project direction | Decided |
| Primary user identified | Decided |
| Nursery workflow discussed | Initial information collected |
| One plant per image | Decided |
| Individual histories | Decided |
| Automatic ID generation | Decided |
| Persistent history | Required |
| Kaggle as planned dataset source | Decided |
| Specific dataset | Not selected |
| Plant classes | Not finalized |
| Condition classes | Not finalized |
| Model architecture | Not selected |
| Model training | Not done |
| Model evaluation | Not done |
| Database design | Not implemented |
| Automatic plant matching | Not tested |
| Watering assessment | Not validated |
| Father testing the prototype | Not done |
| Live demonstration | Not built |

### Confirmed project constraints

- Eight-week mentorship project.
- One student working independently.
- Approximately 3–8 hours between weekly mentorship sessions.
- One AI subscription may be used.
- No additional paid services assumed.
- No guaranteed GPU.
- No new hardware or sensors.
- A working live demonstration is required.
- A model trained by the student is a core requirement.

### Important assumptions

- Suitable public datasets may be available on Kaggle.
- The selected data may support a limited number of plant classes.
- The assistant can be connected to persistent storage within the time limit.
- A simple confirmation workflow can handle uncertain plant matching.
- The father will be able to test the prototype once it demonstrates sufficient reliability.

These assumptions still require testing.

---

## 13. Scope reduction rules

Reduce the project scope if:

- No suitable dataset supports the intended plant categories: reduce the number of categories or reconsider the model task.
- Condition labels are unavailable or unreliable: remove disease/condition classification.
- Dataset preparation takes too long: use a smaller, carefully selected subset while preserving a valid evaluation split.
- Automatic plant matching is unreliable: use suggested records with user confirmation.
- Persistent cross-session retrieval takes too long: prioritize a simple database and basic create/read/update operations.
- Watering guidance cannot be supported safely: retain only general observations and clarification questions.
- The conversational assistant becomes too complex: use a limited set of supported question types and grounded responses.
- Core features are not working reliably: remove optional interface improvements and advanced features.

Do not remove the trained model requirement. Reduce its class count or complexity instead.

---

## 14. Next step

**Dataset discovery and inspection.**

Before implementation:
1. Search Kaggle for plant identification datasets.
2. Search separately for plant disease or condition datasets.
3. Inspect their classes, sample counts, image quality, and licences.
4. Check for duplicates and class imbalance.
5. Compare the data with the nursery's actual plant types and image conditions.
6. Decide which model task is realistic.
7. Freeze the smallest supported set of classes.

Only after this review should the final model design and implementation plan be decided.