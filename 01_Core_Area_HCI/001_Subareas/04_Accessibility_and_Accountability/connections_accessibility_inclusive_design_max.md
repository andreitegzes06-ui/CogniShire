---
title: Connections
area: Accessibility and Inclusive Design
display-name: The Inclusive Gate
category: Method Bridge
cs2023_unit: HCI-Accessibility
secondary_unit: HCI-Accountability
cssclasses:
  - inclusive-gate
tags:
  - HCI
  - CS2023
  - HCI-Accessibility
  - accessibility
  - inclusive-design
  - connections
  - disability-studies
  - assistive-technology
  - WCAG
  - WAI-ARIA
  - policy
  - ethics
  - design-systems
  - software-engineering
  - education
  - UVT
  - local-global
status: expanded-polished-draft
---

# Connections

Back to [[Overview|The Inclusive Gate]].

> [!abstract] Accessibility Bridge Map
> **Connections** in the Inclusive Gate shows how Accessibility and Inclusive Design depends on several fields at once. It connects HCI to disability studies, assistive technology, web standards, software engineering, design systems, law and policy, education, ethics, public services, health technology, human factors, AI, and the local UVT context.

The fantasy name is **Accessibility Bridge Map**.  
The real CS2023 label is **HCI-Accessibility: Accessibility and Inclusive Design**.  
The connected responsibility route is **HCI-Accountability: Accountability and Responsibility in Design**.  
The real-life meaning is **understanding that accessibility is a technical, social, institutional, and ethical design problem**.

This page is not a checklist. It is a bridge map. It explains which fields must be connected when a design claims that more people can perceive it, operate it, understand it, trust it, and participate through it.

> [!quote] Bridge rule
> Accessibility becomes stronger when it is treated as a system of relations: people, tools, code, standards, institutions, evidence, and responsibility.

## Connection Map

```mermaid
flowchart TB
    A((Inclusive Gate<br/>Connections))

    A --> B[Disability Studies]
    A --> C[Assistive Technology]
    A --> D[Web Standards]
    A --> E[Software Engineering]
    A --> F[Design Systems]
    A --> G[Law + Policy]
    A --> H[Education]
    A --> I[Ethics + Accountability]
    A --> J[AI + Data Systems]

    B --> B1[Exclusion and barriers]
    C --> C1[Real access tools]
    D --> D1[WCAG, WAI, ARIA]
    E --> E1[Testing and maintenance]
    F --> F1[Reusable accessible patterns]
    G --> G1[Rights and duties]
    H --> H1[Learning access]
    I --> I1[Harm, dignity, repair]
    J --> J1[Bias, adaptation, uncertainty]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G,H,I,J node;
    class B1,C1,D1,E1,F1,G1,H1,I1,J1 detail;
```

| Connected field | What it adds to accessibility | What goes wrong if it is ignored |
|---|---|---|
| Disability studies | Explains exclusion as a relation between people, systems, and environments | Designers treat disability only as a defect inside the user |
| Assistive technology | Shows how people actually access digital systems | Interfaces are built only for mouse, screen, and default settings |
| Web standards | Gives technical criteria and semantic structure | Content may look visible but remain unusable to assistive tools |
| Software engineering | Keeps accessibility stable through updates | Accessibility breaks after CSS, plugin, or component changes |
| Design systems | Makes accessible patterns reusable | Each page solves access differently and inconsistently |
| Law and policy | Connects access to rights, procurement, and institutional duty | Accessibility becomes optional or decorative |
| Education | Connects access to students, teachers, materials, and assessment | Students are forced to ask for exceptions after barriers appear |
| Ethics and accountability | Defines responsibility for harm, exclusion, and repair | Excluded users are blamed for design failures |
| AI and data systems | Shows how automation can help or harm access | Barriers can be reproduced at scale and hidden behind fluent output |

## CS2023 Connection Gate

CS2023 places Accessibility and Inclusive Design inside HCI. That means accessibility is not separate from user research, system design, evaluation, and accountability. It belongs to the whole HCI map.

```mermaid
flowchart TB
    A((CS2023 HCI))

    A --> B[Understanding Users]
    A --> C[System Design]
    A --> D[Evaluating Design]
    A --> E[Accessibility +<br/>Inclusive Design]
    A --> F[Accountability]

    B --> B1[Human variation]
    C --> C1[Accessible structure]
    D --> D1[Evidence of barriers]
    E --> E1[Standards and frameworks]
    F --> F1[Responsibility and harm]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

| HCI area | Accessibility connection |
|---|---|
| Understanding the User | Users differ in vision, hearing, motor control, cognition, language, device, context, stress, and experience |
| System Design | Accessibility becomes structure, labels, focus order, keyboard paths, alternatives, error states, and component behaviour |
| Evaluating the Design | Accessibility must be checked through standards, manual review, assistive technology, and user evidence |
| Accessibility and Inclusive Design | The central route for WCAG, inclusive design, universal design, ability-based design, and assistive technologies |
| Accountability | Designers must state assumptions, limits, harms, excluded users, and repairs |

## Local UVT Connection Layer

The local dimension is the **Faculty of Informatics / Computer Science context at UVT**. Accessibility connects locally to students, teachers, project materials, GitHub repositories, Obsidian vaults, classroom presentation, professor review, and UVT support for students with disabilities.

UVT also has a wider institutional accessibility context. That matters because accessibility is not only a code issue. It is also connected to support services, teaching adaptations, alternative materials, assistive technologies, and academic participation.

```mermaid
flowchart TB
    A((Local UVT<br/>Accessibility Layer))

    A --> B[Students]
    A --> C[Teachers]
    A --> D[Support Services]
    A --> E[Digital Projects]
    A --> F[Faculty of Informatics]
    A --> G[Institutional Access]

    B --> B1[Different access needs]
    C --> C1[Adapt teaching and review]
    D --> D1[Psychopedagogical support]
    E --> E1[Obsidian, GitHub, Markdown]
    F --> F1[Computer Science project context]
    G --> G1[Spaces, materials, participation]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

| Local UVT connection | Why it matters for Cognishire |
|---|---|
| Students with different access needs | The map should not assume one perfect reader, device, language level, attention level, or input method |
| Teachers and evaluators | The academic structure must be visible without the author explaining it verbally |
| Psychopedagogical support | Accessibility has a local institutional context, not only a technical one |
| Faculty of Informatics | The project is a Computer Science artifact and should connect accessibility to software, AI, data, and digital systems |
| GitHub and Obsidian | Sharing and rendering problems are accessibility and robustness problems |
| Classroom presentation | Text, diagrams, and contrast must work on a projector or shared screen |
| Institutional initiatives | Accessibility includes physical, digital, academic, and social participation |

## Disability Studies Bridge

Disability studies helps HCI avoid a narrow view of disability. It shows that barriers are often created by environments, policies, tools, and assumptions. In HCI, this matters because an interface can create a disability barrier even when the user is skilled and motivated.

```mermaid
flowchart TB
    A((Disability Studies Bridge))

    A --> B[Medical Model]
    A --> C[Social Model]
    A --> D[Interactional View]
    A --> E[Design Response]

    B --> B1[Problem placed in body]
    C --> C1[Problem placed in barriers]
    D --> D1[Person, tool, task, context]
    E --> E1[Change the system]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

| Disability studies idea | HCI consequence |
|---|---|
| Disability is shaped by environment | The interface can create or remove barriers |
| Exclusion is social and political | Accessibility is about rights, dignity, and participation, not only usability |
| The “average user” is a design simplification | Human variation must be expected from the beginning |
| Accommodation is not failure | Alternative formats and flexible interaction are part of responsible design |
| Lived experience matters | Disabled users can reveal barriers that checklists miss |

This bridge connects to [[Theory]] because it explains why accessibility is not just a set of technical fixes. It is also a way to understand power, participation, and design assumptions.

## Assistive Technology Bridge

Assistive technology is where accessibility becomes concrete. Users may access systems through screen readers, keyboards, voice control, magnification, switch devices, captions, transcripts, braille displays, or other tools.

```mermaid
flowchart TB
    A((Assistive Technology Bridge))

    A --> B[Screen Reader]
    A --> C[Keyboard]
    A --> D[Magnification]
    A --> E[Voice Control]
    A --> F[Switch Input]
    A --> G[Captions + Transcripts]

    B --> B1[Semantic structure]
    C --> C1[Focus and operable path]
    D --> D1[Scalable layout]
    E --> E1[Visible labels]
    F --> F1[Sequential operation]
    G --> G1[Text alternatives]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

| Assistive technology | Connected design field |
|---|---|
| Screen reader | Semantic HTML, headings, landmarks, labels, link text, table structure |
| Keyboard navigation | Focus management, interaction design, component behaviour |
| Magnification | Responsive design, layout, typography, zoom support |
| Voice control | Visible labels, commandable controls, predictable UI |
| Switch devices | Sequential navigation and low-complexity interaction |
| Captions and transcripts | Multimedia design, education, public communication |
| Braille display | Semantic structure, text clarity, and language support |

For the Cognishire vault, headings, links, diagrams, source tables, and fallback text are access infrastructure. They are not cosmetic formatting.

## Web Standards Bridge

Web accessibility connects HCI to W3C standards. WCAG gives accessibility success criteria. WAI-ARIA can add semantics for complex widgets when native HTML is not enough. The ARIA Authoring Practices Guide gives patterns for accessible widgets and interactions. WCAG-EM gives a structured method for evaluating WCAG conformance.

```mermaid
flowchart TB
    A((Web Standards Bridge))

    A --> B[HTML Semantics]
    A --> C[WCAG]
    A --> D[WAI-ARIA]
    A --> E[APG Patterns]
    A --> F[Evaluation Guidance]

    B --> B1[Native structure first]
    C --> C1[POUR success criteria]
    D --> D1[Roles, states, properties]
    E --> E1[Accessible widgets]
    F --> F1[WCAG-EM and reports]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

| Standard route | What it contributes |
|---|---|
| HTML semantics | Gives structure before extra accessibility code is needed |
| WCAG 2.2 | Gives success criteria for accessible web content |
| WAI-ARIA | Adds accessibility semantics for complex widgets when native semantics are insufficient |
| ARIA Authoring Practices Guide | Shows accessible design patterns for common widgets |
| W3C WAI evaluation guidance | Helps structure accessibility checking and reporting |
| WCAG-EM | Gives a methodology for evaluating WCAG conformance |

A useful rule is: **use native structure first**. Add ARIA only when the native element cannot express the interaction correctly.

## Software Engineering Bridge

Accessibility fails when it is treated as a one-time design layer. Software engineering connects accessibility to maintenance, version control, code review, regression checks, design-system governance, continuous integration, and documentation.

```mermaid
flowchart TB
    A((Software Engineering Bridge))

    A --> B[Version Control]
    A --> C[Automated Tests]
    A --> D[Code Review]
    A --> E[Component Library]
    A --> F[Regression Checks]
    A --> G[Documentation]

    B --> B1[Track what changed]
    C --> C1[Catch detectable issues]
    D --> D1[Review access risk]
    E --> E1[Reuse good patterns]
    F --> F1[Prevent access drift]
    G --> G1[Explain setup and limits]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

| Software engineering practice | Accessibility value |
|---|---|
| Git versioning | Shows which version was tested and which change introduced a barrier |
| Pull request review | Allows accessibility checks before changes merge |
| Automated accessibility tests | Catch repeated detectable issues early |
| Manual regression checklist | Catches focus, keyboard, semantics, and visual barriers that automation misses |
| Component library | Fixes one pattern once, then reuses it |
| Documentation | Helps users and contributors understand setup, dependencies, and limits |
| Issue tracking | Makes barriers visible as concrete repair tasks |

For this project, GitHub is part of the access path. If CSS disappears, Mermaid styling breaks, or links become unstable after cloning, the project becomes less accessible.

## Design Systems Bridge

Design systems connect accessibility to reusable decisions. Instead of repairing access separately on every page, a design system encodes accessible colour pairs, typography, focus styles, spacing, component states, error patterns, and documentation.

```mermaid
flowchart TB
    A((Design Systems Bridge))

    A --> B[Tokens]
    A --> C[Components]
    A --> D[Patterns]
    A --> E[Documentation]
    A --> F[Governance]

    B --> B1[Colour, type, spacing, focus]
    C --> C1[Buttons, forms, links]
    D --> D1[Navigation, errors, states]
    E --> E1[How to use accessibly]
    F --> F1[How changes are approved]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

| Design-system item | Accessibility connection |
|---|---|
| Colour token | Reduces accidental low contrast |
| Typography token | Supports readability, scaling, and long reading |
| Focus style | Makes keyboard location visible |
| Component pattern | Preserves semantics and behaviour |
| Error pattern | Gives clear, local, recoverable feedback |
| Documentation | Teaches contributors how not to break access |
| Governance | Prevents inaccessible variants from spreading |

The Cognishire vault can use the same logic. CSS classes for Mermaid diagrams, callouts, tables, source blocks, and route boards should behave like a small design system.

## Law and Policy Bridge

Accessibility is not only a design preference. It is also connected to rights, public-sector duties, procurement, and compliance. In Europe, digital accessibility connects to the Web Accessibility Directive, EN 301 549, and the European Accessibility Act.

```mermaid
flowchart TB
    A((Law + Policy Bridge))

    A --> B[Rights]
    A --> C[Public Sector]
    A --> D[Procurement]
    A --> E[Standards]
    A --> F[Accountability]

    B --> B1[Access as participation]
    C --> C1[Websites and apps]
    D --> D1[ICT products and services]
    E --> E1[EN 301 549, WCAG]
    F --> F1[Reports and responsibility]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

| Policy route | What it gives to HCI |
|---|---|
| Web Accessibility Directive | EU public-sector web and mobile accessibility requirements |
| EN 301 549 | Accessibility requirements for ICT products and services |
| European Accessibility Act | EU accessibility rules for selected products and services |
| WCAG | Technical web accessibility standard used by many policies |
| Institutional policy | Local procedures for students, staff, services, teaching, and assessment |
| Procurement | Accessibility becomes a requirement when choosing or building systems |

For a student project, this does not mean making legal claims. It means recognising that accessibility is an institutional responsibility and that technical decisions can affect rights, assessment, and participation.

## Education Bridge

Accessibility and Inclusive Design connects strongly to education. Students need access to readings, slides, platforms, code repositories, assessments, classrooms, software tools, and teacher communication.

```mermaid
flowchart TB
    A((Education Bridge))

    A --> B[Learning Materials]
    A --> C[Assessment]
    A --> D[Classroom]
    A --> E[Digital Platforms]
    A --> F[Student Support]
    A --> G[Teacher Practice]

    B --> B1[Readable and alternative formats]
    C --> C1[Fair demonstration of learning]
    D --> D1[Physical and social access]
    E --> E1[LMS, GitHub, documents]
    F --> F1[Accommodations and services]
    G --> G1[Inclusive teaching choices]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

| Education problem | Accessibility connection |
|---|---|
| Long PDF or note with weak structure | Screen reader and cognitive access problems |
| Slides with tiny text | Low-vision and classroom readability barrier |
| Project works only on one machine | Assessment access and fairness problem |
| Instructions hidden in a chat | Cognitive and organisational barrier |
| GitHub repository missing setup instructions | Technical access barrier |
| Assessment requires one format only | Alternative expression and accommodation issue |
| Teacher cannot inspect project easily | Academic communication barrier |

For the local UVT map, education is not a side topic. The map is a learning artifact, so accessibility means learning access.

## Ethics and Accountability Bridge

Accessibility is ethical because exclusion shifts burden onto users. A design can force users to ask for help, reveal disability, spend extra time, or fail a task through no fault of their own.

```mermaid
flowchart TB
    A((Ethics + Accountability Bridge))

    A --> B[Harm]
    A --> C[Dignity]
    A --> D[Fairness]
    A --> E[Transparency]
    A --> F[Responsibility]

    B --> B1[What damage can exclusion cause?]
    C --> C1[Does the system respect the user?]
    D --> D1[Who receives extra burden?]
    E --> E1[Are limits stated clearly?]
    F --> F1[Who repairs the barrier?]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

| Ethical issue | Accessibility version |
|---|---|
| Harm | A user cannot complete a task, submit work, or access information |
| Dignity | A user must ask for special help because the system ignored them |
| Fairness | Some users need more effort for the same outcome |
| Transparency | The project hides what was not tested |
| Responsibility | The designer treats access failure as a user problem |
| Repair | The team fixes the barrier and retests it |

This bridge connects directly to CS2023 Accountability. Inclusive Design is incomplete if it does not report exclusions and repairs.

## Health and Public Services Bridge

Accessibility also matters in health and public services, where interaction failures can have serious consequences. A system that is confusing in a low-stakes context may become harmful when users need medical information, social services, public forms, or emergency support.

```mermaid
flowchart TB
    A((Health + Public Services Bridge))

    A --> B[Health Systems]
    A --> C[Public Forms]
    A --> D[Identity + Access]
    A --> E[Risk Communication]
    A --> F[Service Continuity]

    B --> B1[High-stakes decisions]
    C --> C1[Forms must be usable]
    D --> D1[Authentication can exclude]
    E --> E1[Warnings must be clear]
    F --> F1[Alternative access routes]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

| Public or health context | Accessibility concern |
|---|---|
| Medical portal | Users must understand results, warnings, appointments, and actions |
| Public form | Users must complete steps without inaccessible fields or time pressure |
| Identity verification | Authentication can exclude users with cognitive, sensory, or motor barriers |
| Emergency or health warning | Meaning cannot depend on colour, sound, or dense text alone |
| E-health monitoring | Data must be interpretable and not create false trust |
| Public university service | Students must access information without needing private workarounds |

This bridge connects to UVT because the local Computer Science context includes AI, medical informatics, e-health, data, and software systems. Accessibility is therefore relevant to local technical work, not only to web pages.

## Human Factors Bridge

Human factors connects accessibility to perception, attention, workload, fatigue, safety, and human performance. It helps explain why a technically accessible interface can still be too demanding for real use.

```mermaid
flowchart TB
    A((Human Factors Bridge))

    A --> B[Perception]
    A --> C[Attention]
    A --> D[Workload]
    A --> E[Fatigue]
    A --> F[Safety]

    B --> B1[Can users notice it?]
    C --> C1[Can users focus?]
    D --> D1[How much effort?]
    E --> E1[Does use become tiring?]
    F --> F1[What happens if it fails?]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

| Human factors concept | Accessibility link |
|---|---|
| Perception | Contrast, typography, icons, spacing, diagram readability |
| Attention | Clear hierarchy and reduced visual clutter |
| Workload | Fewer memory demands and simpler recovery paths |
| Fatigue | Avoid repeated precision tasks, dense scanning, and long unstructured pages |
| Safety | High-stakes systems need stricter access and error handling |
| Context of use | Real devices, lighting, classroom settings, and stress change access |

For Cognishire, the human factors bridge matters in projector view, long reading sessions, small screens, and local classroom review.

## AI and Data Systems Bridge

AI can support accessibility, but it can also introduce new barriers. It can generate captions, descriptions, summaries, code, and alternative formats. It can also hallucinate, misread images, create biased predictions, hide uncertainty, or produce inaccessible interfaces.

```mermaid
flowchart TB
    A((AI + Data Systems Bridge))

    A --> B[Generated Access]
    A --> C[Bias]
    A --> D[Explainability]
    A --> E[Uncertainty]
    A --> F[User Control]
    A --> G[Data Responsibility]

    B --> B1[Captions, alt text, summaries]
    C --> C1[Unequal performance]
    D --> D1[Why did it respond?]
    E --> E1[How sure is it?]
    F --> F1[Can user override it?]
    G --> G1[Consent and privacy]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

| AI accessibility issue | Design question |
|---|---|
| Generated alt text | Is the description accurate enough for the user’s task? |
| Speech recognition | Does performance vary across speech patterns, accents, or disabilities? |
| AI summarisation | Does the summary remove information needed for access or safety? |
| Adaptive interface | Can users understand and control the adaptation? |
| Prediction system | Does the system explain uncertainty and avoid overtrust? |
| Dataset bias | Which users were absent or misrepresented in the data? |
| AI-created code | Does generated UI code preserve accessibility semantics? |

This bridge connects to [[../05_Human_AI_Interaction/Overview|Oracle Engine]]. Any AI part of Cognishire should be checked for correctness, accessibility, bias, and user control.

## Local to Global Repair Path

Connections are useful only when they change design decisions. A local problem should be linked to the field that can explain it and to a repair that can be tested.

```mermaid
flowchart LR
    A[Local barrier] --> B[Connected field]
    B --> C[Trusted source]
    C --> D[Design repair]
    D --> E[Retest]

    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B,C,D node;
    class E final;
```

| Local barrier | Connected field | Source route | Repair |
|---|---|---|---|
| Diagram text is unreadable | Visual accessibility and human factors | WCAG, WebAIM, W3C WAI | Use light Mermaid boxes, dark text, compact labels, and table explanation |
| Theme fails after GitHub clone | Software engineering | Reproducibility, robust content, documentation | Keep content readable without CSS and document setup |
| Fantasy name confuses professor | Cognitive accessibility and education | Inclusive design, plain language, CS2023 labels | Pair metaphor with official academic label |
| Keyboard navigation is weak | Assistive technology and web standards | WCAG operable criteria, ARIA practices | Check focus order and keyboard-reachable routes |
| Student cannot identify trusted sources | Information architecture and education | Academic source hierarchy | Group anchors by source type |
| Accessibility is not retested after changes | Software engineering and accountability | Regression testing, WAI evaluation | Add an accessibility check to every page revision |

## Connection Board for Cognishire

```mermaid
flowchart TB
    A((Cognishire<br/>Accessibility Connections))

    A --> B[Obsidian]
    A --> C[GitHub]
    A --> D[Mermaid]
    A --> E[CSS Theme]
    A --> F[Academic Sources]
    A --> G[UVT Context]

    B --> B1[Markdown structure]
    C --> C1[Robust sharing]
    D --> D1[Diagram alternatives]
    E --> E1[Contrast and focus]
    F --> F1[Trusted routes]
    G --> G1[Students, professor, support context]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

| Cognishire element | Connected accessibility field |
|---|---|
| Obsidian Markdown | Web standards, semantic structure, cognitive accessibility |
| GitHub repository | Software engineering, reproducibility, robust content |
| Mermaid diagrams | Visual communication, cognitive accessibility, non-text alternatives |
| CSS theme | Design systems, contrast, typography, focus style |
| Academic sources | Education, information architecture, trust |
| UVT local context | Institutional accessibility, student support, project evaluation |
| Future AI guide | AI accessibility, bias, explainability, user control |
| Local presentation | Human factors, classroom readability, educational access |

## Connection Reliability Ladder

```mermaid
flowchart TB
    A((Connection Reliability))

    A --> B[Standards + Policy]
    B --> C[Peer-Reviewed Research]
    C --> D[Institutional Sources]
    D --> E[Design System Docs]
    E --> F[Practice Guides]
    F --> G[Blogs + Tutorials]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class G final;
```

| Source type | Use it for | Caution |
|---|---|---|
| Standards and policy | WCAG, EN 301 549, institutional duties, conformance | Standards still need interpretation in real use |
| Peer-reviewed research | Concepts, evidence, open problems, HCI arguments | Papers may be narrow or advanced |
| Institutional sources | Local UVT context and official support information | They may not explain HCI theory |
| Design-system documentation | Practical component rules and accessible patterns | Product-specific rules may not fully generalise |
| Practice guides | Learning, checklists, implementation steps | Not always peer-reviewed |
| Blogs and tutorials | Quick tool help | Not enough for academic grounding alone |

## Study Route

```mermaid
flowchart TB
    A((Study Route))

    A --> B[Start with WCAG + WAI]
    B --> C[Learn disability theory]
    C --> D[Study assistive tools]
    D --> E[Connect to software engineering]
    E --> F[Connect to law and policy]
    F --> G[Apply to UVT project]
    G --> H[Test and repair Cognishire]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class H final;
```

| Step | What to read or do |
|---|---|
| 1 | Read W3C WAI accessibility principles and the WCAG overview |
| 2 | Study Microsoft Inclusive Design and Universal Design principles |
| 3 | Learn how screen readers, keyboard navigation, captions, and magnification change interface requirements |
| 4 | Read ARIA Authoring Practices for complex widgets |
| 5 | Look at accessible design-system documentation such as Carbon, Material, Apple, or GOV.UK |
| 6 | Connect to EU policy through EN 301 549 and the European Accessibility Act |
| 7 | Ground the local layer in UVT accessibility services and Faculty of Informatics context |
| 8 | Apply the connections to Cognishire through a barrier, repair, and retest cycle |

## What This Page Should Not Claim

| Do not claim | Safer wording |
|---|---|
| “Accessibility is solved by following WCAG.” | “WCAG gives a necessary baseline, but real access also needs testing and user evidence.” |
| “Assistive technology users are one group.” | “Assistive technology use varies by person, task, tool, and context.” |
| “A design system is automatically accessible.” | “A design system can support accessibility if its components are tested and maintained.” |
| “AI makes accessibility automatic.” | “AI can support access, but its outputs must be checked for correctness, bias, uncertainty, and control.” |
| “UVT support pages prove this project is accessible.” | “UVT support pages give local context; the project still needs its own accessibility checks.” |
| “Blogs are enough for academic grounding.” | “Practice guides help implementation, but academic pages need standards and research anchors.” |

## Synthesis

Connections in **Accessibility and Inclusive Design** show that accessibility is not a small technical afterthought. It is a bridge between disability studies, assistive technology, web standards, software engineering, design systems, law, education, ethics, health, public services, AI, human factors, and institutional responsibility.

Locally, the Inclusive Gate must speak to the UVT project context: students, professors, learning materials, GitHub, Obsidian, CSS, Markdown, diagrams, and university support for students with disabilities. Globally, it must connect to CS2023, WCAG, WAI-ARIA, EN 301 549, inclusive design, ACM SIGACCESS, ASSETS, Web4All, and accessibility-focused HCI research.

The central question is:

> Which fields must connect so that access is designed, tested, maintained, and repaired instead of left to chance?

This page connects to [[Theory]] because each bridge explains why accessibility matters. It connects to [[Design]] because each bridge becomes a design rule. It connects to [[Experiment]] because each bridge needs evidence. It connects to [[../Overview|Overview]] because the Inclusive Gate protects the whole HCI map.

## Academic Anchors

| Route | Source |
|---|---|
| CS2023 HCI Accessibility basis | [CS2023 HCI Version Gamma](https://csed.acm.org/wp-content/uploads/2023/09/HCI-Version-Gamma.pdf) |
| CS2023 Knowledge Areas | [CS2023 Knowledge Areas](https://csed.acm.org/knowledge-areas/) |
| WCAG 2.2 standard | [W3C WCAG 2.2](https://www.w3.org/TR/WCAG22/) |
| WCAG overview | [W3C WCAG Overview](https://www.w3.org/WAI/standards-guidelines/wcag/) |
| WAI accessibility principles | [W3C Accessibility Principles](https://www.w3.org/WAI/fundamentals/accessibility-principles/) |
| WAI-ARIA overview | [W3C WAI-ARIA Overview](https://www.w3.org/WAI/standards-guidelines/aria/) |
| ARIA Authoring Practices | [WAI-ARIA Authoring Practices Guide](https://www.w3.org/WAI/ARIA/apg/) |
| Accessibility evaluation | [W3C Evaluating Web Accessibility](https://www.w3.org/WAI/test-evaluate/) |
| WCAG conformance evaluation | [W3C WCAG-EM Overview](https://www.w3.org/WAI/test-evaluate/conformance/wcag-em/) |
| Inclusive design method | [Microsoft Inclusive Design](https://inclusive.microsoft.design/) |
| Inclusive design toolkit | [Microsoft Inclusive 101 Guidebook](https://inclusive.microsoft.design/articles/inclusive-101-guidebook) |
| Universal Design principles | [The Center for Universal Design](https://design.ncsu.edu/research/center-for-universal-design/) |
| Ability-Based Design paper | [Ability-Based Design: Concept, Principles and Examples](https://kgajos.seas.harvard.edu/papers/wobbrock11abd.pdf) |
| Ability-Based Design ACM record | [ACM Transactions on Accessible Computing: Ability-Based Design](https://dl.acm.org/doi/10.1145/1952383.1952384) |
| European Accessibility Act | [European Commission: European Accessibility Act](https://commission.europa.eu/strategy-and-policy/policies/justice-and-fundamental-rights/disability/european-accessibility-act-eaa_en) |
| EN 301 549 | [AccessibleEU: EN 301 549](https://accessible-eu-centre.ec.europa.eu/content-corner/digital-library/en-3015492021-accessibility-requirements-ict-products-and-services_en) |
| Accessibility research community | [ACM SIGACCESS](https://www.sigaccess.org/) |
| ACM SIGACCESS description | [ACM SIGACCESS](https://www.acm.org/special-interest-groups/sigs/sigaccess) |
| Accessibility conference | [ACM ASSETS](https://dl.acm.org/conference/assets) |
| Web accessibility conference | [Web4All](https://www.w4a.info/) |
| Practical accessibility resource | [WebAIM](https://webaim.org/) |
| WebAIM resources | [WebAIM Resources](https://webaim.org/resources/) |
| Apple accessibility guidance | [Apple HIG: Accessibility](https://developer.apple.com/design/human-interface-guidelines/accessibility) |
| Material accessibility | [Material Design Accessibility](https://m2.material.io/design/usability/accessibility.html) |
| Carbon accessibility | [Carbon Design System Accessibility](https://carbondesignsystem.com/guidelines/accessibility/overview/) |
| GOV.UK accessible services | [GOV.UK: Making your service accessible](https://www.gov.uk/service-manual/helping-people-to-use-your-service/making-your-service-accessible-an-introduction) |
| UVT accessibility for students with disabilities | [UVT: Accessibility for students with disabilities](https://uvt.ro/en/educatie/info-studenti-proces-educational/accesibilitate-pentru-studentii-cu-dizabilitati/) |
| UVT social inclusion | [UVT actively promotes social inclusion](https://www.uvt.ro/en/blog/uvt-promoveaza-activ-incluziunea-sociala/) |
| UVT tactile accessibility initiative | [UVT tactile models accessibility initiative](https://uvt.ro/en/comunicate-presa/in-cadrul-strategiei-institutionale-orientata-spre-accesibilizare-uvt-instaleaza-machetele-tactile-in-toate-spatiile-principale-din-sediul-principal/) |
| UVT Faculty of Informatics | [Faculty of Informatics UVT](https://info.uvt.ro/en/) |

^connections-accessibility-inclusive-design-end
