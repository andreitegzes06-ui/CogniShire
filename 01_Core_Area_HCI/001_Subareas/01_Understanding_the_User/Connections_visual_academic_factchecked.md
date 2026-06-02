---
title: Connections
area: Mind Library
category: Connections
cssclasses:
  - mind-library
tags:
  - HCI
  - cognition
  - psychology
  - design
  - accessibility
  - ethics
  - AI
  - sociotechnical-systems
status: visual-academic-factchecked
---

# Connections

> [!abstract] Bridge Map
> Connections maps how the Mind Library links HCI concepts to the wider field of Human-Computer Interaction. HCI draws from cognition, psychology, design, computer science, accessibility, ethics, artificial intelligence, organisational practice, and social life.

The Mind Library becomes useful when its concepts travel. A mental model matters because it changes how an interface should be structured. Cognitive load matters because it changes task performance and perceived effort. Accessibility matters because it changes who can participate. Trust matters because automated systems increasingly ask users to accept, question, correct, or override machine output.

Connections is therefore the bridge atlas of this area. It shows how ideas move from [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Activities/Theory]] into [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Activities/Design]], how they are tested in [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Activities/Experiment]], and how they expand into [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Important people]], [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Important Venues]], [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Local and Global]], and [[01_Core_Area_HCI/001_Subareas/01_Mind_Library/Open Problems]].

> [!quote] Bridge rule
> In HCI, an interaction problem is rarely only technical. It is also cognitive, social, material, ethical, and situated.

## Bridge compass

The first map shows the four main directions of the Mind Library. Cognition explains the user's limits and interpretations. Design turns those interpretations into visible form. Computing creates the system behaviour that users experience. Society shapes the values, institutions, cultures, and power relations around the interaction.

```mermaid
flowchart LR
    A["Mind Library"] --> B["Cognition"]
    A --> C["Design"]
    A --> D["Computing"]
    A --> E["Society"]

    B --> B1["Perception"]
    B --> B2["Memory"]
    B --> B3["Attention"]

    C --> C1["Form"]
    C --> C2["Feedback"]
    C --> C3["Navigation"]

    D --> D1["Systems"]
    D --> D2["AI"]
    D --> D3["Data"]

    E --> E1["Ethics"]
    E --> E2["Culture"]
    E --> E3["Access"]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef bridge fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E bridge;
    class B1,B2,B3,C1,C2,C3,D1,D2,D3,E1,E2,E3 detail;
```

| Bridge realm | Central question | HCI consequence |
|---|---|---|
| Cognition | How do users perceive, remember, decide, and learn? | Interfaces must respect attention, memory, and mental models. |
| Design | How should interaction become visible and usable? | Systems need structure, signifiers, feedback, and recovery paths. |
| Computing | How does system behaviour become interpretable? | Users need transparency, control, reliability, and understandable outcomes. |
| Society | Who is included, excluded, influenced, or harmed? | HCI must address accessibility, ethics, culture, and power. |

## The cognitive bridge

The cognitive bridge connects HCI with cognitive science and psychology. Interaction depends on perception, attention, memory, learning, decision-making, emotion, and expectation. Users do not approach interfaces as blank minds. They bring previous patterns, learned conventions, goals, fears, habits, and partial knowledge.

This bridge explains why people miss visible controls, rely on familiar layouts, misunderstand icons, forget multi-step processes, or trust confident system responses. It also explains why interface design cannot be separated from cognition. A search bar, menu, error message, filter, notification, or chatbot response becomes part of the user's thinking environment.

```mermaid
flowchart LR
    A["Cognitive Bridge"] --> B["Perception"]
    A --> C["Attention"]
    A --> D["Memory"]
    A --> E["Decision"]

    B --> B1["What is noticed"]
    C --> C1["What is selected"]
    D --> D1["What is retained"]
    E --> E1["What action is chosen"]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef bridge fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef trace fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E bridge;
    class B1,C1,D1,E1 trace;
```

The key move in this bridge is from isolated cognition to situated cognition. HCI does not study memory or attention as abstract laboratory objects only. It studies how memory and attention operate while a person works with a designed artefact. A calendar app supports memory. A progress bar supports expectation. A warning supports decision-making. A navigation structure supports orientation.

| Cognitive idea | Interface translation | Possible experimental trace |
|---|---|---|
| Mental model | System structure should match user expectation. | Users choose the expected route more quickly. |
| Cognitive load | Interfaces should reduce unnecessary mental effort. | Users complete tasks with fewer pauses and corrections. |
| Attention | Important actions should be visually discoverable. | Users notice primary actions without searching. |
| Feedback | System response should make action outcomes clear. | Users stop repeating actions after receiving confirmation. |

Useful anchors for this bridge include [NN/g on mental models](https://www.nngroup.com/articles/mental-models/), [NN/g on recognition rather than recall](https://www.nngroup.com/articles/recognition-and-recall/), and the [Interaction Design Foundation overview of HCI](https://www.interaction-design.org/literature/topics/human-computer-interaction).

## The design bridge

The design bridge connects knowledge about users to visible interaction form. If the Mind Library explains how users think, Design asks how that explanation should become structure, layout, navigation, signifier, feedback, constraint, and prototype.

A design is not just a visual layer. It is a theory of the user made visible. A layout implies what matters first. A menu implies how information is grouped. A button implies what action is possible. An error message implies how the system understands failure. A prototype implies what kind of interaction is being imagined.

```mermaid
flowchart LR
    A["Design Bridge"] --> B["Theory"]
    B --> C["Interface form"]
    C --> D["Prototype"]
    D --> E["Experiment"]
    E --> F["Redesign"]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef step fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef result fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E step;
    class F result;
```

> [!example] Bridge example
> A student portal may fail because its information architecture follows administrative departments rather than student goals. The issue is not only layout. It is a mismatch between institutional structure and user mental model.

The design bridge is closely linked to [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Activities/Design]]. Human-centred design makes this connection explicit by treating user needs, context of use, prototyping, and evaluation as part of the design process.

Useful anchors include [ISO 9241-210](https://www.iso.org/standard/77520.html), [NIST Human-Centered Design](https://www.nist.gov/itl/iad/human-centered-technologies/human-factors-human-centered-design), [Stanford d.school tools](https://dschool.stanford.edu/tools), and [NN/g on design thinking](https://www.nngroup.com/articles/design-thinking/).

## The computing bridge

The computing bridge connects HCI with the systems that execute, store, calculate, recommend, sense, predict, and automate. Users do not directly experience code as code. They experience system behaviour: delay, error, recommendation, notification, prediction, search result, chatbot answer, interface state, and data trace.

This bridge asks how technical behaviour becomes human meaning. A database result becomes a search page. Algorithmic ranking becomes perceived relevance. A model output becomes advice. A network delay becomes uncertainty. A permission request becomes trust or suspicion.

```mermaid
flowchart LR
    A["Technical system"] --> B["System behaviour"]
    B --> C["Interface state"]
    C --> D["User interpretation"]
    D --> E["Trust or action"]
    E --> F["Design responsibility"]

    classDef system fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef meaning fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;
    classDef result fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B,C system;
    class D,E meaning;
    class F result;
```

| System behaviour | User interpretation problem | Design responsibility |
|---|---|---|
| Delay | Is the system broken or still working? | Show progress, status, and recovery. |
| Recommendation | Why was this shown to me? | Explain relevance and allow control. |
| Error | What happened and how do I fix it? | Provide clear, actionable recovery. |
| Automation | Should I trust this decision? | Show uncertainty, limits, and override paths. |

This bridge is especially important for human-AI interaction. AI systems can be probabilistic, adaptive, and opaque. Users may overtrust them, undertrust them, misunderstand their limits, or treat generated output as more certain than it is.

Useful anchors include the [Microsoft Human-AI Interaction Guidelines](https://www.microsoft.com/en-us/research/project/guidelines-for-human-ai-interaction/), the [Microsoft HAX Toolkit](https://www.microsoft.com/en-us/haxtoolkit/ai-guidelines/), and Google's [People + AI Guidebook](https://pair.withgoogle.com/guidebook/).

## The AI trust gate

AI adds a special gate to the Connections map because it changes the relation between system behaviour and user interpretation. Traditional interfaces often respond through fixed rules. AI systems may produce uncertain, generated, personalised, or context-sensitive responses.

```mermaid
flowchart LR
    A["AI output"] --> B["Uncertainty or limit shown"]
    B --> C["User judgement"]
    C --> D["Accept"]
    C --> E["Reject"]
    C --> F["Correct"]
    D --> G["Consequence"]
    E --> G
    F --> G

    classDef ai fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef choice fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;
    classDef result fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B,C ai;
    class D,E,F choice;
    class G result;
```

> [!warning] Trust calibration
> The goal of human-AI interaction is not maximum trust. The goal is appropriate trust. Users should neither blindly accept nor automatically reject system output.

This gate connects directly to [[01_Core_Area_HCI/001_Subareas/01_Mind_Library/Open Problems]], because explainability, accountability, contestability, bias, automation dependence, and human agency remain difficult research and design problems.

## The accessibility and inclusion bridge

The accessibility bridge asks who can cross the system at all. A design that works only for a narrow imagined user is incomplete. HCI must account for differences in vision, hearing, movement, cognition, language, age, device access, network conditions, and social context.

Accessibility is not only a legal or technical checklist. It is a theory of participation. It asks whether people can perceive information, operate controls, understand interaction, and use the system with current and future technologies.

```mermaid
flowchart LR
    A["Inclusion Bridge"] --> B["Perceivable"]
    A --> C["Operable"]
    A --> D["Understandable"]
    A --> E["Robust"]

    B --> B1["Contrast and alternatives"]
    C --> C1["Keyboard and focus"]
    D --> D1["Clear language"]
    E --> E1["Assistive technology"]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef principle fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef practice fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E principle;
    class B1,C1,D1,E1 practice;
```

The main external anchors for this bridge are the [W3C Web Accessibility Initiative](https://www.w3.org/WAI/), the [W3C Accessibility Principles](https://www.w3.org/WAI/fundamentals/accessibility-principles/), [WCAG 2.2](https://www.w3.org/TR/WCAG22/), and [WebAIM](https://webaim.org/). In the vault, this route connects strongly to [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Local and Global]], because accessibility is shaped by language, infrastructure, device availability, education, disability, and institutional power.

## The ethical bridge

The ethical bridge appears whenever a system shapes attention, action, access, privacy, or judgement. HCI cannot treat the user as a data point alone. The user is a person situated in a social world, and interaction design can support or weaken autonomy, dignity, safety, fairness, and trust.

```mermaid
flowchart LR
    A["Ethical Bridge"] --> B["Privacy"]
    A --> C["Autonomy"]
    A --> D["Fairness"]
    A --> E["Accountability"]

    B --> B1["Data minimisation"]
    C --> C1["Meaningful control"]
    D --> D1["Bias awareness"]
    E --> E1["Clear responsibility"]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef value fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef action fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E value;
    class B1,C1,D1,E1 action;
```

| Ethical concern | HCI question | Design implication |
|---|---|---|
| Privacy | Does the user understand what data is collected? | Make data practices visible and controllable. |
| Autonomy | Can the user refuse, undo, or override? | Provide meaningful exits and alternatives. |
| Fairness | Who receives poorer outcomes? | Test across groups and contexts. |
| Accountability | Who is responsible when the system harms? | Make responsibility and escalation paths clear. |

The [ACM Code of Ethics](https://www.acm.org/code-of-ethics) is a strong professional anchor for this bridge. For AI-mediated systems, the ethical bridge also connects to the [ACM FAccT Conference](https://facctconference.org/), where fairness, accountability, and transparency are treated as sociotechnical research problems.

## The social and organisational bridge

Many HCI problems are not located only inside the interface. They also come from organisations, institutions, work practices, social norms, and economic incentives. A hospital system, school platform, government portal, or workplace dashboard does not exist as an isolated screen. It exists inside procedures, roles, rules, deadlines, and responsibilities.

```mermaid
flowchart LR
    A["Institutional requirement"] --> B["Official platform"]
    B --> C["Interface labels"]
    C --> D["Form or workflow"]
    D --> E["System feedback"]
    E --> F["Support or escalation"]
    F --> G["Organisational outcome"]

    classDef context fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef interaction fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;
    classDef outcome fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B context;
    class C,D,E,F interaction;
    class G outcome;
```

This bridge matters because an interface can be locally usable but globally frustrating. A form may be easy to complete, but the institutional process behind it may be opaque. A chatbot may answer quickly, but the organisation may provide no human escalation. HCI therefore studies micro-interactions and larger sociotechnical systems.

This route connects directly to [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Local and Global]], where the same design may function differently across cultures, languages, institutions, infrastructures, and legal environments.

## Bridge atlas

The following atlas summarises the major crossings inside the Connections chamber.

| Crossing | Connected discipline | What enters HCI | What HCI transforms it into |
|---|---|---|---|
| Cognitive bridge | Cognitive science | Attention, memory, perception | Interface structure and mental model support |
| Psychological bridge | Psychology | Error, motivation, learning | Task design, feedback, and evaluation |
| Design bridge | Design studies | Form, prototyping, visual hierarchy | Interaction flows and usability principles |
| Computing bridge | Computer science | Algorithms, systems, data | Interpretable and controllable user experience |
| Accessibility bridge | Disability studies and standards | Human diversity and assistive technology | Inclusive interaction and WCAG-based evaluation |
| Ethical bridge | Applied ethics | Autonomy, privacy, fairness, accountability | Responsible design and transparent systems |
| Social bridge | Sociology and organisational studies | Institutions, roles, practices | Sociotechnical analysis of real-world use |

## Connection patterns

This chamber does not connect ideas randomly. Most HCI bridges follow recurring patterns.

```mermaid
flowchart LR
    A["Human capacity"] --> B["Interface assumption"]
    B --> C["Observed interaction"]
    C --> D["HCI explanation"]
    D --> E["Design consequence"]

    classDef step fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef explanation fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;
    classDef result fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B,C step;
    class D explanation;
    class E result;
```

For example, limited working memory becomes an interface assumption about how much information users can hold. That assumption appears in navigation, form design, onboarding, and error recovery. Evaluation then shows whether the assumption holds. The design consequence may be a change in layout, feedback, labels, grouping, or task flow.

## Chamber synthesis

Connections makes the Mind Library more than a psychology shelf. It becomes a bridge system linking cognition to design form, design form to technical implementation, technical implementation to social context, and social context to ethical responsibility.

The central demand of the chamber is careful translation. Concepts should not remain abstract. They must move into design choices, experimental methods, accessibility checks, ethical questions, and sociotechnical analysis. A strong HCI project does not ask only what users think. It asks how systems shape thinking, how design shapes action, how context shapes interpretation, and how evidence should reshape the system.

## Academic anchors

| Route | Trusted source | Why it supports this page |
|---|---|---|
| HCI research community | [ACM SIGCHI](https://sigchi.org/) | Identifies SIGCHI as a major international HCI community. |
| Academic HCI venue | [ACM CHI Conference](https://dl.acm.org/conference/chi) | Shows the central conference route for HCI research. |
| HCI publications | [ACM Digital Library](https://dl.acm.org/) | Provides access to peer-reviewed HCI research. |
| Human-centred design | [ISO 9241-210:2019](https://www.iso.org/standard/77520.html) | Defines human-centred design principles and activities for interactive systems. |
| Human-centred technologies | [NIST Human-Centered Design](https://www.nist.gov/itl/iad/human-centered-technologies/human-factors-human-centered-design) | Supports the link between usability, human factors, user needs, and evaluation. |
| Usability and UX research | [Nielsen Norman Group](https://www.nngroup.com/) | Provides practical guidance on mental models, recognition, design thinking, and usability. |
| Accessibility standards | [W3C Web Accessibility Initiative](https://www.w3.org/WAI/) | Provides standards and guidance for accessible web interaction. |
| Accessibility guidelines | [WCAG 2.2](https://www.w3.org/TR/WCAG22/) | Supports the four accessibility principles used in the inclusion bridge. |
| Human-AI interaction | [Microsoft Human-AI Interaction Guidelines](https://www.microsoft.com/en-us/research/project/guidelines-for-human-ai-interaction/) | Supports guidance on AI system behaviour across initial use, regular use, errors, and change over time. |
| AI design practice | [Google People + AI Guidebook](https://pair.withgoogle.com/guidebook/) | Provides practical guidance for human-centred AI products. |
| Computing ethics | [ACM Code of Ethics](https://www.acm.org/code-of-ethics) | Supports the ethical bridge through public good, harm reduction, privacy, honesty, and responsibility. |
| Fairness and accountability | [ACM FAccT](https://facctconference.org/) | Connects AI and computing systems to fairness, accountability, transparency, and sociotechnical analysis. |

## Connected chambers

This chamber connects to [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Overview]] because it explains why the Mind Library exists as a bridge system. It connects to [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Activities/Theory]] because theory supplies the concepts that travel across the map. It connects to [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Activities/Design]] because design gives those concepts visible form. It connects to [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Activities/Experiment]] because experiments test whether the bridges actually hold. It connects to [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Important people]] and [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Important Venues]] because HCI knowledge is built by communities, conferences, laboratories, and scholars. It connects to [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Local and Global]] because interaction changes across cultures and infrastructures. It connects to [[01_Core_Area_HCI/001_Subareas/01_Mind_Library/Open Problems]] because many bridges remain unstable, contested, and unfinished.

^connections-end
