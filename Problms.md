# Problem Discovery and Selection

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Current project direction:** Agriculture / Nursery Management  
**Status:** Agriculture selected as the current project direction. This decision replaces CoursePath as the active project, but does not erase the earlier project history.

---

## 1. Purpose of this document

This document records the problems considered during project discovery and explains why agriculture was selected as the current direction.

The project went through two selection periods:

- **Historical selection:** Academic Planning, Student Transportation, and Heart Care were explored in V1–V3, leading to CoursePath.
- **Current selection:** Agriculture, University Academic Planning, and Heart Care were reconsidered, leading to the Smart Nursery Assistant.

The historical decision to select CoursePath remains part of the project record. The current decision is a later change based on a different real-world problem and a more accessible project context.

## 2. Evidence labels

- **[Firsthand]:** I experienced the situation or directly participated in it.
- **[Observed]:** I saw or heard about it, but have not independently verified it.
- **[Assumption]:** My interpretation or belief without sufficient evidence.
- **[Unknown]:** Information that has not yet been established.

These labels distinguish actual experience from assumptions and proposed ideas.

---

# Part A — Historical Problem Selection

## 3. Original candidates from V1

### Candidate 1: Academic Planning

**Target users:** TTU students whose academic progress depends on courses being offered and available for registration.

**Problem identified:**

A student may be unable to register for an important course because it is not offered or a section is cancelled. If that course is a prerequisite for later courses, the student may have difficulty finding alternatives that fit their study plan.

**Evidence:**
- [Firsthand] I experienced a Data Mining section cancellation. I contacted the university and travelled from Salt to Tafila, but did not find a solution.
- [Firsthand] I registered for fewer credit hours because the available alternatives did not move me forward in my study plan.
- [Firsthand] A small group of affected students collected names and approached the university together.
- [Observed] I noticed similar complaints from Cybersecurity students and other students regarding course offerings.
- [Unknown] How widespread the problem is across TTU and how the university decides which courses to offer or cancel.

**Current workaround:**
Students check the semester offering list, try to register quickly, contact university offices, and sometimes seek a "no objection" approval when a section is full.

**Main limitation:**
A planning tool can help students understand the courses actually offered and the consequences of missing prerequisites. It cannot control university decisions or prevent course cancellations.

### Candidate 2: Student Transportation

**Target users:** Students travelling from areas with limited direct transportation to TTU.

**Problem identified:**

Travelling from Salt to TTU can require multiple transport connections, significant time, and at least 10 JOD according to my described trip. Direct transportation options are limited and depend on departure locations, schedules, and passenger availability.

**Evidence:**
- [Firsthand] I described my own Salt-to-Tafila route, its connections, approximate duration, and cost.
- [Observed] I noticed transportation difficulties among students from my area.
- [Assumption] Students from other governorates may experience similar difficulties.
- [Unknown] The number of affected students, how frequently they travel, and whether the same problem exists across other routes.

**Current workaround:**
Using multiple public transport connections or arranging an external bus from a gathering point.

**Main limitation:**
A software solution can help organize available information, but it cannot create additional buses or guarantee transport availability. A matching or ride-sharing system would also depend on having enough active users.

### Candidate 3: Heart Care

**Target users:** Not yet defined. Potentially people with weakened heart muscles or their caregivers.

**Problem identified:**

The idea was motivated by a personal family experience involving a heart attack and a weakened heart muscle. However, the specific day-to-day problem that an AI project should address was not identified.

**Evidence:**
- [Firsthand] Personal motivation to explore ways technology could support people dealing with heart-related conditions.
- [Unknown] The actual daily difficulties, target user, current coping methods, and needs of patients or caregivers.

**Main limitation:**
The problem requires further discovery and access to appropriate users or professionals. It also carries medical safety risks. A student project must not diagnose, interpret symptoms as a medical conclusion, or replace professional care.

---

# Part B — Current Project Reconsideration

## 4. Current candidates

The three candidates reconsidered for the current project direction are:

1. Agriculture / Nursery Management.
2. University Academic Planning (CoursePath).
3. Heart Care.

Student Transportation remains documented in the historical V1–V3 records, but it is not part of this current three-candidate comparison.

### Candidate 1: Agriculture / Nursery Management

**Target user:** My father, who manages a medium-sized plant nursery.

**Problem identified:**

Managing the nursery involves inspecting plants, identifying problems, deciding what care each plant needs, watering, treating, cleaning, arranging, moving pots, and monitoring the work.

Some decisions require identifying the condition of an individual plant and deciding whether it needs water or another form of care. These decisions can be difficult when the owner is not present or when an experienced agricultural specialist is unavailable.

**Evidence:**
- [Firsthand] I am familiar with the nursery and my father's work and have discussed the tasks and difficulties with him.
- [Observed] The nursery contains one greenhouse and potted plants around it. A worker may sometimes be present, but does not have the same agricultural experience as my father.
- [Observed] My father may rely on his experience, seek advice, use videos, or apply treatments when trying to address plant problems.
- [Observed] He may water the nursery as a whole rather than assess every individual pot's watering needs.
- [Unknown] How frequently each problem occurs, how many plants are affected, and whether the current practices cause measurable losses or unnecessary resource use.

**Current workflow and workarounds:**
- Inspect plants when visiting the nursery.
- Use personal experience to assess visible problems.
- Ask another person for advice when needed, if available.
- Search for information or videos about a plant.
- Apply treatments or nutrients based on the available judgement.
- Water the nursery, sometimes without assessing every pot individually.
- Give instructions to the worker when the owner is absent.

**Why the current workflow may be insufficient:**
- Inspecting and caring for individual plants takes time.
- The worker may not have enough experience to make independent decisions.
- Expert advice may not always be available.
- A visible symptom may have more than one possible cause.
- A plant may receive water or treatment that it does not actually need.

These are identified concerns, not measured outcomes. No financial losses, disease spread, or water waste have been quantified.

**Potential AI contribution:**
- Identify a plant type from an image, if the selected dataset supports it.
- Classify certain visible plant conditions or diseases, if suitable labelled data is available.
- Help interpret observations and provide cautious care guidance.
- Maintain a separate history for each tracked plant.
- Support follow-up questions about previously recorded plants.

**Important limitations:**
A photograph cannot reliably measure soil moisture or confirm every disease. Watering guidance must be cautious and may require additional information. Automatic recognition of the same individual pot across different photographs is also a technical challenge.

### Candidate 2: University Academic Planning

**Target users:** TTU AI & Data Science students.

**Problem identified:**

Students may struggle to plan registration when important courses are unavailable, particularly when those courses are prerequisites for later courses.

**Evidence:**
- [Firsthand] My own Data Mining registration experience and the impact on my course load.
- [Firsthand] A small group of students approached the university about the issue.
- [Observed] Similar complaints from students in other majors.
- [Unknown] Wider prevalence, official data accessibility, and whether the prototype could represent all relevant university rules.

**Potential AI contribution:**
A trained intent-classification model could recognize student questions and connect them to a deterministic course-planning engine.

**Why it is no longer the selected direction:**
CoursePath was previously selected and developed through V1–V6. However, the current project reconsideration identified a different accessible real-world workflow in the family nursery. University planning also depends on accurate academic data and university-specific rules that still require verification.

The earlier work remains valid historical project work, but CoursePath is no longer the active project direction.

### Candidate 3: Heart Care

**Potential target users:** People with weakened heart muscles or their caregivers. The exact user remains undefined.

**Problem identified:**

The idea has personal motivation, but a specific and validated daily problem has not yet been established.

**Evidence:**
- [Firsthand] Personal motivation.
- [Unknown] Specific user needs, access to participants, suitable data, and a safe project boundary.

**Potential AI contribution:**
Could only be determined after identifying a real user problem and consulting appropriate healthcare knowledge and professionals.

**Why it is no longer the selected direction:**
The problem remains insufficiently defined for an eight-week solo project. It also requires stronger safety controls and access to relevant users or professionals. Agriculture currently offers a more accessible workflow for building and testing a limited prototype.

---

## 5. Comparison of the current candidates

The following ratings are qualitative project-planning judgments, not measured results.

| Criterion | Agriculture | University | Heart Care |
|---|---|---|---|
| Problem clarity | Relatively clear workflow | Clear from earlier experience | Not yet clear |
| Access to primary user | Father is accessible | Students are accessible | Not established |
| Evidence | Direct familiarity with nursery work; details need further validation | Firsthand experience and small group | Personal motivation only |
| Data availability | Public datasets may be available; suitability unknown | Study plan and offering data still need verification | Suitable data and access unknown |
| Eight-week feasibility | Possible with a narrow image-based scope | Previously assessed as possible with reductions | Uncertain |
| Live demo potential | Image analysis, assistant, and plant records | Course eligibility and intent classification | Depends on a yet-undefined problem |
| AI contribution | Image classification and conversational assistance | Intent classification | Not yet established |
| Main risk | Dataset suitability and reliable plant identification | University data and complex rules | Medical safety and unclear user need |

## 6. Final selection

**Selected current direction: Agriculture / Smart Nursery Assistant.**

Agriculture was selected because:

1. It is connected to a real nursery and an existing workflow that I can observe and understand.
2. The primary user, my father, is accessible for discussing requirements and reviewing the prototype.
3. The project can be narrowed to individual plant analysis, a trained image model, and a simple assistant.
4. Public datasets, particularly from Kaggle, are a possible starting point for training. Their suitability has not yet been verified.
5. The project can potentially produce a visible live demonstration within eight weeks if the scope is controlled.

My father is willing to try the system once it demonstrates that it works reliably. This is a conditional willingness to test, not proof that the prototype has already been validated.

## 7. Why the other candidates were not selected

**University Academic Planning:**

CoursePath was a reasonable project based on firsthand experience and a clearly identified student problem. However, it depends on accurate study-plan and course-offering data and university-specific rules. Agriculture offers a more directly accessible workflow for the current project, so CoursePath is no longer the active direction.

**Heart Care:**

The idea has personal importance, but the actual daily problem and target user have not been sufficiently defined. It also has higher safety requirements and would need access to appropriate patients, caregivers, or healthcare professionals.

## 8. Remaining unknowns

### Agriculture
- Which Kaggle datasets are suitable and what are their licences?
- Which plant types are represented?
- Do the datasets contain reliable plant-condition or disease labels?
- Can plant identification and condition classification be handled within the same project, or should they be separate tasks?
- How well do the images represent the lighting, backgrounds, pots, and camera conditions in the actual nursery?
- What additional information is needed to give cautious watering guidance?
- Can the system reliably distinguish individual pots across different visits?
- What is the simplest persistent record structure?
- What level of reliability would make the father comfortable testing it?

### University
- The study plan and offering data have not been fully verified.
- Student check-ins were not completed.
- The CoursePath model and dataset were not completed as part of the earlier project.

### Heart Care
- Target user, daily problem, validation participants, and safe scope remain undefined.

## 9. Current decision status

- **Current selected project:** Agriculture / Smart Nursery Assistant.
- **Previous project:** CoursePath, preserved as historical work.
- **Dataset source:** Kaggle is the planned source; no dataset has been selected yet.
- **Model training:** Required as part of the project direction; not yet performed.
- **Prototype:** Not yet implemented.
- **User testing:** Not yet performed.
- **Commercial validation:** Not performed.

The selection is a project-direction decision, not evidence that the proposed system already works or that its benefits have been measured.
