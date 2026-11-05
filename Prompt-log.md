# Prompt Log — IEEE WIE JS Mentorship Program 2026

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Student:** Wateen Yaseen Mousa Albalawneh  
**Project status:** Pivoted from CoursePath (Academic Planning) to an AI-Powered Smart Nursery Assistant  
**Last updated:** November 5, 2026

---

# Historical Project Record — CoursePath

> **Preservation note:** The following stages document the original CoursePath project. They are retained as historical records. The later agriculture project supersedes the old project selection, but does not invalidate or erase the decisions made at the time.

---

# V1 - Discover the Problem

**Program:** IEEE WIE JS Mentorship Program 2026  
**Stage:** V1, problem discovery interview (6 questions, one per message)  
**Evidence labels:** [Firsthand] = I lived it or did it myself. [Observed] = I saw or heard it, not verified. [Assumption] = my belief, no data. [Unknown] = not yet known.

## Prompt given to the AI mentor (original, verbatim)

> V1 — Discover the Problem
>
> Role: You are my AI project mentor for the IEEE WIE JS Mentorship Program 2026.
>
> Context: I am a fourth-year Artificial Intelligence and Data Science student at Tafila Technical University (TTU), Jordan. I have three possible project ideas:
>
> 1. Academic Planning Assistant: An assistant that helps TTU students understand their study plans, course prerequisites, completed courses, and possible next-semester courses. I experienced a problem when a Data Mining section was cancelled, even though the course is a prerequisite for two later courses. This could affect students' academic plans and graduation timelines.
> 2. Student Transportation: A project related to transportation problems faced by university students. I have not clearly defined the exact problem yet.
> 3. Heart Care Assistant: An AI-related project intended to help people with weak heart muscles. The exact problem and solution are not yet defined.
>
> Task: Help me understand the real problem behind each idea before comparing or choosing between them.
>
> Interview me by asking one question per message, with a maximum of 6 questions in this first stage. Prioritize understanding:
>
> - Who experiences the problem?
> - When and how often does it happen?
> - How do people currently deal with it?
> - What makes the current solution insufficient?
> - What evidence do I have, and what am I only assuming?
>
> Start with the academic planning idea, then explore the other two. If you need more information, prioritize the questions that will help us understand the problem rather than its technical solution.
>
> Constraints:
>
> - The project lasts 8 weeks.
> - I will work alone, with around 3–8 hours available between weekly mentorship sessions.
> - I can use one AI subscription but cannot rely on additional paid services.
> - The final project must be realistic and demonstrable live.
> - Do not invent facts or assume that data is available.
> - Do not choose the project for me during this stage.
> - If something is ambiguous, ask me instead of deciding it yourself.
>
> Format: Ask one clear question and wait for my answer before continuing. After the interview, summarize the three problems separately and identify any important unknowns.
>
> Keep a record of the questions and answers so I can document the actual process in my "prompt-log.md" file.

## Interview record

### Q1 (Academic Planning)
**Q:** After the Data Mining cancellation, what did you do to figure out the impact, who or what did you check, and what was the outcome?

**A (summary):** I contacted the university and travelled from Salt to Tafila, but found no solution. I registered for fewer credit hours because no suitable alternative courses were available. The other offered courses did not move me forward in my study plan. I lost time and travel effort. This made me want a tool to plan courses, understand prerequisites, and find alternatives before registering.

**Evidence:** [Firsthand] cancellation, trip, reduced credit load, no alternatives.

### Q2 (Academic Planning)
**Q:** Do you know other students affected by the same or a similar cancellation, and how do you know?

**A (summary):** Yes. I contacted other students with the same problem; a small group collected each other's names and went to the university together, with no useful result. I also noticed similar complaints from Cybersecurity students (an important course not open for registration while less relevant courses were offered) and many complaints about this semester's offerings. I can't say how common it is university-wide.

**Evidence:** [Firsthand] small group of affected students. [Observed] Cybersecurity and general offering complaints. [Unknown] how widespread.

### Q3 (Academic Planning)
**Q:** How do TTU students currently work out which courses to take before registration, and where does that fail?

**A (summary):** Students check the semester course offering list and pick from what is available. Important study-plan courses may not be offered while electives are. The university decides offerings. Registration opens for everyone at once, so sections can fill fast. If a section is full, students may need an in-person "no objection" approval from the instructor and department head, then take it to the registration office. Sections can be cancelled for low enrollment even when important (e.g., Data Mining). Main failure: students have little control over what is offered and can't plan ahead. A useful system should help with prerequisites, identify the most important courses, and explore alternatives based on courses actually offered.

**Evidence:** [Firsthand] current process and its failures as I experienced them. [Unknown] how the university decides offerings or cancellations.

### Q4 (Transportation)
**Q:** Think of the last time transportation caused a problem for you or another student. What happened, and who was affected?

**A (summary):** Most students from my area face this problem. Students near the South Bus Terminal in Amman seem to have easier access. I believe students from Irbid, Jerash, Ajloun, Mafraq and Al-Balqa may face similar difficulty because reaching the terminal takes long and options are limited. I have not collected data.

**Evidence:** [Observed] students from my area. [Assumption] northern governorates and Balqa. [Unknown] numbers.

### Q5 (Transportation)
**Q:** Walk me through your most recent trip between Salt and TTU: how, how long, how often, and what went wrong?

**A (summary):** Public transport route: taxi home to Salt Bus Terminal (~10 min), bus Salt to Raghadan, Amman (1-1.5 h, up to 2 h), service taxi Raghadan to South Bus Terminal (~30 min), bus to Tafila (~3 h). Cost at least 10 JOD. Booking an external bus directly to Tafila is more convenient, but direct buses from Salt are rare; sometimes I take a taxi to a gathering point in Salt, or travel to Sweileh in Amman. Options depend on departure location, fixed schedules, and whether enough passengers have booked. Trip is expensive, long, and hard to plan around university commitments.

**Evidence:** [Firsthand] route, times, cost, booking constraints. [Unknown] how often I make the trip.

### Q6 (Heart Care)
**Q:** Who specifically do you have in mind, and what day-to-day problem have you actually seen or heard about?

**A (summary):** My grandfather had a heart attack that weakened his heart muscle, and he later passed away. This motivated me to explore how AI could support people with a weakened heart muscle. I have not identified a specific daily problem he faced or verified what other patients experience. I would need to learn from patients, caregivers, or healthcare professionals. Any tool must support patients safely and not replace medical advice or diagnosis.

**Evidence:** [Firsthand] personal motivation. [Unknown] the actual problem, the affected group, current coping methods.

## Problem summaries

### 1. Academic Planning
- **Who:** TTU students whose study plans depend on courses that may not be offered. Confirmed: me and a small group of classmates. Observed: Cybersecurity students.
- **Problem:** Students can't predict or influence which courses are offered or cancelled. A cancelled prerequisite (Data Mining, prerequisite for two later courses) can delay progress and graduation.
- **When/how often:** Each registration period; cancellations on low enrollment. Frequency unknown.
- **Current coping:** Check the offering list, race to register, in-person "no objection" approval, visit offices, take fewer credits.
- **Why insufficient:** Offerings are outside student control; no alternatives found; costly in-person follow-up with no resolution.
- **Evidence vs assumption:** Firsthand case plus a small group; wider spread is unverified.

### 2. Student Transportation
- **Who:** Confirmed: me (Salt to Tafila). Observed: students from my area. Assumed: northern governorates and Balqa.
- **Problem:** Reaching TTU from Salt requires several connections, 10+ JOD, and roughly 5-7 hours one way (my estimate from the legs listed). Direct options are rare and depend on schedules and passenger numbers.
- **When/how often:** Frequency unknown.
- **Current coping:** Multi-leg public transport, or booking an external bus to Tafila from a gathering point.
- **Why insufficient:** Expensive, slow, hard to plan, dependent on departure location.
- **Evidence vs assumption:** Firsthand trip details; prevalence is unverified.

### 3. Heart Care
- **Who:** People with a weakened heart muscle (and possibly caregivers). Specific group not defined.
- **Problem:** Not yet defined.
- **When/how often, current coping, why insufficient:** Unknown.
- **Evidence vs assumption:** Only personal motivation; no verified problem.
- **Note:** Any project here carries safety considerations (must not replace medical advice or diagnosis).

## Important unknowns

**Academic Planning**
- How many students are affected, and in which majors?
- How and when does TTU decide offerings and cancellations? Is any of that information visible to students?
- Is the study plan, prerequisite, and offering data accessible, and in what format?
- Do advisors or the registration office already provide any guidance?

**Transportation**
- How often do I and others make the trip (weekly, daily, per semester)?
- How many students share this route or similar ones?
- What do other students do (shared taxis, private cars, group bookings, renting near campus)?
- What exactly is the core problem: cost, time, scheduling, or finding direct options?

**Heart Care**
- Who is the user (patient, caregiver, clinician)?
- What daily problem exists, and how is it handled today?
- Can I access patients, caregivers, or healthcare professionals within 8 weeks?
- What safety and data limits apply?

**Across all three**
- Which problems can be validated with real people within the first weeks?
- Which could be demonstrated live within my time and tool limits? (Not assessed yet.)

---

*(End of V1 record. The V1 file originally ended with "No project chosen. Next step: compare the three problems." That status is superseded by the current status at the bottom of this file.)*

---

# V2 - Compare the Problems

> Note: V2 was not yet in this file when V1 was saved. It is added here with V3 and V4.

## Prompt given to the AI mentor (original, verbatim)

> V2 — Compare the Problems
>
> You are my AI project mentor for the IEEE WIE JS Mentorship Program 2026.
>
> We have completed V1, a six-question interview about three possible project ideas:
>
> 1. Academic Planning for TTU students.
> 2. Student Transportation between Salt and Tafila Technical University.
> 3. Heart Care support for people with a weakened heart muscle.
>
> Use the actual answers and evidence labels from my V1 prompt log. Do not invent facts or treat assumptions as verified evidence.
>
> Task: Compare the three problems using these criteria:
>
> - Clarity of the problem and target user.
> - Strength of existing evidence and ease of validating it with real people.
> - Availability and reliability of the required data.
> - Feasibility for one student working for 8 weeks, with 3–8 hours between weekly mentorship sessions.
> - Potential to build a useful working prototype and demonstrate it live.
> - Technical difficulty, safety risks, and dependence on external organizations or services.
> - Whether AI is genuinely useful for solving the problem.
>
> For each idea:
>
> 1. Explain its strongest advantage and biggest weakness.
> 2. Identify the most important unknown that should be checked before committing.
> 3. Suggest one small validation activity that I could complete in the first week without spending money.
> 4. Describe what a realistic, limited prototype might look like, without designing the full solution yet.
>
> Then create a comparison table and explain the trade-offs honestly.
>
> Important considerations:
>
> - For Academic Planning, distinguish between helping students plan around the courses actually offered and trying to predict or control university decisions. Do not assume that all study plans, prerequisites, or course-offering data are accessible.
> - For Transportation, distinguish my firsthand travel experience from assumptions about students in other governorates. Do not assume real-time transport data is available.
> - For Heart Care, remember that I have personal motivation but have not identified a verified patient problem. Any prototype must avoid diagnosis or replacing medical advice.
>
> Do not select a final project for me yet. Do not start coding. End by identifying the two most useful questions I should answer before making the decision.

## Response summary

**Academic Planning**
- Strongest advantage: best-supported problem (my own case plus a small group); users are easy to reach.
- Biggest weakness: the root cause (offerings and cancellations) is outside student control. A tool can only help plan around what is offered, not predict or control decisions.
- Key unknown: whether usable study-plan, prerequisite, and offering data can be obtained.
- Week-1 validation: collect my major's study plan and the current offering list, and hand-trace the Data Mining prerequisite chain.
- Limited prototype: one major; completed courses plus a manually entered offering list produce eligible/blocked courses and what a missing course would block; sample profiles only.

**Student Transportation**
- Strongest advantage: concrete firsthand trip (about four legs, at least 10 JOD, roughly 5-7 hours one way, the 5-7 hours being the mentor's sum of my stated times).
- Biggest weakness: only my own trip is firsthand; prevalence is observed or assumed; the core issue looks like too few direct buses, which software can't create.
- Key unknown: how many other students make similar trips, how often, and what they do today (my own trip frequency is also still unknown).
- Week-1 validation: ask 5-10 students four short questions (where from, how often, how they travel, biggest pain) and log my own next trip.
- Limited prototype: a one-route planner using manually collected static information; no real-time data assumed; any matching-board demo would need clearly labelled simulated users.

**Heart Care**
- Strongest advantage: strong personal motivation and potentially high impact.
- Biggest weakness: no verified problem, user, or current workaround; highest safety risk.
- Key unknown: who the user is (patient, caregiver, clinician) and what daily problem they face; access to such people.
- Week-1 validation: one 20-30 minute open conversation with someone close to heart-weakness care, about daily difficulties rather than solutions.
- Limited prototype: depends on what is learned; a non-clinical tool using fictional data, with no diagnosis, symptom interpretation, or medication advice.

**Comparison (mentor's judgments, not facts)**

| Criterion | Academic | Transport | Heart Care |
|---|---|---|---|
| Problem/user clarity | Clear, root cause outside students' control | Clear for me; wider group unverified | Unclear |
| Existing evidence | Medium | Medium for me, low beyond | Low (motivation only) |
| Ease of validating | High | Medium to high | Low to medium |
| Data availability | Unknown, must check | Static info by hand | Sensitive; none verified |
| 8-week feasibility | Medium to high (one major) | Medium | Low to medium |
| Live demo potential | High | Medium | Medium, weak credibility |
| Difficulty/safety/dependencies | Low to medium | Low to medium | Highest |
| AI usefulness | Medium (core logic is rule-based) | Low to medium | Unknown; risky |

## Decision and what changed

- **Decision:** none yet, as requested.
- **What changed from V1:** the unknowns became criteria-based comparisons and week-1 validation ideas. Academic Planning emerged as the strongest on evidence and demo-ability, but with the caveat that it addresses planning and visibility, not the cancellations themselves.
- **Two questions to answer before deciding:** (1) Would 5-10 real people confirm the problem and say they'd use a helping tool? (2) Which data or people can I actually access for free in the next week?

## Remaining assumptions after V2
- Wider prevalence of each problem: unverified.
- Data access for Academic Planning: unverified.
- Heart Care user and problem: undefined.

---

# V3 - Select the Project

## Prompt given to the AI mentor (original, verbatim)

> V3 — Select the Project
>
> You are my AI project mentor for the IEEE WIE JS Mentorship Program 2026.
>
> We have completed:
>
> - V1: Discover the Problem.
> - V2: Compare the Problems.
>
> Use the actual evidence and comparison from those stages. Do not invent validation results or claim that I interviewed additional students.
>
> My three ideas are:
>
> 1. Academic Planning for TTU students.
> 2. Student Transportation between Salt and Tafila Technical University.
> 3. Heart Care support for people with a weakened heart muscle.
>
> I can access or obtain the study plan and semester course offering list for my major, and I can reach approximately 5–10 students for future validation. However, I have not conducted those additional interviews yet.
>
> Task: Help me select one project for an 8-week, solo AI mentorship project.
>
> Evaluate the three ideas based on:
>
> - Strength of the problem evidence.
> - Feasibility within 8 weeks and 3–8 hours between weekly sessions.
> - Access to the required data and users.
> - Potential to build a working prototype and demonstrate it live.
> - Whether AI adds meaningful value.
> - Safety risks and dependence on university decisions or external services.
>
> For the selected project, define:
>
> 1. A clear project title.
> 2. The specific target user.
> 3. The problem statement in 2–4 sentences.
> 4. The proposed solution and how it addresses the problem.
> 5. Why this project is worth building.
> 6. What I can realistically demonstrate at the end of 8 weeks.
>
> Also explain why the other two ideas were not selected, in 2–3 sentences each.
>
> Important:
>
> - Distinguish helping students plan around actual course offerings from predicting or controlling university decisions.
> - Do not promise that the system can prevent cancellations or guarantee graduation.
> - Do not assume all data is available or verified.
> - Do not begin coding or expand the project into a full university platform.
> - If you recommend Academic Planning, keep the first version limited to TTU's AI & Data Science major.
>
> Give me your recommendation with honest reasoning, but identify any remaining assumptions clearly.

## Response summary

**Recommendation: Academic Planning, limited to TTU's AI & Data Science major.**

- **Title:** CoursePath: A Course-Offering-Aware Planning Assistant for TTU AI & Data Science Students
- **Target user:** TTU AI & Data Science students planning next semester's registration.
- **Problem:** students choose from the offering list, but important plan courses may not be offered or may be cancelled for low enrollment. When a prerequisite such as Data Mining is unavailable, it is hard to see what it blocks and which offered courses still fit the plan.
- **Solution:** a prototype that takes the study plan, completed courses, and the semester offering list, then shows eligible, blocked, and downstream-affected courses, plus the best-fitting offered options, with an AI layer for plain-language questions and explanations. It helps students plan around what is offered; it does not predict or control university decisions.
- **Why worth building:** the problem was experienced firsthand and cost real time, money, and credits; the users are reachable.
- **Realistic week-8 demo:** one major, synthetic student profiles, eligible/blocked output, a Data Mining-style scenario, a few plain-language Q&A answers, and feedback from the 5-10 check-ins only if they are completed.

**Why the others were not selected**
- **Transportation:** only my own trip is firsthand; the core issue looks like too few direct buses, which software can't fix; a matching tool needs enough users to be demonstrable.
- **Heart Care:** strong motivation but no verified patient problem or access to patients/professionals, and the highest safety risk for a solo 8-week project. Kept as a longer-term interest.

## Decision and what changed

- **Decision:** Academic Planning (CoursePath), first version limited to the AI & Data Science major.
- **What changed from V2:** the choice was made on evidence strength, data and user access, demo-ability, and safety. The scope was narrowed from "academic planning" to a planning aid with explicit limits (no cancellation prevention, no graduation guarantee).

## Remaining assumptions after V3
- AI adds only moderate value; eligibility and prerequisite logic is rule-based. AI is for natural-language questions and explanations.
- Study-plan and offering-list format, completeness, and prerequisite coverage: **not verified**.
- Whether other students confirm the problem: **not verified** (check-ins not done).
- Whether an offered course counts toward the plan depends on university rules not yet seen; the tool must flag "needs advisor confirmation."

---

# V4 - Define the MVP

## Prompt given to the AI mentor (original, verbatim)

> V4 — Define the MVP
>
> You are my AI project mentor for the IEEE WIE JS Mentorship Program 2026.
>
> My selected project is:
>
> CoursePath: A Course-Offering-Aware Planning Assistant for TTU AI & Data Science Students.
>
> The project helps TTU AI & Data Science students understand which courses they may be eligible to take based on their completed courses, the official study plan, prerequisites, and the current semester's course offering list. It also explains which courses may be blocked by an unavailable prerequisite and identifies potentially suitable offered courses.
>
> The prototype may include a natural-language AI interface, but prerequisite eligibility must be determined using explicit rules and verified data, not generated guesses.
>
> Constraints:
>
> - 8 weeks total.
> - I will work alone.
> - I have approximately 3–8 hours between weekly mentorship sessions.
> - I can use one AI subscription but cannot rely on additional paid services.
> - The final project must be a working prototype that I can demonstrate live.
> - The official study plan and offering list appear accessible to me, but their exact format and completeness have not yet been verified.
> - I have not completed the planned check-ins with 5–10 students yet.
> - I must not use private student records without permission.
>
> Task: Propose the smallest useful MVP for CoursePath.
>
> Please define:
>
> 1. Core user and problem: One specific user and one primary problem.
> 2. User journey: What the student enters, what the system processes, and what the student sees.
> 3. Essential features: Separate must-have features from optional features.
> 4. Course eligibility logic: Explain how completed courses, prerequisites, and offered courses will be checked using deterministic rules.
> 5. Unavailable-course analysis: Explain how the prototype could show downstream courses affected by a missing course, without claiming that a course will definitely be cancelled or that graduation will be delayed.
> 6. AI role: Identify what should use normal programming logic and what genuinely benefits from AI.
> 7. Data requirements: List the minimum required data and how I should verify it before implementation.
> 8. Demo success criteria: Define 3–5 observable criteria for a successful live demonstration.
> 9. Out of scope: Explicitly exclude automatic registration, guaranteed graduation predictions, university-wide coverage, unverified alternative-course approvals, and features that depend on unavailable data or permissions.
> 10. Main risks and assumptions: Identify what could prevent the MVP from working.
> 11. MVP boundary: Give me a clear final list of features I should commit to and features I should leave out.
>
> Do not start coding or produce a detailed week-by-week implementation plan yet. Do not assume that AI must be used for every feature. Keep the MVP achievable within the stated constraints, and label all unverified assumptions clearly.

## Response summary

- **Core user and problem:** a TTU AI & Data Science student preparing next semester's registration; when a course isn't offered, they can't quickly see what it blocks or which offered courses still fit the plan.
- **User journey:** the student selects completed courses (and optionally marks a course "unavailable" for a what-if); the system checks each course against plan rules and the offering list; the student sees eligible-and-offered, not-offered, and blocked lists (with the missing prerequisite), the downstream impact of an unavailable course, and can ask plain-language questions.
- **Must-have features:** structured course/prerequisite data; completed-course input; eligibility checker; offered/not-offered flag; unavailable-course impact view; "why?" explanations; advisor-confirmation warnings.
- **Optional features:** natural-language question box; credit-hour totals; export/print; prerequisite graph visual.
- **Eligibility logic (deterministic):** a course is eligible if it isn't completed, its prerequisite rule is satisfied by the completed set, and it is in the offering list. If the rule is satisfied but it isn't offered: "eligible by plan, not offered." If the rule isn't satisfied: "blocked," naming the missing prerequisites. Rules the data can't express are shown as "needs advisor confirmation."
- **Unavailable-course analysis:** walk prerequisite links forward from the unavailable course to list direct and downstream dependents. Cautious wording only ("may not be able to take next semester"); never claims a cancellation, delay, or graduation impact. Offered, eligible plan courses appear as "possible options; substitution needs department approval."
- **AI role:** normal code does eligibility, matching, traversal, credit totals. AI only helps turn natural-language questions into structured requests, explain the engine's output, and optionally draft structured data from plan documents (to be manually verified). Whether a live LLM call fits the free/one-subscription constraint is unverified; fallback is fixed question types, labelled honestly.
- **Minimum data:** study plan (code, name, credits, category, prerequisites, semester placement), offering list (course code, section if available), synthetic test profiles (no real records).
- **Verification before building:** check every course against the official plan; have a classmate or advisor spot-check prerequisites; list unclear rules separately; write 5-10 test cases with known answers (including a synthetic reconstruction of the Data Mining scenario); record the date and source of the offering list.
- **Demo success criteria:** (1) correct eligible/blocked/not-offered lists on all hand-checked test cases; (2) Data Mining marked unavailable shows direct and downstream dependents with cautious wording; (3) every blocked result names the missing prerequisite; (4) uncertain rules are flagged "confirm with advisor"; (5) if AI is included, at least two plain-language questions return answers consistent with the rule engine.
- **Out of scope:** automatic registration or TTU system integration; cancellation prediction or graduation guarantees; other majors or university-wide coverage; approving substitutions; real student records, logins, or personal data; anything depending on unavailable data or permissions.
- **Main risks:** plan/offering data may be incomplete, scanned, or inconsistent; plans may have rules beyond simple prerequisites; the offering list can change; check-ins not done; a live AI feature may fail; data cleaning could consume the time budget.
- **MVP boundary:** commit to structured plan data for one major, completed-course input, eligibility checker, offered/not-offered matching, unavailable-course impact view, explanations, and advisor-confirmation warnings. Leave out automation, predictions, other majors, substitution approvals, real records, and the optional polish items; the natural-language interface stays optional until the core passes its test cases.

## Decision and what changed

- **Decision:** the MVP is a deterministic rule engine plus an explanation layer, with AI optional and subordinate to the rules.
- **What changed from V3:** the "AI assistant" framing became "rule-based planner first, AI second." The tool shows eligibility and impact; it never claims to predict or decide.
- **Two checks that matter most before moving on:** (1) can the major's study plan be converted into clean structured data? (2) are there prerequisite rules that can't be expressed as simple course-code conditions?

---

# Current status (after V4)

**Completed:** V1 (problem discovery), V2 (comparison), V3 (project selection), V4 (MVP definition).

**Not completed yet:**
- **Student check-ins (5-10 students):** NOT done. No validation results exist. Any statement about how many students share this problem remains unverified.
- **Data verification:** NOT done. The study plan and offering list are believed to be accessible, but their format, completeness, and prerequisite rules have not been checked or converted to structured data.
- **Test cases:** not yet written.
- **Live AI feature feasibility** under the one-subscription, no-extra-cost constraint: not checked.

**Next stage:** verify the data and run the check-ins before committing fully; a week-by-week plan has not been created yet.

---

# V5 - Test Feasibility & Risks

## Prompt given to the AI mentor (original, verbatim)

> V5 — Test Feasibility & Risks
>
> You are my AI project mentor for the IEEE WIE JS Mentorship Program 2026.
>
> My selected project is:
>
> CoursePath: A Course-Offering-Aware Planning Assistant for TTU AI & Data Science Students.
>
> We have completed:
>
> - V1: Discover the Problem.
> - V2: Compare the Problems.
> - V3: Select the Project.
> - V4: Define the MVP.
>
> Use the existing "prompt-log.md" and the decisions made in V1–V4 as the source of truth. Do not invent facts, validation results, or data availability.
>
> Project context:
>
> CoursePath is intended to help a TTU AI & Data Science student plan for registration by using their completed courses, the major's study plan and prerequisites, and the current semester's course offering list.
>
> The core prototype may show:
>
> - Courses that appear eligible based on completed courses and verified prerequisites.
> - Courses that appear eligible by plan but are not offered this semester.
> - Courses blocked by missing prerequisites.
> - Direct and downstream courses that may be affected if a prerequisite is unavailable.
> - Explanations and warnings when university rules are unclear.
>
> The core eligibility logic should use deterministic programming rules. A natural-language AI interface is optional and must not be allowed to invent courses or determine eligibility independently.
>
> Current constraints and status:
>
> - The project lasts 8 weeks.
> - I work alone, with approximately 3–8 hours between weekly sessions.
> - I can use one AI subscription but cannot rely on additional paid services.
> - I can obtain the study plan and offering list, but I have not verified their formats, completeness, or prerequisite rules yet.
> - I have not completed interviews or check-ins with 5–10 students.
> - I have not written the test cases yet.
> - I will not use private student records without permission.
> - The prototype must be demonstrable live.
>
> Your task:
>
> 1. Assess whether the current MVP is realistic within the time and resource limits. Be honest about what may need to be simplified.
>
> 2. Identify the five biggest project risks. For each risk, explain:
>
>    - Why it matters.
>    - How I can check it without spending money.
>    - A practical fallback if the risk becomes a problem.
>
> 3. Separate what must be verified before implementation from what can be tested during development. Do not claim that any verification has already happened.
>
> 4. Review the data requirements. Identify the minimum course information required for a working prototype and which complicated university rules should be excluded or flagged for advisor confirmation.
>
> 5. Evaluate whether an AI feature is genuinely necessary for the first working demo. Compare:
>
>    - A deterministic planner with predefined explanations.
>    - A planner with an optional natural-language AI interface.
>
>    Recommend the safer choice for an 8-week solo project without assuming access to a free API.
>
> 6. Define a minimum feasibility test using a small, manually prepared sample of courses and a synthetic student profile. Include a test involving Data Mining being unavailable and explain what a successful result would look like. Do not pretend this test has already been performed.
>
> 7. Identify clear conditions under which I should reduce the scope or remove a feature.
>
> 8. End with a concise feasibility verdict: realistic, realistic with scope reductions, or not realistic in its current form. Explain why.
>
> Important restrictions:
>
> - Do not start coding.
> - Do not create a detailed week-by-week implementation plan.
> - Do not expand the project to other majors or universities.
> - Do not promise that the tool can prevent cancellations, approve substitutions, or guarantee graduation.
> - Clearly label unverified information and proposed tests.
> - Do not repeat V1–V4 in full.
>
> After the analysis, provide a concise V5 record that I can append to "prompt-log.md", including the prompt used, key findings, any decisions or changes, and remaining unknowns. Preserve the existing V1–V4 records.

## Key findings (mentor's analysis)

**Verdict: realistic with scope reductions**, conditional on the data checks below. The main uncertainty is the data, not the programming.

**Simplifications recommended:** hand-enter data (no PDF parsing); start with a vertical slice (the Data Mining dependency chain plus a limited set of nearby courses); basic interface; predefined explanations; natural-language AI as a stretch feature only.

**Five biggest risks (check at no cost / fallback)**
1. *Plan or offering list not usable as-is (scan, inconsistent, incomplete).* Check: obtain both, note the format, hand-enter 10 courses and time it. Fallback: enter only the Data Mining chain and nearby courses; label the demo "partial plan."
2. *Prerequisite rules go beyond simple course codes.* Check: copy every prerequisite statement and label it simple-AND, OR, or other. Fallback: encode only AND/OR; show the rest as "confirm with advisor."
3. *Offering list stale, partial, or without sections.* Check: record its date and source and whether it lists course codes. Fallback: treat it as a replaceable input file with an "as of" date in the output.
4. *Problem not validated beyond my own case and a small group.* Check: 5-10 students, four short questions, plus a paper mockup of the output. Fallback: present the project honestly as based on my experience and a small group; report partial check-in results as partial.
5. *Time and scope: data cleaning consumes hours, optional features creep, AI feature fails.* Check: time-box the first 10 course entries; log hours weekly. Fallback: cut in this order: natural-language interface, graph visual, export, credit totals.

**Verify BEFORE implementation (none done yet)**
- Plan and offering list obtained, and their formats known.
- All prerequisite statements classified (simple vs complex).
- Which courses depend on Data Mining, confirmed against the official plan (V1 says two later courses; names and codes unverified).
- Offering list date and source recorded.
- List of excluded or flagged rules agreed.
- Test data decided: synthetic profiles only, no private records.

**Test DURING development:** engine output vs hand-written expected answers; multi-level downstream traversal; wording of explanations; edge cases (completed course outside the plan, course with no prerequisites, missing or circular prerequisite entries); interface clarity with 1-2 people; demo rehearsal; any optional AI behavior.

**Minimum data per course:** code, name, credits, structured prerequisite rule, offered this semester (yes/no). Optional: category, plan semester, section.

**Exclude or flag for advisor confirmation (if present in the plan or rules; unverified):** minimum grades; credit-hour or standing requirements; corequisites; instructor/department approvals, including the "no objection" process; substitutions or equivalents; retake rules; credit-load limits; elective-category counting and graduation-requirement rules.

**AI for the first demo:** not necessary. Recommended: deterministic planner with predefined explanations generated from the rule engine's output. Reasons: no free API access assumed; the subscription's use as a runtime service is unverified (it is a development aid); lower demo risk; the core value (correct eligibility and impact) does not need AI. A middle path is a dropdown of fixed question types, which gives a question-and-answer feel without any AI. Honest trade-off: the demo is less "AI"-visible; raise this with the mentor. AI can still help during development (drafting test cases, helping with code, suggesting structured data from plan text, all of which must be manually verified) and that use can be documented in this log.

**Proposed minimum feasibility test (NOT yet performed)**
- Sample: about 9 manually prepared placeholder courses until real data is verified. Example structure: A (no prerequisite); B (no prerequisite); C (needs A); D = Data Mining (needs B and C; placeholder rule); E and F (each needs D); G (needs E); H (needs A); I (needs B or C); J (rule flagged "advisor confirmation").
- Profile 1 (synthetic): completed A, B, C. Offering list: all offered except D.
- Expected, written before running: D = eligible by plan, not offered. E, F = blocked, missing D. G = blocked, missing E (depends on D). H, I = eligible and offered. J = flagged for advisor confirmation.
- Data Mining unavailable what-if: lists E and F as direct dependents and G as downstream, with cautious wording; no claim of cancellation, delay, or graduation impact.
- Profile 2 (synthetic): completed A, B, C, D. Expected: E and F become eligible if offered.
- Success: output matches every expected result; every blocked course names its missing prerequisite; flagged rule shown as advisor confirmation; wording passes a check for forbidden claims; the test can be set up and run within roughly one session (proposed target, adjustable).

**Reduce scope or remove a feature if (proposed triggers):**
- Hand-entering the first 10 courses takes more than one session -> restrict data to the Data Mining chain plus a small set of courses.
- Many prerequisite statements are not simple AND/OR -> encode only AND/OR and flag the rest.
- Offering list not obtainable in usable form early on -> use a manually entered, clearly labelled sample list.
- Check-ins cannot be done -> proceed on my own evidence and label the demo as unvalidated.
- Core test cases not passing by the project midpoint -> freeze all optional features.
- No confirmed runtime AI access -> remove the natural-language interface.

## Decisions and changes (recommended; student to confirm)
- First demo uses a deterministic planner with predefined explanations; the natural-language AI interface moves from "optional in MVP" to "stretch only."
- Data scope narrowed to a vertical slice around the Data Mining chain.
- Complex university rules excluded or flagged "confirm with advisor."
- Expected test results are written before the engine is run.
- AI is documented as a development aid.

## Remaining unknowns and status
- **Not done:** student check-ins, data verification, test cases, and the feasibility test. No results exist for any of them.
- **Unknown:** plan and offering-list format and completeness; which prerequisite rules are non-simple; whether the Data Mining dependents match what V1 states; whether runtime AI access is possible within the constraints; whether the mentor expects a visible AI component.
- **Next step:** do the "verify before implementation" checks and decide whether the reductions above are accepted.

---

# V5 Addendum - Train a Task-Specific AI Model

> The original V5 record above is preserved unchanged. This addendum documents a new requirement and its effect on the feasibility assessment.

## Prompt given to the AI mentor (original, verbatim)

> V5 Addendum — Train a Task-Specific AI Model
>
> After the original V5 feasibility assessment, I clarified an important requirement: I want CoursePath to include a model that I train myself using a dataset I prepare. I also want the final product to be a useful conversational academic assistant, not only a rule-based planner.
>
> Available resources: my laptop and a free cloud notebook environment. I cannot rely on paid APIs or guaranteed GPU access.
>
> Please reassess feasibility with this requirement.
>
> Consider a realistic approach in which I:
>
> - Create a labelled dataset of student questions related to academic planning.
> - Train a task-specific intent-classification model using a lightweight machine-learning approach.
> - Evaluate the trained model on held-out examples.
> - Connect its predictions to CoursePath's deterministic academic planning engine.
> - Generate grounded responses using verified course data and predefined response templates.
>
> The initial model may classify intents such as eligible-course queries, missing prerequisites, unavailable courses, downstream impact, result explanations, and uncertain rules. Treat these as proposed classes that may be refined.
>
> Please explain:
>
> 1. Whether this approach is realistic within eight weeks and 3–8 hours between weekly sessions.
> 2. A reasonable initial dataset target and how to avoid evaluating the model on near-duplicate training examples.
> 3. Which parts must be learned by the trained model and which should remain deterministic.
> 4. Suitable lightweight model choices and evaluation metrics.
> 5. How the assistant should respond when the model is uncertain or the question is outside its supported classes.
> 6. A fallback if the trained model performs poorly or time becomes limited.
>
> Do not assume I have already created the dataset, trained the model, measured performance, or validated the problem with students. Do not require a paid API or guaranteed GPU access.
>
> Preserve the original V5 record. Provide this as an addendum documenting the updated AI requirement and any changes to the feasibility assessment.

## What changed
- **New requirement (from me):** the product must include a model I train myself on a dataset I prepare, and should work as a conversational academic assistant. This supersedes the original V5 recommendation that AI was "not necessary" for the first demo. The trained model is now a core component, kept isolated from the rule engine.
- **Resources:** laptop plus a free cloud notebook; no paid APIs; no guaranteed GPU.

## Key findings (mentor's analysis; nothing here has been done or measured)

**Verdict: still realistic with scope reductions, but with a heavier workload and more risk than the original V5.** A lightweight intent classifier trains in seconds on a laptop CPU, so compute is not the constraint. The bottleneck is writing and labelling a diverse dataset, and evaluating it honestly.

**What "conversational" means here:** a guided, task-oriented assistant: the model picks an intent, deterministic code finds course entities and runs the engine, and templates produce the answer. It is not a free-form chatbot and does not generate open-ended text.

**Proposed intents (refinable):** eligible_courses, missing_prerequisites, unavailable_course_impact, downstream_impact, explain_result, uncertain_rule, out_of_scope. Likely confusable pair: unavailable_course_impact vs downstream_impact; merge if the confusion matrix shows it.

**Dataset (proposed targets, adjustable):** about 50 examples per in-domain class and about 80 for out_of_scope for training/validation (about 380); a separate hand-written test set of about 15 per in-domain class and about 30 out_of_scope (about 120). Total about 500. Rough, unverified effort estimate: 6-10 hours of writing and labelling plus review. Questions must contain no private student information; any real questions from classmates need permission and anonymization.

**Avoiding near-duplicate leakage:** write examples in groups (a base question plus its paraphrases) and split by group, never by row; mask course names/codes with a placeholder before training and de-duplicate after masking; write the test set separately and lock it (no tuning on it); automatically check train/test similarity (for example TF-IDF cosine similarity) and remove pairs above a chosen threshold (proposed starting point about 0.8); AI-drafted paraphrases are allowed only as manually reviewed drafts and should not be used in the test set; add a small "hard" test set (typos, mixed language, multi-intent, near-domain out-of-scope).

**Learned vs deterministic**
- Learned: intent classification only (including an out_of_scope class).
- Deterministic: course entity extraction (dictionary, code normalization, fuzzy matching), eligibility and prerequisite checks, offering match, downstream traversal, missing-slot handling (asking which course), confidence thresholds and routing, warnings, response templates. Every fact in a response comes from the verified data. Completed courses come from a checklist, not free-text parsing.

**Model choices and metrics**
- Baselines: a keyword-rule router (to show whether training actually adds value) and majority class.
- Core candidates: TF-IDF (word plus character n-grams) with Logistic Regression, Linear SVM (needs calibration for probabilities), Multinomial Naive Bayes. All run on CPU.
- Stretch (unverified availability): small pretrained sentence embeddings plus Logistic Regression. Fine-tuning transformers is excluded (needs GPU not guaranteed).
- Metrics: macro-F1, per-class precision/recall/F1, confusion matrix, out_of_scope false-accept and false-reject rates, accuracy-versus-coverage at the confidence threshold, and a manual end-to-end check (correct engine function and correct grounded facts). Test sets are small, so results are noisy and must be reported with that caveat. Set minimum acceptable thresholds (for example, macro-F1 around 0.8, proposed) before looking at test results.

**Uncertain or out-of-scope behaviour (layered)**
1. Low confidence: do not guess; offer the top two interpretations as options.
2. Predicted out_of_scope: say what is not supported and show examples of supported questions.
3. Intent clear but course missing or ambiguous: ask which course, with matches.
4. Intent clear but rule or data unknown: "uncertain rule" template with advisor-confirmation warning.
5. Never generate free text about university policy; never claim substitutions, approvals, cancellation, or graduation outcomes.
6. Thresholds are tuned on validation data, not test data.

**Fallback tiers**
1. Full: trained classifier + engine + templates.
2. Merge confusable classes, add data for weak classes, add character n-grams, use top-two clarification.
3. Hybrid: keyword router handles low-confidence cases; report honestly how much the trained model contributes.
4. Minimal: 3-4 intents plus out_of_scope, form-based UI as the primary interface, the model as a secondary question box. Poor results are documented honestly as findings, not hidden.

## Decisions and changes (recommended; student to confirm)
- The trained intent classifier becomes part of the committed MVP, but the form-based planner must work without it.
- Build and test the deterministic engine first so it never depends on the model.
- Test set is hand-written separately and locked; group-based splits only.
- Assistant is described as a "guided conversational assistant," not a free-form chatbot.

## Remaining unknowns
- **Not done:** dataset, training, evaluation, student check-ins, data verification, test cases, feasibility test. No results exist for any of them.
- **Unknown:** the language(s) students would use (Arabic, English, mixed) and how that affects dataset effort; whether real student questions can be used with permission; free notebook limits; whether the intent set holds up once real questions are collected.

---

# V6 - Finalize CoursePath Project Definition

## Prompt given to the AI mentor (original, verbatim)

> V6 — Finalize CoursePath Project Definition
>
> You are my project planning assistant for the IEEE WIE JS Mentorship 2026 AI & Programming track.
>
> Context
>
> My project is CoursePath: a course-planning assistant for AI & Data Science students at Tafila Technical University (TTU).
>
> The project should help students understand which courses they may be eligible to take, identify missing prerequisites, and understand how a course that is not offered may affect later courses.
>
> I want to train a task-specific machine learning model using my own prepared dataset. Students may ask questions in Jordanian Arabic dialect, Modern Standard Arabic, English, or a mixture of Arabic and English.
>
> The model will classify the intent of a question. A deterministic planning engine will handle academic rules and verified course data. Responses will use grounded templates, clarification questions, and advisor-confirmation messages.
>
> Constraints
>
> - Eight weeks, one person, 3–8 hours of work between weekly sessions.
> - Use free tools and available laptop/Colab resources; do not assume a GPU or paid APIs.
> - The project must run and be demonstrated live.
> - Training an intent classifier is a core requirement; do not replace it with a ready-made chatbot or a rule-only system.
> - Do not claim university data has been verified, students interviewed, a dataset created, or a model trained unless I have actually done it.
> - The current language requirement is Arabic dialect + MSA + English + mixed-language questions.
> - Keep the project small enough to finish.
>
> Task
>
> Finalize the project definition, not the implementation.
>
> 1. Review the existing V1–V5 records and the existing V5 addendum.
> 2. Preserve the historical records. Do not rewrite or delete them.
> 3. Define the chosen project, the problem, target users, current workaround, value, and what a successful live demo should show.
> 4. Define the scope, exclusions, risks, assumptions, and fallback plan.
> 5. Define the proposed intent-classification model and dataset plan, including the initial intent labels, language coverage, CSV schema, leakage prevention, baseline comparison, and evaluation metrics.
> 6. Keep academic eligibility, prerequisite checking, course availability, downstream dependency analysis, and factual responses in the deterministic engine using verified data.
> 7. Make clear that the initial dataset size and evaluation criteria are proposals, not completed work or achieved results.
> 8. Mark unresolved facts, especially the real TTU course relationships and available data formats.
> 9. Identify the smallest useful live-demo version if the full scope becomes too large.
> 10. Update docs/brief.md and docs/scope.md, and append a V6 entry to prompt-log.md. Keep docs/problems.md consistent with the three original candidate problems.
>
> Output
>
> - List the proposed changes before making them.
> - Then provide the complete contents of docs/brief.md and docs/scope.md.
> - Provide the exact V6 entry to append to prompt-log.md, including what changed and why.
> - Clearly separate confirmed decisions, assumptions, and work not yet done.
> - If anything is ambiguous, ask me instead of silently deciding.
>
> Do not write implementation code or claim the project is complete.

## What changed and why
- **Language requirement settled:** the V5 addendum left the language question open. V6 states four categories: Jordanian dialect, MSA, English, mixed Arabic-English. This changes the dataset plan (language and script columns, group splits that keep translations together, per-language reporting, likely larger effort than the earlier 6-10 hour estimate).
- **Classifier is a core requirement:** reaffirmed. It is not to be replaced by a ready-made chatbot or a rule-only system. The keyword router is kept only as a baseline and fallback.
- **Project definition consolidated:** problem, users, current workaround, value, demo, scope, exclusions, risks, fallback tiers, and a smallest-useful-demo version are now in `docs/brief.md` and `docs/scope.md`. The three candidate problems are summarized in `docs/problems.md`.
- **Why:** to freeze a small, finishable definition before implementation, with every unverified item and every proposal clearly labelled.
- **Historical records:** V1-V5 and the V5 addendum are unchanged.
- **Files:** `docs/brief.md`, `docs/scope.md`, and `docs/problems.md` were created as complete drafts, because earlier versions were not visible to the assistant. Compare them with any existing versions before replacing.

## Decided (by the student; not the same as verified)
- Project: CoursePath, TTU AI & Data Science only.
- A trained intent classifier on a student-prepared dataset is core.
- Deterministic engine handles all eligibility, prerequisites, availability, downstream dependencies, and factual content.
- Responses use grounded templates, clarification questions, and advisor-confirmation messages.
- Languages: Jordanian dialect, MSA, English, mixed.
- Constraints: 8 weeks, solo, 3-8 hours between sessions, free tools, no assumed GPU or paid APIs, live demo, no private student records.
- Exclusions: automatic registration, cancellation or graduation guarantees, substitution approvals, other majors or universities, real student records, paid APIs.

## Assumptions (not verified)
- The study plan and offering list are obtainable and usable.
- Data Mining is a prerequisite for two later courses (from the student's own experience; names unverified).
- Students' questions will fall into the four language styles and the proposed intents.
- A classical model on CPU is enough; free notebook limits are unchecked.
- The problem affects other students (small group firsthand; wider spread unverified).

## Proposals (not results)
- Dataset about 500 examples plus a hard test set; intent labels; CSV schema; leakage rules; baselines; metrics; success thresholds (macro-F1 around 0.80); fallback triggers. All are targets and plans only.

## Not done (no results exist)
- Student check-ins (5-10 students).
- Data verification of the study plan, prerequisites, and offering list.
- Test cases and the feasibility test.
- Dataset creation, model training, and evaluation.

## Open questions
- Which language(s) should the assistant's replies use (English only, Arabic only, bilingual, or follow the question)?
- Include or exclude Arabizi (Arabic in Latin letters)? Currently excluded.
- Merge unavailable_course_impact and downstream_impact? To be decided from data.
- Final success thresholds, to agree with the mentor.

---

# Language Policy Addendum — October 15, 2026

## Decision

CoursePath follows the language style used in the student's question.

- Jordanian Arabic dialect: respond in clear, simple Arabic.
- Modern Standard Arabic (MSA): respond in clear, simple Arabic.
- English: respond in English.
- Mixed Arabic-English: respond in simple Arabic while preserving course names and necessary academic terms in English.
- Arabizi (Arabic written in Latin letters) remains outside the current scope.

## Why this changed

V6 recorded the language and Arabizi questions as unresolved. This addendum records the subsequent decision to support four input categories and exclude Arabizi from the initial version.

## Impact on the project

The training dataset should represent the four supported input categories where practical. Dataset size, language balance, and model performance across categories remain to be tested. Translated or paraphrased versions of the same underlying question should be grouped appropriately to reduce data leakage between training and test sets.

## Historical record

This addendum does not replace or rewrite V1–V6 or the original V5 Addendum. It records a later decision made after V6.

---

# New Project Record — Agriculture / Nursery Assistant

> **Project pivot note — November 2026**
>
> After the CoursePath project definition and language-policy addendum, I reconsidered the project direction. I decided to move away from CoursePath and explore a problem connected to my family's plant nursery.
>
> This is a project pivot, not a continuation of CoursePath's academic-planning functionality. The old CoursePath stages remain part of the mentorship history, but they are no longer the current project.

---

# V7 — Reopen Project Selection and Pivot to Agriculture

**Stage:** Reconsider the selected project and compare the current candidate problems.  
**Date:** November 5, 2026  
**Evidence labels:** [Firsthand], [Observed], [Assumption], [Unknown].

## Prompt given to the AI mentor

> **Documentation note:** The following is a reconstructed summary of the request and discussion, not a verbatim prompt transcript.
>
> Revisit the project selection for the IEEE WIE JS Mentorship Program 2026.
>
> CoursePath was previously selected, but I want to reconsider the direction and explore a project based on a real problem in my family's plant nursery.
>
> Compare these three current candidates:
>
> 1. Heart Care.
> 2. Agriculture / Nursery Management.
> 3. University Academic Planning (CoursePath).
>
> Use the actual context and evidence already discussed. Do not invent validation results or treat assumptions as facts.
>
> Explain the strongest reasons for selecting agriculture and the reasons for not selecting the other two.
>
> Keep the original CoursePath records intact. Document the new decision as a later project pivot.

## Current candidate comparison

### 1. Agriculture / Nursery Management

**Problem area:** Managing and monitoring individual plants in a nursery can take substantial time. Identifying a plant's condition, deciding whether it needs water or another form of care, and following up on changes may require repeated inspection and judgement.

**Evidence available:**
- [Firsthand] The nursery belongs to my family, and I have direct knowledge of some of its daily work and challenges.
- [Observed] I have seen the time and effort involved in inspecting, watering, treating, cleaning, arranging, moving, and monitoring plants.
- [Unknown] The exact frequency of each problem, the number of affected plants, and measurable losses have not been recorded.
- [Assumption] A software assistant may reduce some of the time and uncertainty involved in plant monitoring. This needs testing.

**Strongest advantage:** There is an accessible real-world environment and a potential primary user: my father, who manages the nursery.

**Main limitation:** Plant identification, disease classification, watering assessment, and persistent plant tracking are different technical problems. A photograph cannot reliably establish every plant condition or measure soil moisture.

### 2. University Academic Planning — CoursePath

**Problem area:** Students may struggle to plan registration when important courses are not offered or when prerequisites are unavailable.

**Evidence available:**
- [Firsthand] My Data Mining course experience and the effort to seek a solution.
- [Firsthand] A small group of students with a similar issue.
- [Observed] Complaints from other students and majors.
- [Unknown] The wider prevalence of the problem and the completeness and accessibility of university data.

**Reason for not selecting it now:** CoursePath had a reasonably clear problem and a defined prototype direction, but its usefulness depended on verifying university study-plan and offering data. I chose to prioritize a different problem that is directly connected to an accessible family environment and a potential real-world user.

**Important note:** This does not mean the CoursePath problem is solved or invalid. It remains a documented project idea that could be revisited later.

### 3. Heart Care

**Problem area:** Potential AI support for people with heart-related care needs.

**Evidence available:**
- [Firsthand] Personal motivation to explore this area.
- [Unknown] A specific daily problem, a clearly defined user, current coping methods, and access to patients or professionals for validation.

**Reason for not selecting it now:** The actual user problem is still insufficiently defined, and a health-related tool has higher safety requirements. An eight-week solo project should not make medical claims or risk being mistaken for diagnosis or treatment advice.

## Decision

**Selected direction: Agriculture / Nursery Management.**

The project will explore an AI-powered assistant for plant identification, visible condition assessment, care guidance, and individual plant history.

Reasons for the decision:
1. The nursery is a real environment I can understand and observe.
2. My father is an identifiable potential primary user.
3. The workflow includes repeated tasks that can be studied and narrowed into a prototype.
4. Public image datasets may support an initial machine-learning experiment.
5. A limited live demo may be possible without buying sensors or other equipment.

## What this decision does not prove

- It does not prove that the nursery's problems are common across other nurseries.
- It does not prove that AI will improve plant health or reduce costs.
- It does not prove that suitable datasets exist for the exact plants and conditions in this nursery.
- It does not prove that automatic identification of individual pots will work.
- It does not mean that the system is ready for real operational use.

## Decision status

- **Current project direction:** Agriculture / Nursery Management.
- **Previous project:** CoursePath, retained as historical.
- **Transportation:** Retained only in the original V1–V3 historical comparison; it is not one of the three candidates in this new comparison.
- **Heart Care:** Not selected for this mentorship project.
- **Next step:** Understand the nursery's actual workflow and define a realistic problem before committing to technical features.

---

# V8 — Nursery Problem Discovery

**Stage:** Understand the nursery, its users, current workflow, and recurring difficulties.  
**Date:** November 2026  
**Interview format:** One question at a time.  
**Documentation note:** Answers below are summarized from the discussion. They are not presented as verbatim transcripts.

## Prompt given to the AI mentor

> **Documentation note:** Reconstructed summary, not a verbatim prompt.
>
> Help me understand the real workflow and problems in my family's nursery before designing the AI solution.
>
> Ask one question at a time. Focus on:
>
> - The nursery's size and layout.
> - Who works there and who makes care decisions.
> - How often the owner visits.
> - What tasks take the most time.
> - How plant problems are identified and handled.
> - How watering decisions are made.
> - What happens when the owner is absent.
> - Which problems are firsthand observations and which are assumptions.
>
> Do not jump into coding or assume that every problem needs AI.

## Nursery context

### Environment

- The nursery is medium-sized, not extremely large or very small.
- It includes one greenhouse and plants or seedlings arranged around it.
- Most plants are kept in pots rather than planted directly in the ground.
- [Firsthand / Observed] This description is based on the family's nursery environment.

### People and responsibilities

- My father is the main person responsible for the nursery.
- A worker may be present when my father is absent.
- The worker does not have the same agricultural experience and generally follows instructions given by my father.
- Sometimes the worker arrives late or postpones tasks.
- [Observed] The worker's role and level of experience are based on what I know about the nursery.

### Owner's visits

- My father may not be able to visit every day.
- There is no fixed daily schedule.
- He usually visits and stays for a long period, often from the morning into the afternoon or evening.
- [Observed] This describes the current routine, not a guaranteed schedule.

### Existing monitoring

- A camera is available in the nursery.
- Sometimes it stops working because of battery or charging issues, or because the internet connection is lost.
- It is therefore not a fully reliable continuous monitoring solution.

## Current workflow and time-consuming tasks

The tasks that take time include:

1. Inspecting plants.
2. Identifying problems and deciding how to treat them.
3. Watering.
4. Cleaning.
5. Arranging plants.
6. Moving pots.
7. Following up on plant condition.
8. Monitoring whether the worker has completed assigned tasks.

The time required varies. No formal time measurements have been collected.

## Current ways of handling plant problems

When a plant appears unhealthy or behaves unusually, possible responses include:

- Using vitamins or nutrients, even when the plant may not need them.
- Asking another person for advice, although that person may not be available.
- Relying on personal experience, which may not always be sufficient.
- Watering the plant based on the assumption that it lacks water.
- Watching videos or searching for information about the plant.

These are reported current practices and possible workarounds, not evidence that every treatment is wrong.

## Watering workflow

- My father generally waters the nursery when he visits.
- He may water the nursery broadly rather than assessing the water requirement of every individual pot.
- The nursery may receive a large amount of water during this process.
- [Observed] This is the current practice as described.
- [Unknown] The exact amount of water used, how often overwatering occurs, and whether measurable damage or waste results from it.

## Potential consequences

The concerns identified during discovery include:

- A plant may die if its actual problem is not recognized.
- An unsuitable treatment may make the condition worse.
- A disease may spread if it is not identified and managed appropriately.
- Water or nutrients may be used unnecessarily.
- The owner may spend additional time checking plants or seeking advice.

These are potential risks, not measured outcomes. No confirmed financial loss or disease-spread incident has been established in this interview.

## Evidence summary

| Statement | Evidence label | Status |
|---|---|---|
| The nursery is medium-sized and has one greenhouse | [Firsthand / Observed] | Described |
| Most plants are in pots | [Firsthand / Observed] | Described |
| Father is the main nursery manager | [Firsthand / Observed] | Described |
| A worker sometimes helps | [Observed] | Described |
| The worker has limited agricultural experience | [Observed] | Described |
| The camera sometimes loses power or internet | [Observed] | Described |
| Inspection and care tasks take time | [Observed] | Described |
| Plant treatment decisions can involve uncertainty | [Observed] | Described |
| Broad watering is part of the current routine | [Observed] | Described |
| The system will reduce losses or water use | [Assumption] | Not demonstrated |
| The problem occurs at a measurable frequency | [Unknown] | Not measured |

## Initial problem statement

The nursery owner needs to monitor and care for many individual potted plants. Inspecting plants, identifying visible problems, deciding on suitable care, and following up on changes take time and may involve uncertainty, especially when the owner is absent or another worker has to follow instructions.

A potential digital assistant could help organize observations and provide cautious, evidence-based guidance for individual plants.

## Important unknowns

- How many plants are in the nursery?
- Which plant types are most common?
- Which plant types are most important to the owner?
- Which problems occur most often?
- How frequently does the owner inspect each plant?
- How are plants currently distinguished and tracked?
- How often are plants moved?
- How does the owner decide whether a plant needs water?
- Which plant problems can be recognized reliably from photographs?
- What information would the owner need before trusting a recommendation?
- How much time could the system realistically save?

---

# V9 — Define the User Requirements and Individual Plant Records

**Stage:** Clarify the intended user experience and how the system should track individual plants.  
**Date:** November 2026  
**Documentation note:** The following records summarize the actual discussion and decisions; they are not verbatim question-and-answer transcripts.

## Prompt given to the AI mentor

> **Documentation note:** Reconstructed summary, not a verbatim prompt.
>
> Based on the nursery workflow, help me define what the owner should be able to do with the system.
>
> I want to explore a system that:
>
> - Identifies the plant type from a photograph.
> - Assesses visible plant condition.
> - Suggests possible causes and care steps.
> - Helps assess whether watering may be needed.
> - Keeps a separate history for each individual plant.
> - Allows the owner to ask follow-up questions in a conversational interface.
> - Can retrieve previous observations even when the user starts a new conversation.
>
> Ask clarifying questions one at a time. Do not assume that identifying a plant species and identifying an individual pot are the same problem.

## Confirmed user requirements

### 1. Plant identification

The system should attempt to identify the full plant type from a photograph, not only give a generic plant category.

The father already has experience recognizing plant types, so the system's identification should be treated as assistance and should allow uncertainty or correction.

### 2. One plant per analysis

- Each submitted photograph should focus on one plant.
- The system should not be designed around identifying many different plants in one image.
- This helps keep the analysis and plant history associated with a single subject.

### 3. Condition assessment

The system should attempt to assess visible signs of plant condition and identify possible issues.

Potential outputs include:
- A description of visible symptoms.
- Possible explanations.
- A confidence or uncertainty indication.
- Suggested next steps.
- A request for another photograph or more information when the image is insufficient.

The system must not present an uncertain image-based prediction as a confirmed diagnosis.

### 4. Watering assessment

The system should help the owner consider whether a plant may need water.

However, a photograph alone cannot directly measure soil moisture. The system may need additional information, such as:
- Whether the soil feels dry or wet.
- When the plant was last watered.
- The plant type.
- The plant's location and exposure.
- Other relevant observations.

The feature must therefore be described as an estimate or decision-support feature, not an exact measurement.

### 5. Written conversational assistant

The system should not return only a static classification result.

The owner should be able to ask questions and receive written responses, such as:
- What is this plant?
- What could be causing these symptoms?
- What should I check next?
- Does it appear to need water?
- What should I do now?
- What changed compared with the previous observation?

The assistant should ask follow-up questions when necessary instead of guessing.

### 6. Individual plant history

- The system should preserve a record for each individual plant.
- Two pots containing the same plant type must not automatically share one history.
- Each pot should have its own observations and follow-up history.
- The system should retain previous records so later observations can be compared with earlier ones.

### 7. Automatic identification / generated ID

The user does not want the owner to manually enter a plant ID or scan a QR code every time.

The desired workflow is for the system to generate an ID automatically when a plant is first registered.

However, assigning an ID is different from reliably recognizing the same physical pot in later photographs. Automatic matching across photographs is a technical challenge and must be tested.

If reliable matching cannot be achieved, the system may need a simple confirmation step rather than silently assigning an observation to the wrong plant.

### 8. Persistent memory across conversations

The user wants the assistant to remember the plant's previous information even if the owner opens a new conversation.

This requires persistent application-level storage and retrieval of plant records. It should not depend only on the conversational model's temporary context.

### 9. Follow-up questions

The assistant should support questions referring to earlier observations, such as:

- "شو صار على هاي النبتة؟"
- "هل تحسنت عن المرة الماضية؟"
- "شو كان عندها قبل؟"
- "هل أعمل نفس العلاج؟"

The system must retrieve the correct individual plant record before answering.

## Important technical distinction

The project contains separate tasks:

1. Plant-type identification.
2. Visible condition or disease classification.
3. Watering-need assessment.
4. Conversational question handling.
5. Persistent individual plant records.
6. Matching a newly submitted photograph to an existing individual plant.

These tasks should not be treated as one model or assumed to be solved by one dataset.

## Decisions and limitations

- One plant per photograph.
- Separate records for separate pots, even when they contain the same plant type.
- Automatically generated IDs are preferred.
- Persistent records are required for follow-up questions.
- A written conversational interface is required.
- The system should ask for clarification when information is insufficient.
- Automatic matching must be tested; it is not yet a proven capability.

---

# V10 — Dataset Strategy and Trained Model Direction

**Stage:** Explore the data source and clarify the model-training requirement.  
**Date:** November 2026  
**Documentation note:** This section summarizes the discussion. It is not a record of completed dataset research or model training.

## Prompt given to the AI mentor

> **Documentation note:** Reconstructed summary, not a verbatim prompt.
>
> I want the project to include a model that I train myself. I do not want the final project to be only a ready-made chatbot.
>
> I plan to obtain image data from Kaggle.
>
> Help me distinguish the possible machine-learning tasks:
>
> - Plant-type classification.
> - Plant-condition or disease classification.
> - Any additional image-based task that might be realistic.
>
> Explain what must be checked in the datasets before choosing the model task. Do not assume that a dataset contains the plant types in my nursery or that it supports reliable diagnosis.
>
> Keep the plan realistic for one person working for eight weeks, with limited weekly hours and no additional paid services or hardware.

## Confirmed direction

- The user wants to train a model herself.
- Kaggle is the planned source for image datasets.
- The model should be connected to the nursery assistant rather than existing as an unrelated experiment.
- The exact dataset has not yet been selected.
- No model has been trained or evaluated.

## Separate model tasks

### A. Plant-type identification

Possible task: classify an image into one of the plant types represented in the selected dataset.

This is the initial candidate for the main image-classification model because the user explicitly wants the system to identify the plant type.

The final class list must depend on the dataset and the nursery's actual plant types.

### B. Plant-condition or disease classification

Possible task: classify visible conditions or disease categories if a suitable labelled dataset is available.

This is a separate task from plant-type identification. A dataset that identifies plant species does not automatically provide disease labels.

It must not be included as a guaranteed feature before the dataset is reviewed.

### C. Watering-need assessment

This is not automatically solved by either plant-type or disease classification.

A photograph may show visual signs associated with stress, but it cannot reliably measure the water content of the soil. This feature may need contextual questions and cautious decision logic rather than a standalone image classifier.

## Dataset inspection requirements

Before committing to a model, inspect:

1. Which plant types are included?
2. Which condition or disease labels are included?
3. How many images are available per class?
4. Are the labels clear and reliable?
5. Are there duplicate or near-duplicate images?
6. Are the images taken in varied lighting and backgrounds?
7. Do the images resemble photographs that could realistically be taken in the nursery?
8. Are some classes severely underrepresented?
9. What is the dataset license and what uses does it permit?
10. Is there a risk that images from the same original source appear in both training and test sets?
11. Does the dataset cover the plants that matter most in the nursery?

## Proposed approach

- Inspect available Kaggle datasets before selecting the final task.
- Select a manageable group of plant classes.
- Prepare labels and remove unsuitable or duplicate images where practical.
- Split the data carefully to avoid leakage.
- Train a lightweight image-classification model using available free resources.
- Evaluate it on held-out data.
- Report actual results and limitations.
- Test whether the model can handle photographs that differ from the dataset images.

## Current status

- **Planned data source:** Kaggle.
- **Dataset selected:** No.
- **Dataset license checked:** No.
- **Class balance inspected:** No.
- **Images cleaned:** No.
- **Model architecture selected:** No.
- **Model trained:** No.
- **Evaluation completed:** No.

These are future tasks, not completed results.

---

# V11 — Define the Project Scope and Feasibility

**Stage:** Establish a realistic project boundary for the eight-week mentorship.  
**Date:** November 5, 2026

## Prompt given to the AI mentor

> **Documentation note:** Reconstructed summary of the scope discussion, not a verbatim prompt.
>
> My current project direction is an AI-powered nursery assistant based on my family's plant nursery.
>
> The intended system should help the owner identify a plant from a photograph, assess its visible condition, receive cautious care guidance, and maintain a separate history for each individual plant.
>
> I want to train my own model using image data I plan to obtain from Kaggle.
>
> The assistant should support written conversations and retrieve previous records even when the user starts a new chat.
>
> The owner should not have to manually enter an ID every time. The system should generate plant IDs and, if technically possible, recognize previously registered individual plants.
>
> Constraints:
>
> - Eight weeks total.
> - One person working alone.
> - Approximately 3–8 hours of work between weekly mentorship sessions.
> - One AI subscription may be used.
> - No additional paid services.
> - No new sensors, cameras, or other hardware purchases.
> - The final project must be demonstrable live.
> - Do not claim that a dataset has been selected or a model trained.
> - Do not promise accurate disease diagnosis or exact watering decisions from images.
>
> Please define a realistic project scope, separate essential features from experimental features, identify risks, and explain what should be excluded if the project becomes too large.

## Project title

**AI-Powered Smart Nursery Assistant**

Working title only. A final brand or product name has not been selected.

## One-sentence concept

A digital assistant for nursery management that uses plant photographs, a trained image-classification model, contextual questions, and persistent individual plant records to help the owner identify plants, review visible conditions, and make more informed care decisions.

## Primary user

The primary intended user is my father, who manages the family nursery.

He is willing to try the prototype once it has demonstrated that it works reliably enough for him to trust testing it. This is conditional willingness, not evidence that he has already tested or approved the system.

## Problem statement

Managing the nursery involves repeated inspection, watering, treatment, cleaning, arranging, moving pots, and monitoring plants. Identifying visible problems and deciding what action a particular plant needs can involve uncertainty, especially when the owner is absent or another worker must follow instructions.

The proposed system aims to support the owner by organizing plant observations, identifying supported plant types, providing cautious guidance, and preserving the history of each individual plant.

## Proposed solution components

### 1. Trained plant-type image classifier

- Accept a photograph focused on one plant.
- Predict among the plant classes included in the selected dataset.
- Display the predicted class and an uncertainty indication where possible.
- Allow the user to correct an incorrect prediction.
- Do not claim support for every plant species.

### 2. Condition assessment

This feature is conditional on finding a suitable labelled dataset.

If the dataset supports it, the system may classify a limited set of visible conditions or disease categories.

The system must:
- Show possible results rather than claim a confirmed diagnosis.
- Communicate uncertainty.
- Ask for additional information where appropriate.
- Avoid recommending treatment beyond the evidence and scope of the prototype.

If suitable data is unavailable, this feature must be reduced or excluded.

### 3. Care guidance

The assistant may use the identified plant type, visible observations, and user-provided context to offer cautious next steps.

The system should distinguish:
- What is visible in the image.
- What the model predicts.
- What remains uncertain.
- What the owner should check next.

### 4. Watering support

Watering need may be considered using plant type, visible symptoms, soil observations, and watering history.

A photograph alone cannot measure soil moisture. The system must not claim that it can determine exact watering requirements from an image.

### 5. Individual plant records

- Each registered pot receives a generated ID.
- Each pot has a separate history.
- Different pots of the same plant type remain separate records.
- Previous observations can be retrieved and compared.
- The assistant can answer follow-up questions about a previously registered plant.

### 6. Conversational interface

The owner should be able to ask written questions and receive contextual responses.

Examples:
- "شو نوع هاي النبتة؟"
- "شو المشكلة اللي مبينة عليها؟"
- "هل ممكن تحتاج مي؟"
- "شو أعمل هسا؟"
- "شو صار على هاي النبتة من آخر مرة؟"

The assistant must retrieve the correct record before answering a question about a plant's history.

## What is essential for the first useful prototype

1. A small, selected set of plant classes.
2. A trained image-classification model.
3. A basic interface for submitting one plant photograph.
4. A result showing the predicted plant type and uncertainty.
5. A basic written assistant that explains the result and asks for missing context.
6. A persistent record for each registered plant.
7. A generated ID for each new plant record.
8. A way to retrieve and display previous observations for a selected plant.
9. A basic live demonstration using prepared example images and records.

## Experimental or conditional features

- Disease or condition classification, depending on dataset suitability.
- Watering-need assessment using image and contextual information.
- Automatic matching of a new photograph to a previously registered physical pot.
- More advanced conversational responses.
- Comparison of multiple observations over time.

These features should not be promised until they have been tested.

## Out of scope

The initial project will not attempt to provide:

- Identification of every plant species.
- Detection of every plant disease.
- Guaranteed diagnosis.
- Exact soil-moisture measurement from photographs.
- Guaranteed watering schedules.
- Automatic irrigation.
- IoT sensors or new hardware.
- Integration with the existing nursery camera.
- Continuous video monitoring.
- Automatic worker supervision.
- Full nursery inventory or accounting.
- Sales, purchasing, or customer-management systems.
- Guaranteed recognition of every individual pot from any photograph.
- Replacement of an agricultural specialist.

## Main technical risks

### 1. Dataset mismatch

Kaggle images may not resemble the plants, lighting, backgrounds, ages, or camera angles in the nursery.

**Fallback:** restrict the model to classes with sufficient data and clearly report the difference between dataset evaluation and real nursery performance.

### 2. Disease labels may be insufficient

A dataset may contain plant-type labels without reliable disease or condition labels.

**Fallback:** keep plant identification as the main trained task and remove disease classification from the first version.

### 3. Watering cannot be measured from an image alone

Visible symptoms may have several possible causes.

**Fallback:** ask contextual questions and present cautious guidance rather than a definitive watering decision.

### 4. Individual plant matching

A generated ID can identify a stored record, but it does not automatically prove that a new photograph shows the same physical pot.

**Fallback:** use a confirmation step or a simple record-selection workflow if automatic matching is unreliable.

### 5. Persistent records

The assistant needs an application-level storage mechanism to retrieve the correct plant history across separate sessions.

**Fallback:** implement a simple local database or structured record store before attempting advanced memory features.

### 6. Time constraints

The full project combines image classification, a conversational interface, persistent storage, and individual-plant matching.

**Fallback:** prioritize a trained plant classifier, one-plant submission, generated ID, and a basic persistent record. Reduce experimental features first.

## Feasibility verdict

**Realistic only with a carefully limited scope.**

A small trained plant-type classifier and a basic plant-record workflow appear more achievable than a complete nursery-management platform.

Disease classification, watering assessment, and automatic individual-plant matching should remain conditional until the data and implementation feasibility are tested.

The main feasibility question is not whether a chatbot can be built. It is whether the selected image data supports a useful trained model and whether the record system can reliably connect observations to individual pots.

## Success criteria (proposed, not yet achieved)

A successful limited demonstration should show:

1. A user submits a photograph of one plant.
2. The trained model returns a plant-type prediction within its supported classes.
3. The system displays uncertainty and does not force a confident answer when evidence is weak.
4. A new plant record is created with a generated ID.
5. A later observation can be attached to the correct plant record through the implemented workflow.
6. The assistant can retrieve the earlier observation and answer a follow-up question using stored information.

Disease and watering features should only be included in the success criteria if the relevant dataset and evaluation support them.

---

# Current Project Status — November 5, 2026

## Project direction

**Current project:** AI-Powered Smart Nursery Assistant.

**Previous project:** CoursePath, retained as historical documentation.

## Confirmed decisions

- Agriculture / Nursery Management is the current selected direction.
- The primary intended user is my father.
- The project is based on the family nursery.
- The system should identify supported plant types from photographs.
- Each analysis should focus on one plant.
- The user wants a trained model, not only a ready-made chatbot.
- Kaggle is the planned image-data source.
- The system should support a written conversational interface.
- Each individual pot should have its own record and history.
- Different pots of the same plant type must remain separate.
- Generated plant IDs are preferred over manual ID entry every time.
- Persistent history across separate conversations is required.
- The system should ask follow-up questions instead of guessing.
- My father is willing to try the prototype once it has demonstrated sufficient reliability.

## Proposed, not yet verified

- The exact plant classes to support.
- Whether a suitable Kaggle dataset exists.
- Whether disease or condition classification can be included.
- Whether watering support can be made useful with contextual information.
- Whether individual pots can be automatically matched across photographs.
- Whether the prototype will reduce the owner's workload.
- Whether the prototype will improve plant-care decisions.

## Work not yet completed

- Kaggle dataset selection.
- Dataset license review.
- Dataset inspection and cleaning.
- Plant-class selection.
- Model selection.
- Model training.
- Model evaluation.
- Persistent record implementation.
- Automatic plant-matching experiment.
- End-to-end prototype.
- Live testing with my father.
- Measurement of time saved or nursery outcomes.

## Next step

Review Kaggle datasets and compare them against the actual plant types and conditions in the nursery. Select the smallest defensible model task based on the available labels and image quality before finalizing the technical implementation.

---

# Change History

| Stage | Project direction | Status |
|---|---|---|
| V1 | Academic Planning, Transportation, Heart Care discovery | Historical |
| V2 | Comparison of the original three candidates | Historical |
| V3 | CoursePath selected | Superseded |
| V4 | CoursePath MVP defined | Historical |
| V5 | CoursePath feasibility and risks | Historical |
| V5 Addendum | CoursePath trained intent-classifier requirement | Historical |
| V6 | CoursePath final project definition | Historical |
| Language Policy Addendum | CoursePath language behaviour | Historical |
| V7 | Reconsider project selection; agriculture selected | Current pivot |
| V8 | Nursery problem discovery | Completed discussion summary |
| V9 | User requirements and individual plant records | Current requirements |
| V10 | Kaggle dataset and trained-model direction | Planned |
| V11 | Nursery assistant scope and feasibility | Current working scope |

**Final documentation rule:** Historical CoursePath records must remain intact. Future changes to the agriculture project should be appended as new dated stages or clearly identified amendments. Do not rewrite earlier stages to make it appear that the agriculture project was the original idea.

## Task 02 — BRD Critical Review

**Date:** November 5, 2026  
**Stage:** Skeptical Manager Review  
**Project:** Smart Nursery Assistant

### Prompt Given to the AI Mentor

Here is my BRD. Do not rewrite it.

Read it as the manager who has to approve it and who is sceptical.

List:
- What is unclear.
- What is assumed without evidence.
- What would make you refuse to fund it.

Then ask me the three questions you most need answered.

### Main Feedback Received

The AI mentor identified the following concerns:

1. The initial plant types and the number of supported categories are not yet defined.
2. Plant identification and plant condition assessment are separate AI tasks and require suitable datasets.
3. Agricultural recommendations need reliable sources and must avoid unsupported diagnoses.
4. Individual plant matching across different photographs may be unreliable.
5. Persistent plant records need a suitable storage solution.
6. The project may be too ambitious for an eight-week, individual development schedule.
7. The usefulness of the application has not yet been validated.
8. The project needs a clearer distinction from existing plant-care applications.

### Three Questions and My Answers

**Question 1: How will the project handle different data sources and evaluate the model?**

My answer:

I will separate training and testing data. I also plan to collect and reserve nursery photographs for local evaluation, so the model can be tested under actual nursery conditions. I will prioritize agricultural data from Jordan when available, or data covering plants commonly grown in Jordan. Additional nursery data will be collected when suitable public data is missing.

**Question 2: What happens if there is insufficient data for plant disease assessment?**

My answer:

I accept starting with plant identification and condition assessment for a limited number of categories supported by available data. Unsupported conditions will be left for future development rather than presented as reliable results.

**Question 3: How will the project demonstrate practical usefulness?**

My answer:

The main expected benefit is reducing the time spent searching websites and watching YouTube videos to find plant-care information. Instead, the user can ask the assistant directly and receive guidance in one place.

The benefit will be evaluated by comparing the time required to find relevant information using the current approach with the time required using the prototype. Task completion and the user's ability to understand the suggested next steps will also be considered.

### Additional Decisions Confirmed During the Review

- The application will support Arabic and English, with Arabic as the primary language.
- Android will be the primary target platform.
- The system will ask the user to confirm a plant match when image matching is uncertain.
- Plant selection will be based on dataset availability and relevance to Jordanian agriculture.
- The broader target audience includes Jordanian and Arab farmers, nursery owners, and early-stage agricultural entrepreneurs.

### Changes and Decisions

- Training and testing data will be kept separate.
- Nursery images reserved for local evaluation will not be used for training or model tuning.
- The condition assessment task will be limited to categories supported by suitable labeled data.
- The project will prioritize a reliable prototype over implementing every planned feature.
- Practical value will be evaluated through time comparison and task completion rather than assumed in advance.

### Disagreements

No major disagreement with the review findings was identified. The project owner accepted the need to reduce the model's scope if dataset quality or development time is insufficient.

### Review Outcome

**Conditional approval for prototype development.**

The project can proceed to research and implementation planning, provided that dataset suitability, model performance, and practical usefulness are evaluated before making broader claims.

**Status:** Review completed. The BRD remains subject to refinement based on competitor research and dataset investigation.