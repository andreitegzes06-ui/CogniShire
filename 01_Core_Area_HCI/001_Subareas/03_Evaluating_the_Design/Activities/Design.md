---
title: Design
area: Evaluating the Design
category: Activities
cs2023_unit: HCI-Evaluation
cssclasses:
  - observation-chamber
tags:
  - HCI
  - CS2023
  - HCI-Evaluation
  - evaluation-design
  - usability-testing
  - protocol-design
  - task-design
  - metrics
  - instruments
  - rubrics
  - study-materials
  - accessibility-evaluation
status: expanded-polished-draft
---
![[como.jpg|1000]]
# Design

Back to [[../Overview|The Observation Chamber]].

> [!abstract] Protocol Design Table
> Design in the Observation Chamber means designing the evaluation itself: the protocol, tasks, instruments, metrics, rubrics, participant materials, consent language, accessibility checks, and analysis plan. A weak protocol produces weak evidence, even when the interface being tested is interesting.

The fantasy name is **Protocol Design Table**.  
The real CS2023 label is **HCI-Evaluation: Evaluating the Design**.  
The real-life meaning is **planning an evaluation before collecting data so the study can produce clear, ethical, and defensible findings**.


> [!quote] Protocol rule
> A study does not become rigorous because it uses many metrics. It becomes rigorous when every task, measure, and instrument serves the evaluation question.

## Protocol Map

```mermaid
flowchart TB
    A((Protocol Design Table))

    A --> B[Evaluation Question]
    A --> C[Task Script]
    A --> D[Method Choice]
    A --> E[Instrument Kit]
    A --> F[Metric Board]
    A --> G[Analysis Plan]

    B --> B1[What must be learned]
    C --> C1[What users must do]
    D --> D1[How evidence is collected]
    E --> E1[Surveys, rubrics, notes]
    F --> F1[What is measured]

    classDef center fill:#d8d7ff,stroke:#8b5cf6,color:#05051a,stroke-width:3px;
    classDef station fill:#101022,stroke:#8b5cf6,color:#ffffff,stroke-width:2px;
    classDef detail fill:#5b2aa8,stroke:#d6a64f,color:#ffffff,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G station;
    class B1,C1,D1,E1,F1,G1 detail;
```

| Protocol part | Real-life meaning | Weak version |
|---|---|---|
| Evaluation question | The specific thing the study must learn | “Is the design good?” |
| Task script | A realistic goal given to the participant | “Click this button.” |
| Method choice | Usability test, experiment, interview, survey, heuristic evaluation, log study, or mixed method | Choosing a method because it sounds academic |
| Instrument kit | Consent text, script, note sheet, survey, scale, checklist, rubric | Random questions after the test |
| Metric board | Task success, time, errors, confidence, satisfaction, workload, accessibility checks | Collecting numbers without interpretation |
| Analysis plan | How data becomes findings and design implications | Looking at results only after the study and guessing |

## CS2023 Design Grounding

CS2023 HCI-Evaluation includes methods for evaluation with users, formative and summative assessment, usability testing, qualitative and quantitative methods, surveys, interviews, focus groups, observation, study planning, hypothesis design, heuristic evaluation, and drawing defensible conclusions.

Designing an evaluation protocol is therefore not a side activity. It is part of the CS2023 skill itself.

```mermaid
flowchart TB
    A((CS2023 Evaluation Design))

    A --> B[Study Planning]
    A --> C[Hypothesis Design]
    A --> D[Method Selection]
    A --> E[Data Collection]
    A --> F[Defensible Conclusion]

    B --> B1[Protocol before testing]
    C --> C1[Expected relation]
    D --> D1[Match method to question]
    E --> E1[Collect usable evidence]

    classDef center fill:#d8d7ff,stroke:#8b5cf6,color:#05051a,stroke-width:3px;
    classDef stage fill:#101022,stroke:#8b5cf6,color:#ffffff,stroke-width:2px;
    classDef detail fill:#5b2aa8,stroke:#d6a64f,color:#ffffff,stroke-width:2px;

    class A center;
    class B,C,D,E,F stage;
    class B1,C1,D1,E1,F1 detail;
```

| CS2023 evaluation element | Protocol design translation |
|---|---|
| Formative assessment | Design a study that finds problems and improves the interface |
| Summative assessment | Design a study that judges a stable interface against criteria |
| Functionality and usability testing | Create tasks that reveal whether the system works and is usable |
| Utility, efficiency, learnability, satisfaction | Select metrics and instruments that match each construct |
| Qualitative methods | Prepare observation notes, interview questions, and coding categories |
| Quantitative methods | Define variables, measures, comparison logic, and data recording |
| Heuristic evaluation | Prepare evaluator instructions, heuristics, severity ratings, and issue templates |

## The Evaluation Question Gate

The Evaluation Question Gate is the first protocol decision. A vague question creates vague evidence. A good question identifies the interface, users, task, context, and outcome.

```mermaid
flowchart TB
    A((Evaluation Question))

    A --> B[Interface]
    A --> C[Users]
    A --> D[Task]
    A --> E[Context]
    A --> F[Outcome]

    B --> B1[What is tested]
    C --> C1[Who uses it]
    D --> D1[What goal they attempt]
    E --> E1[Where and how use happens]
    F --> F1[What evidence matters]

    classDef center fill:#d8d7ff,stroke:#8b5cf6,color:#05051a,stroke-width:3px;
    classDef part fill:#101022,stroke:#8b5cf6,color:#ffffff,stroke-width:2px;
    classDef detail fill:#5b2aa8,stroke:#d6a64f,color:#ffffff,stroke-width:2px;

    class A center;
    class B,C,D,E,F part;
    class B1,C1,D1,E1,F1 detail;
```

| Weak question | Stronger evaluation question |
|---|---|
| Is the map easy to use? | Can first-year students find the correct HCI room and explain its CS2023 meaning within three minutes? |
| Is the interface nice? | Does the visual hierarchy help users identify the main action without hesitation? |
| Is the form good? | Can users complete the form, understand validation messages, and recover from errors without help? |
| Is the page accessible? | Can keyboard and screen reader users navigate the page, identify headings, and operate controls? |
| Is version B better? | Does version B reduce wrong turns compared with version A for the same navigation task? |

NN/g describes usability testing tasks as realistic activities participants might perform in real life. This matters because the evaluation question should be grounded in real use, not in artificial button-clicking.

## The Method Selection Compass

A protocol must choose the method that fits the question. The wrong method can produce data, but not useful evidence.

```mermaid
flowchart TB
    A((Method Selection))

    A --> B[Find usability problems]
    A --> C[Compare versions]
    A --> D[Understand meaning]
    A --> E[Inspect principles]
    A --> F[Check accessibility]
    A --> G[Study real use]

    B --> B1[Usability test]
    C --> C1[Controlled experiment]
    D --> D1[Interview or field study]
    E --> E1[Heuristic evaluation]
    F --> F1[Accessibility evaluation]
    G --> G1[Field or log study]

    classDef center fill:#d8d7ff,stroke:#8b5cf6,color:#05051a,stroke-width:3px;
    classDef need fill:#101022,stroke:#8b5cf6,color:#ffffff,stroke-width:2px;
    classDef method fill:#2a1b10,stroke:#d6a64f,color:#ffffff,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G need;
    class B1,C1,D1,E1,F1,G1 method;
```

| Evaluation need | Best method family | Why |
|---|---|---|
| Discover interface breakdowns | Moderated usability test | Shows behaviour, confusion, and recovery |
| Compare two design alternatives | Controlled experiment or A/B comparison | Supports condition-based comparison |
| Understand user context | Interview, diary, or field study | Reveals meaning, motivation, and environment |
| Find obvious usability issues quickly | Heuristic evaluation | Uses expert inspection before user testing |
| Evaluate learnability | Cognitive walkthrough or first-use test | Focuses on step-by-step understanding |
| Check accessibility | WCAG review, keyboard test, screen reader check, user testing with disabled participants | Evaluates inclusion beyond average use |
| Study large-scale usage | Product analytics or log study | Reveals patterns at scale, but not always reasons |

NN/g’s UX research method guidance is useful here because it distinguishes methods by purpose, such as discovery, validation, behavioural observation, attitudinal data, qualitative insight, and quantitative measurement.

## The Task Script Forge

Task design is one of the most important parts of an evaluation protocol. The task should give a goal, not instructions for how to use the interface. If the task tells users exactly what to click, the test no longer evaluates navigation or discoverability.

```mermaid
sequenceDiagram
    participant R as Researcher
    participant U as Participant
    participant I as Interface
    participant N as Notes

    R->>U: Gives goal-based task
    U->>I: Attempts task
    I-->>U: Shows feedback
    R->>N: Records behaviour
    U-->>R: Explains interpretation
```

| Bad task | Better task |
|---|---|
| Click the “Theory” link. | Find the page that explains the concepts behind evaluation. |
| Press the submit button. | You finished filling the form. Make sure your answer is saved. |
| Open the accessibility section. | Find one check that would help a screen reader user. |
| Use the search bar. | Find where this vault explains design-system scalability. |
| Click the breadcrumb. | Return to the room overview from this page. |

A strong task should be realistic, short enough to understand, and open enough to reveal the user’s strategy. It should not hide the answer inside the wording.

## The Moderator Script

A moderated usability test needs a script so participants receive the same setup. The script protects consistency and reduces accidental hints.

```mermaid
flowchart TB
    A((Moderator Script))

    A --> B[Greeting]
    A --> C[Consent]
    A --> D[Context]
    A --> E[Task]
    A --> F[Think-aloud reminder]
    A --> G[Debrief]

    B --> B1[Set tone]
    C --> C1[Explain rights]
    D --> D1[Explain test purpose]
    E --> E1[Give goal]
    F --> F1[Ask for thoughts]
    G --> G1[Ask final questions]

    classDef center fill:#d8d7ff,stroke:#8b5cf6,color:#05051a,stroke-width:3px;
    classDef step fill:#101022,stroke:#8b5cf6,color:#ffffff,stroke-width:2px;
    classDef detail fill:#5b2aa8,stroke:#d6a64f,color:#ffffff,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G step;
    class B1,C1,D1,E1,F1,G1 detail;
```

| Script part | Example wording |
|---|---|
| Greeting | “Thank you for helping me test this learning interface.” |
| Non-blame framing | “We are testing the design, not you.” |
| Consent | “You can stop at any time and skip any question.” |
| Think-aloud instruction | “Please say what you are looking for and what you expect to happen.” |
| Neutral help rule | “I may ask what you are thinking, but I will not guide you unless you are stuck for too long.” |
| Debrief | “What felt clear, what felt confusing, and what would you change?” |

NN/g describes thinking aloud as a simple and powerful usability method because it reveals what users think while interacting. It must still be handled carefully: the moderator should encourage explanation without leading the participant.

## The Instrument Kit

The Instrument Kit is the set of materials used to collect evidence. It may include a consent form, participant screener, task sheet, observation form, post-task questionnaire, post-study questionnaire, accessibility checklist, issue log, severity rubric, and debrief questions.

```mermaid
flowchart TB
    A((Instrument Kit))

    A --> B[Consent Form]
    A --> C[Task Sheet]
    A --> D[Observation Form]
    A --> E[Questionnaire]
    A --> F[Accessibility Checklist]
    A --> G[Issue Log]

    B --> B1[Ethical permission]
    C --> C1[What participant does]
    D --> D1[What researcher records]
    E --> E1[What participant reports]
    F --> F1[Access checks]
    G --> G1[Problems and severity]

    classDef center fill:#d8d7ff,stroke:#8b5cf6,color:#05051a,stroke-width:3px;
    classDef tool fill:#101022,stroke:#8b5cf6,color:#ffffff,stroke-width:2px;
    classDef purpose fill:#5b2aa8,stroke:#d6a64f,color:#ffffff,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G tool;
    class B1,C1,D1,E1,F1,G1 purpose;
```

| Instrument | What it should contain |
|---|---|
| Consent form | Purpose, recording, voluntary participation, privacy, withdrawal |
| Screener | Participant type, experience level, accessibility needs, device context |
| Task sheet | Goal-based tasks, not step-by-step instructions |
| Observation form | Time, success, errors, hesitation, quotes, unexpected behaviour |
| Post-task scale | Difficulty, confidence, satisfaction, workload, depending on the question |
| Post-study scale | SUS, UEQ, or custom global ratings when appropriate |
| Accessibility checklist | Keyboard, focus, contrast, labels, headings, screen reader checks |
| Issue log | Problem, evidence, severity, likely cause, design implication |

A good instrument kit makes the study reproducible. Another person should be able to run the same evaluation and collect comparable evidence.

## The Metric Board

The Metric Board defines what will be counted, rated, or judged.

```mermaid
flowchart TB
    A((Metric Board))

    A --> B[Task Success]
    A --> C[Time]
    A --> D[Errors]
    A --> E[Self-report]
    A --> F[Accessibility]
    A --> G[Qualitative Notes]

    B --> B1[Complete, partial, failed]
    C --> C1[Time on task]
    D --> D1[Wrong paths and mistakes]
    E --> E1[SUS, TLX, confidence]
    F --> F1[Keyboard, screen reader, contrast]
    G --> G1[Quotes and observations]

    classDef center fill:#d8d7ff,stroke:#8b5cf6,color:#05051a,stroke-width:3px;
    classDef metric fill:#101022,stroke:#8b5cf6,color:#ffffff,stroke-width:2px;
    classDef detail fill:#5b2aa8,stroke:#d6a64f,color:#ffffff,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G metric;
    class B1,C1,D1,E1,F1,G1 detail;
```

| Metric | Definition example | Interpretation caution |
|---|---|---|
| Task success | Complete, partial, failed | Success does not prove low effort |
| Time on task | Seconds from task start to completion | Fast can mean efficient or careless |
| Error count | Wrong clicks, invalid submissions, route errors | Errors need cause analysis |
| Assistance needed | No help, minor prompt, major help | Help from moderator can invalidate task success |
| Confidence rating | User rates confidence after task | Confidence may be wrong |
| SUS | Global perceived usability after using the system | Does not identify exact problems |
| NASA-TLX | Perceived workload after task | Workload score does not tell what to fix |
| Accessibility check | Keyboard path, focus order, contrast, labels | Automated checks are not enough |

MeasuringU recommends combining study-level and task-based UX metrics when quantifying product or interface experience. NN/g also explains that perceived-usability instruments such as SUS and workload instruments such as NASA-TLX can support evaluation, but they should be paired with behavioural evidence.

## The Rubric Wall

The Rubric Wall turns subjective judgement into a structured assessment. It is useful for heuristic evaluation, severity rating, prototype comparison, accessibility review, and student project grading.

```mermaid
flowchart TB
    A((Rubric Wall))

    A --> B[Criterion]
    A --> C[Level]
    A --> D[Evidence]
    A --> E[Decision]

    B --> B1[What is judged]
    C --> C1[Scale or category]
    D --> D1[What supports score]
    E --> E1[What changes next]

    classDef center fill:#d8d7ff,stroke:#8b5cf6,color:#05051a,stroke-width:3px;
    classDef part fill:#101022,stroke:#8b5cf6,color:#ffffff,stroke-width:2px;
    classDef detail fill:#5b2aa8,stroke:#d6a64f,color:#ffffff,stroke-width:2px;

    class A center;
    class B,C,D,E part;
    class B1,C1,D1,E1 detail;
```

| Criterion | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| Task clarity | Task cannot be understood | Task is vague | Task is mostly clear | Task is realistic and goal-based |
| Feedback visibility | No feedback | Feedback appears but is unclear | Feedback is visible | Feedback clearly explains state and next step |
| Error recovery | No repair path | Repair is hidden | Repair is possible | Repair is clear, local, and respectful |
| Navigation | User cannot orient | Some routes are unclear | Main routes are usable | Location, routes, and return paths are clear |
| Accessibility | Major barriers | Some basic access | Mostly accessible | Keyboard, focus, labels, contrast, and semantics are checked |

NN/g severity ratings are useful for prioritising usability problems. A severity rubric should include impact, frequency, and persistence. A cosmetic issue is not the same as a problem that blocks task completion or excludes users.

## Accessibility Evaluation Plan

Accessibility must be designed into the evaluation protocol, not added only if time remains. W3C describes accessibility evaluation as assessment, audit, and testing. WCAG 2.2 provides testable success criteria under perceivable, operable, understandable, and robust principles.

```mermaid
flowchart TB
    A((Accessibility Plan))

    A --> B[Scope]
    A --> C[WCAG Review]
    A --> D[Keyboard Test]
    A --> E[Screen Reader Check]
    A --> F[User Evidence]

    B --> B1[Pages, states, components]
    C --> C1[Success criteria]
    D --> D1[Focus and operation]
    E --> E1[Labels and structure]
    F --> F1[Disabled users when possible]

    classDef center fill:#d8d7ff,stroke:#8b5cf6,color:#05051a,stroke-width:3px;
    classDef check fill:#101022,stroke:#8b5cf6,color:#ffffff,stroke-width:2px;
    classDef detail fill:#5b2aa8,stroke:#d6a64f,color:#ffffff,stroke-width:2px;

    class A center;
    class B,C,D,E,F check;
    class B1,C1,D1,E1,F1 detail;
```

| Accessibility protocol item | What to specify |
|---|---|
| Scope | Which pages, states, components, and breakpoints are checked |
| Standard | Which WCAG version and level are used |
| Keyboard path | Which task is completed without mouse |
| Focus review | Whether focus order, focus visibility, and focus traps are checked |
| Screen reader check | Which screen reader/browser combination is used |
| Contrast check | Which text and UI elements are tested |
| Error check | Whether users can identify and recover from errors |
| Reporting | Issue, evidence, affected users, severity, repair recommendation |

W3C’s WCAG-EM provides a structured methodology for evaluating conformance to WCAG. For a student project, the full methodology may be too heavy, but the logic is useful: define scope, explore the target, select samples, audit selected items, and report findings clearly.

## Study Materials Pack

A complete evaluation should have a small pack of materials.

```mermaid
flowchart TB
    A((Study Materials Pack))

    A --> B[Protocol]
    A --> C[Participant Script]
    A --> D[Task List]
    A --> E[Data Sheet]
    A --> F[Questionnaires]
    A --> G[Report Template]

    B --> B1[Whole study plan]
    C --> C1[What researcher says]
    D --> D1[What participant attempts]
    E --> E1[What is recorded]
    F --> F1[What participant rates]
    G --> G1[How findings are written]

    classDef center fill:#d8d7ff,stroke:#8b5cf6,color:#05051a,stroke-width:3px;
    classDef item fill:#101022,stroke:#8b5cf6,color:#ffffff,stroke-width:2px;
    classDef purpose fill:#5b2aa8,stroke:#d6a64f,color:#ffffff,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G item;
    class B1,C1,D1,E1,F1,G1 purpose;
```

| Material | Minimum content |
|---|---|
| Protocol | Purpose, research question, participants, method, tasks, metrics, analysis plan |
| Participant script | Introduction, consent, non-blame statement, think-aloud instruction, closing |
| Task list | Goal-based tasks with success criteria |
| Observation sheet | Time, success, errors, hesitation, quotes, assistance, notes |
| Questionnaire | Post-task and post-study ratings |
| Accessibility checklist | Keyboard, focus, screen reader, contrast, labels, headings |
| Issue log | Issue, evidence, severity, affected task, design recommendation |
| Report template | Method, participants, findings, limitations, recommendations |

## Analysis Plan

The analysis plan should be written before data collection. It prevents the researcher from inventing interpretations after seeing results.

```mermaid
flowchart TB
    A((Analysis Plan))

    A --> B[Clean Data]
    A --> C[Summarise Metrics]
    A --> D[Code Observations]
    A --> E[Rate Severity]
    A --> F[Write Findings]

    B --> B1[Check completeness]
    C --> C1[Success, time, errors]
    D --> D1[Patterns and themes]
    E --> E1[Prioritise problems]
    F --> F1[Evidence + implication]

    classDef center fill:#d8d7ff,stroke:#8b5cf6,color:#05051a,stroke-width:3px;
    classDef step fill:#101022,stroke:#8b5cf6,color:#ffffff,stroke-width:2px;
    classDef detail fill:#5b2aa8,stroke:#d6a64f,color:#ffffff,stroke-width:2px;

    class A center;
    class B,C,D,E,F step;
    class B1,C1,D1,E1,F1 detail;
```

| Data type | Analysis action |
|---|---|
| Task success | Count complete, partial, failed attempts |
| Time | Summarise cautiously, especially with small samples |
| Errors | Group by interface location and likely cause |
| Think-aloud comments | Extract quotes that explain confusion or expectation |
| Questionnaire ratings | Report scale, timing, and what the score means |
| Accessibility issues | Map issue to WCAG criterion or user impact |
| Observed behaviour | Convert repeated patterns into findings |
| Findings | Connect evidence to design implication |

A finding should follow this pattern:

| Finding part | Example |
|---|---|
| Problem | Users did not understand the room names. |
| Evidence | Three participants opened the wrong room first and asked what “Forge” meant. |
| Explanation | The metaphor was memorable but not self-explanatory. |
| Design implication | Add the CS2023 label and real-life translation near the room title. |

## Ethics and Consent Station

Evaluation design must include ethics. Even a small student usability test should explain the purpose, avoid pressure, protect privacy, and avoid making the participant feel judged.

```mermaid
stateDiagram-v2
    [*] --> Purpose
    Purpose --> Consent
    Consent --> Participation
    Participation --> Privacy
    Privacy --> Debrief
    Debrief --> [*]

    Purpose: Explain study goal
    Consent: Voluntary agreement
    Participation: User can stop
    Privacy: Data handled carefully
    Debrief: Explain and thank
```

| Ethical protocol item | Why it matters |
|---|---|
| Non-blame statement | Participants know the design is being tested, not their intelligence |
| Voluntary participation | Participants can refuse or stop |
| Minimal data | Researcher collects only what is needed |
| Recording permission | Participants know if audio, video, or screen activity is captured |
| Anonymisation | Report does not expose unnecessary identity |
| Accessibility accommodation | Participants can use needed tools and adjustments |
| Debrief | Participants understand what the study was about |

## Mini Protocol: Testing Cognishire Navigation

This mini protocol applies the page to the HCI vault itself.

| Protocol field | Decision |
|---|---|
| Evaluation question | Can first-year students navigate from the five-room overview to the System Design and Evaluation rooms and explain what each room means? |
| Method | Moderated usability test with think-aloud |
| Participants | Three to five students unfamiliar with the vault |
| Task one | Find the room that explains how interfaces are built |
| Task two | Find the room that explains how interfaces are evaluated |
| Task three | Find one official CS2023 source link |
| Metrics | Task success, wrong turns, time, assistance, confidence |
| Qualitative notes | What users say they expect each room name to mean |
| Accessibility check | Keyboard-only navigation through the same route |
| Output | Navigation, wording, diagram, and source-link improvements |

```mermaid
flowchart TB
    A((Cognishire Protocol))

    A --> B[Find room]
    A --> C[Explain meaning]
    A --> D[Find source]
    A --> E[Check access]
    A --> F[Revise map]

    B --> B1[Navigation evidence]
    C --> C1[Comprehension evidence]
    D --> D1[Credibility evidence]
    E --> E1[Accessibility evidence]
    F --> F1[Design implication]

    classDef center fill:#d8d7ff,stroke:#8b5cf6,color:#05051a,stroke-width:3px;
    classDef task fill:#101022,stroke:#8b5cf6,color:#ffffff,stroke-width:2px;
    classDef evidence fill:#5b2aa8,stroke:#d6a64f,color:#ffffff,stroke-width:2px;

    class A center;
    class B,C,D,E,F task;
    class B1,C1,D1,E1,F1 evidence;
```

## Protocol Checklist

| Check | Question |
|---|---|
| Research question | Is the evaluation question specific enough? |
| Method | Does the method match the question? |
| Tasks | Are tasks realistic and goal-based? |
| Metrics | Does each metric measure something relevant? |
| Instruments | Are scripts, sheets, and questionnaires prepared? |
| Accessibility | Is keyboard, focus, contrast, and assistive technology considered? |
| Ethics | Is consent, privacy, and non-blame framing included? |
| Analysis | Is there a plan for turning evidence into findings? |

## Academic Anchors

| Route | Source |
|---|---|
| CS2023 HCI Evaluation basis | [CS2023 HCI Version Gamma](https://csed.acm.org/wp-content/uploads/2023/09/HCI-Version-Gamma.pdf) |
| Usability framework | [ISO 9241-11](https://www.iso.org/obp/ui/) |
| Usability testing basics | [NN/g: Usability Testing 101](https://www.nngroup.com/articles/usability-testing-101/) |
| Thinking aloud | [NN/g: Thinking Aloud: The #1 Usability Tool](https://www.nngroup.com/articles/thinking-aloud-the-1-usability-tool/) |
| UX method selection | [NN/g: Which UX Research Methods to Use](https://www.nngroup.com/articles/which-ux-research-methods/) |
| UX research cheat sheet | [NN/g: UX Research Cheat Sheet](https://www.nngroup.com/articles/ux-research-cheat-sheet/) |
| Measuring perceived usability | [NN/g: Measuring Perceived Usability](https://www.nngroup.com/articles/measuring-perceived-usability/) |
| Task-based UX metrics | [MeasuringU: Task-Based UX Metrics](https://measuringu.com/task-based-metrics/) |
| System Usability Scale | [Brooke: SUS, A Quick and Dirty Usability Scale](https://digital.ahrq.gov/sites/default/files/docs/survey/systemusabilityscale%28sus%29_comp%5B1%5D.pdf) |
| Workload instrument | [NASA Task Load Index](https://www.nasa.gov/human-systems-integration-division/nasa-task-load-index-tlx/) |
| User Experience Questionnaire | [UEQ Online](https://www.ueq-online.org/) |
| Severity ratings | [NN/g: Severity Ratings for Usability Problems](https://www.nngroup.com/articles/how-to-rate-the-severity-of-usability-problems/) |
| Accessibility evaluation overview | [W3C: Evaluating Web Accessibility Overview](https://www.w3.org/WAI/test-evaluate/) |
| Accessibility conformance methodology | [W3C: WCAG-EM Overview](https://www.w3.org/WAI/test-evaluate/conformance/wcag-em/) |
| Accessibility standard | [WCAG 2.2](https://www.w3.org/TR/WCAG22/) |
| WCAG overview | [W3C: WCAG Overview](https://www.w3.org/WAI/standards-guidelines/wcag/) |

^design-evaluating-design-end
