---
title: Theory
area: Interface Forge
category: Activities
cssclasses:
  - interface-forge
tags:
  - HCI
  - interface-theory
  - interaction-design
  - interface-principles
  - visual-hierarchy
  - affordances
  - feedback
  - navigation
  - design-systems
  - accessibility
status: polished-cognishire-draft
---
![[lake.gif|1000]]
# Theory

Back to [[../Overview|The Interface Forge]].

> [!abstract] Theory Forge
> Theory in the Interface Forge explains how interface form is built. It connects user understanding to layout, controls, states, navigation, components, design systems, responsiveness, and accessibility.

The [[01_Core_Area_HCI/001_Subareas/01_Understanding_the_User/Activities/Theory|Mind Library]] studies the user. It asks how people perceive, remember, learn, trust, recover, and act. The Interface Forge asks a more practical question: how should those human limits become interface structure?

This page is therefore about design-facing theory. It does not replace general HCI theory. It applies it to screens, flows, components, feedback, and systems. It explains why layout guides attention, why controls need signifiers, why system state must be visible, why navigation must support wayfinding, and why accessibility must be built into interface components.

> [!quote] Forge theory rule
> Interface theory is useful when it tells the designer what to make visible, what to constrain, what to test, and what to repair.

## Theory Forge Map

```mermaid
flowchart TB
    A((Theory Forge))

    A --> B[Structure]
    A --> C[Action]
    A --> D[State]
    A --> E[Navigation]
    A --> F[Access]

    B --> B1[Layout and hierarchy]
    C --> C1[Controls and signifiers]
    D --> D1[Feedback and recovery]
    E --> E1[Routes and labels]
    F --> F1[Inclusive operation]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

| Theory route | Interface question | Design consequence |
|---|---|---|
| Structure theory | How should information be organised? | Layout, grouping, hierarchy, spacing, and information architecture |
| Action theory | How does the user know what can be done? | Controls, affordances, signifiers, labels, and interaction cues |
| Navigation theory | How does the user move and stay oriented? | Menus, breadcrumbs, active states, internal links, and labels |
| Component theory | How does the interface stay consistent? | Components, variants, states, tokens, and documentation |
| Access theory | How does the interface work across abilities and technologies? | Keyboard access, contrast, focus order, semantics, and assistive technology support |

## Structure Theory: The Screen as an Organised Field


Visual hierarchy guides the eye toward important elements. In interface design, this is not only aesthetic. It affects whether users find the main action, understand the page, and predict the next step.

```mermaid
flowchart TB
    A((Structure Theory))

    A --> B[Grouping]
    A --> C[Hierarchy]
    A --> D[Alignment]
    A --> E[Spacing]

    B --> B1[Related items]
    C --> C1[Visible priority]
    D --> D1[Stable order]
    E --> E1[Clear separation]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

| Structural principle | Interface meaning | Failure pattern |
|---|---|---|
| Proximity | Nearby items are interpreted as related | Users group unrelated actions together |
| Similarity | Similar-looking items are read as similar in function | Decorative elements look interactive |
| Contrast | Strong difference signals importance | Primary actions disappear into the page |
| Alignment | Ordered placement communicates structure | The page feels accidental or unstable |
| Progressive disclosure | Detail appears when needed | Users are overloaded too early |

The practical theory is that the interface should reduce unnecessary interpretation. If users must scan repeatedly, compare too many equal elements, or guess what belongs together, the structure is forcing them to do extra cognitive work.

Useful routes: [NN/g on visual hierarchy](https://www.nngroup.com/articles/visual-hierarchy-ux-definition/), [NN/g on visual design principles](https://www.nngroup.com/articles/principles-visual-design/), and [Apple Human Interface Guidelines: Layout](https://developer.apple.com/design/human-interface-guidelines/layout).

## Action Theory: Controls Must Explain Themselves

Action theory concerns how users understand possible actions. A control works well only when the user can recognise what it is, what it does, and whether it is available.

Affordances are the possible actions a system offers. Signifiers are the visible or perceivable cues that show those actions. A button may technically afford clicking, but if it does not look clickable, the action is hidden. A card may look tappable but do nothing, creating a false affordance. A disabled button may prevent action but fail to explain why the action is unavailable.

```mermaid
flowchart LR
    A[Affordance] --> B[Signifier]
    B --> C[User action]
    C --> D[System response]
    D --> E[Action learned]

    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B,C,D node;
    class E final;
```

| Control type | Theoretical job | Interface check |
|---|---|---|
| Button | Makes a command visible | Label, contrast, state, and click target are clear |
| Link | Signals movement to another place or resource | Text describes the destination |
| Text field | Invites input | Label and expected format are visible |
| Toggle | Represents binary state | Current state and change effect are clear |
| Slider | Represents adjustable value | Range, value, and effect are understandable |
| Disabled control | Communicates unavailable action | Reason and path to availability are shown when useful |

The core theory is that users should not need accidental exploration to find basic actions. Exploration can be useful, but essential functions need strong signifiers, predictable behaviour, and immediate feedback.

Useful routes: [NN/g signifiers topic](https://www.nngroup.com/topic/signifiers/), [NN/g design-pattern guidelines](https://www.nngroup.com/articles/design-pattern-guidelines/), and Donald Norman’s writing on affordances and signifiers.

## State Theory: Interfaces Are Always Changing


Apple’s feedback guidance explains that clear, consistent feedback helps people understand what happens as they interact with an app. This is central to the Interface Forge because state is often invisible unless the designer expresses it through feedback.

```mermaid
flowchart LR
    A[Ready state] --> B[User action]
    B --> C[Processing]
    C --> D{Outcome}
    D --> E[Success]
    D --> F[Error]
    F --> G[Recovery]
    G --> A
    E --> A

    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B,C,G node;
    class D,F detail;
    class E final;
```

| Interface state | User question | Design requirement |
|---|---|---|
| Idle | What can I do now? | Available actions are visible |
| Loading | Is the system working? | Progress or processing feedback appears |
| Success | Did it work? | Confirmation and next step are clear |
| Error | What failed, and how do I repair it? | Message is visible, constructive, and specific |
| Empty | Why is nothing here? | Explain the state and offer the next action |
| Disabled | Why can I not do this? | Show the condition or requirement when useful |

State theory prevents silent change. If a system changes without clear feedback, the user must guess. That can create repeated clicking, duplicate submissions, anxiety, and mistrust.

Useful routes: [Apple HIG: Feedback](https://developer.apple.com/design/human-interface-guidelines/feedback), [NN/g 10 usability heuristics](https://www.nngroup.com/articles/ten-usability-heuristics/), and [NN/g error-message guidelines](https://www.nngroup.com/articles/error-message-guidelines/).

## Navigation Theory: Interfaces Need Wayfinding

Navigation theory treats the interface as a place the user moves through. The user needs to know where they are, what paths exist, what each path means, and how to return.

Navigation is more than a menu. It includes page titles, breadcrumbs, tabs, active states, search, internal links, labels, categories, cards, and information scent. Information scent means that users can predict whether a route is likely to lead to the desired content.

```mermaid
flowchart TB
    A((Navigation Theory))

    A --> B[Location]
    A --> C[Routes]
    A --> D[Labels]
    A --> E[Return path]

    B --> B1[Where am I?]
    C --> C1[Where can I go?]
    D --> D1[What will I find?]
    E --> E1[How do I recover?]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

| Navigation problem | User interpretation | Repair |
|---|---|---|
| Current location is hidden | “I am lost.” | Add active states, headings, or breadcrumbs |
| Labels are vague | “I cannot predict what is inside.” | Use task-based, user-centred language |
| Too many routes compete | “Everything looks equally important.” | Prioritise primary paths |
| Back path is unclear | “I might lose my work.” | Support safe return, undo, and saved state |
| Search is the only usable navigation | “The structure is not learnable.” | Improve categories and information architecture |

In this project, navigation theory matters because the vault itself is an interface. [[../../01_Understanding_the_User/Overview|Mind Library]], [[../Overview|Interface Forge]], [[../../03_Evaluating_the_Design/Overview|Observation Chamber]], [[../../04_Accessibility_and_Accountability/Overview|Inclusive Gate]], and [[../../05_Human_AI_Interaction/Overview|Oracle Engine]] should behave like meaningful regions, not random folders.

## Feedback and Error Theory: Failure Is Part of the Interface

Error theory begins with respect for the user. Errors are not only user mistakes. They often reveal mismatches between system expectations and human behaviour. A good interface prevents avoidable errors, detects problems early, and helps users recover without blame.

```mermaid
flowchart LR
    A[User action] --> B[System check]
    B --> C{Result}
    C --> D[Success feedback]
    C --> E[Error feedback]
    E --> F[Repair path]
    F --> A

    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B,F node;
    class C,E detail;
    class D final;
```

| Error principle | Interface theory | Example |
|---|---|---|
| Prevention | Avoid the error before it happens | Disable impossible dates |
| Visibility | Show the problem where it occurs | Inline field message |
| Constructive language | Explain repair, not blame | “Use at least 8 characters” |
| Efficiency | Let users fix without restarting | Keep valid fields filled |
| Recovery | Provide undo or safe reversal | Restore deleted item |

NN/g’s error-message guidance recommends messages that are visible, constructive, and respectful of user effort. This belongs in theory because error design expresses the system’s attitude toward the user. A hostile error message makes the user feel like the problem. A good error message treats the problem as repairable.

Useful routes: [NN/g error-message guidelines](https://www.nngroup.com/articles/error-message-guidelines/) and [NN/g error-message scoring rubric](https://www.nngroup.com/articles/error-messages-scoring-rubric/).

## Component Theory: Interfaces Are Built From Reusable Parts

Component theory explains how modern interfaces scale. A product is not built from isolated screens. It is built from repeated components: buttons, fields, cards, dialogs, tabs, navigation bars, lists, tables, tooltips, modals, and forms.

When components are consistent, users can transfer learning from one part of the system to another. When components change behaviour randomly, the interface becomes unstable. Consistency is therefore cognitive, not only visual.

```mermaid
flowchart TB
    A((Component Theory))

    A --> B[Component]
    A --> C[Variant]
    A --> D[State]
    A --> E[Rule]

    B --> B1[Reusable object]
    C --> C1[Different purpose]
    D --> D1[Idle, active, disabled]
    E --> E1[When to use it]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

| Component layer | What it controls | Why it matters |
|---|---|---|
| Component | The reusable interface object | Prevents rebuilding and inconsistency |
| Variant | Different forms of that object | Supports different contexts without chaos |
| State | The object’s behaviour over time | Shows availability, feedback, and response |
| Token | The design value behind appearance | Keeps colour, spacing, and type consistent |
| Documentation | The rule for use | Prevents misuse by designers and developers |

Useful routes: [Material Design components](https://m3.material.io/components), [Material Design foundations](https://m3.material.io/foundations), [Microsoft Fluent 2](https://fluent2.microsoft.design/), and [Fluent 2 design tokens](https://fluent2.microsoft.design/design-tokens).

## Design System Theory: Consistency Becomes Infrastructure

A design system is a theory of consistency made operational. It defines the shared language of an interface: components, tokens, patterns, accessibility rules, motion, content style, layout principles, and documentation.

Design systems matter because interface design often happens across teams, platforms, and time. Without shared rules, every screen becomes a new negotiation. With a stable system, designers and developers can build new flows while preserving predictable interaction.

```mermaid
flowchart TB
    A((Design System))

    A --> B[Tokens]
    A --> C[Components]
    A --> D[Patterns]
    A --> E[Guidelines]

    B --> B1[Colour, spacing, type]
    C --> C1[Buttons, fields, dialogs]
    D --> D1[Reusable flows]
    E --> E1[Rules and examples]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

| System element | Theory role | Practical question |
|---|---|---|
| Token | Stores a reusable design value | Is this colour or spacing used consistently? |
| Component | Stores a reusable interface object | Does this button behave the same everywhere? |
| Pattern | Stores a recurring interaction solution | Do similar tasks follow similar flows? |
| Guideline | Stores the rule behind usage | Does the team know when to use this element? |
| Accessibility rule | Stores inclusive requirements | Does every component support keyboard and screen reader use? |

Fluent 2 describes design tokens as flexible and accessibility-supporting, including support for light, dark, high-contrast, and branded themes. Material Design describes components and foundations as reusable resources for building user interfaces. These sources are useful because they show how interface theory becomes maintainable infrastructure.

## Accessibility Theory Inside the Forge

Accessibility theory in the Interface Forge is component-level. It asks whether the actual interface pieces can be perceived, operated, understood, and interpreted reliably by assistive technologies.

WCAG organises accessibility around four principles: perceivable, operable, understandable, and robust. In interface construction, these principles become practical questions about every component and state.

```mermaid
flowchart TB
    A((Access Theory))

    A --> B[Perceivable]
    A --> C[Operable]
    A --> D[Understandable]
    A --> E[Robust]

    B --> B1[Contrast and alternatives]
    C --> C1[Keyboard and focus]
    D --> D1[Labels and states]
    E --> E1[Semantic structure]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

| WCAG principle | Interface theory | Forge check |
|---|---|---|
| Perceivable | Users must be able to access information through available senses | Contrast, labels, captions, alternatives |
| Operable | Users must be able to use controls through available input methods | Keyboard access, focus order, target size |
| Understandable | Users must be able to predict and interpret interaction | Clear language, consistent states, helpful errors |
| Robust | Interface must work with assistive technologies | Semantic HTML, ARIA when needed, reliable structure |

Accessibility cannot be added only at the end because inaccessible components reproduce barriers everywhere they are reused. A design system with inaccessible buttons, fields, dialogs, and menus becomes a barrier factory.

Useful routes: [W3C Accessibility Principles](https://www.w3.org/WAI/fundamentals/accessibility-principles/), [WCAG 2.2](https://www.w3.org/TR/WCAG22/), [WCAG overview](https://www.w3.org/WAI/standards-guidelines/wcag/), and [Fluent 2 accessibility](https://fluent2.microsoft.design/accessibility).

## Responsive Theory: One Interface, Many Conditions

Responsive theory explains how an interface remains coherent across screen sizes, input modes, user settings, contexts, and accessibility needs. A desktop layout cannot simply be squeezed into mobile form. A hover interaction cannot be assumed on touch. A dense data screen may not work under time pressure or poor lighting.

```mermaid
flowchart TB
    A((Responsive Theory))

    A --> B[Screen]
    A --> C[Input]
    A --> D[Context]
    A --> E[Preference]

    B --> B1[Width and density]
    C --> C1[Mouse, touch, keyboard]
    D --> D1[Light, motion, noise]
    E --> E1[Text, contrast, motion]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

Material Design’s layout guidance discusses layout foundations and interaction patterns. Apple’s layout guidance emphasises designing for different Apple platforms and contexts. The theory is that responsiveness is not only resizing. It preserves task meaning across conditions.

## Platform Theory: Interfaces Live Inside Ecosystems

Platform theory explains why the same interface idea may need different expression on different systems. Users bring expectations from their operating system, device, and application ecosystem. A control that feels natural on iOS may feel foreign on desktop web. A keyboard shortcut may be expected by expert desktop users but irrelevant to a touch-first mobile flow.

```mermaid
flowchart TB
    A((Platform Theory))

    A --> B[Conventions]
    A --> C[Input expectations]
    A --> D[System components]
    A --> E[User habits]

    B --> B1[Native patterns]
    C --> C1[Touch, pointer, keyboard]
    D --> D1[Menus, sheets, dialogs]
    E --> E1[Learned behaviour]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

Platform guidance should not be copied mechanically, but it must be understood. Apple’s Human Interface Guidelines, Material Design, and Microsoft Fluent show how mature ecosystems document components, motion, layout, accessibility, and system behaviour.

## Theory-to-Prototype Loop

The final purpose of interface theory is not memorisation. It is better making. A theory becomes useful only when it generates a design choice that can be prototyped and tested.

```mermaid
flowchart LR
    A[Theory] --> B[Design principle]
    B --> C[Interface decision]
    C --> D[Prototype]
    D --> E[Test]
    E --> F[Refine]

    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B,C,D,E node;
    class F final;
```

| Theory | Prototype decision | Test question |
|---|---|---|
| Visual hierarchy | Make the primary action visually dominant | Do users notice the correct action first? |
| Signifiers | Add clearer button states and labels | Do users understand what is clickable? |
| Feedback | Add loading, success, and error states | Do users know what happened? |
| Navigation | Add active state and clearer labels | Can users find the target page? |
| Accessibility | Add keyboard focus and semantic labels | Can assistive technology users operate the flow? |
| Design system | Use consistent components | Do repeated patterns behave predictably? |

This loop connects the Interface Forge to the [[../../03_Evaluating_the_Design/Overview|Observation Chamber]], where prototypes are tested, and to the [[../../04_Accessibility_and_Accountability/Overview|Inclusive Gate]], where interface theory is checked against accessibility and ethics.

## Cognishire Application

The Cognishire vault is itself an interface. The theory on this page can be used to check whether the vault is readable, navigable, consistent, and accessible.

| Theory route | Cognishire design check |
|---|---|
| Structure | Are headings, diagrams, callouts, and tables visually ordered? |
| Action | Do links look meaningful and lead to expected places? |
| State | Does the user know when they are in a room, subarea, or activity page? |
| Navigation | Can the user move from the five rooms to a specific concept and back? |
| Component | Do repeated callouts, diagrams, and tables behave consistently? |
| Accessibility | Can the theme be read with enough contrast and used with keyboard navigation? |

This gives the Interface Forge a practical role inside the project. It is not only a chapter about interface design. It is also a checklist for improving the vault as a learning system.

## Academic anchors

| Route | Trusted source |
|---|---|
| Human-centred design | [ISO 9241-210](https://www.iso.org/standard/77520.html) |
| Human-centred design context | [NIST Human-Centered Design](https://www.nist.gov/itl/iad/visualization-and-usability-group/human-factors-human-centered-design) |
| Usability heuristics | [NN/g: 10 Usability Heuristics](https://www.nngroup.com/articles/ten-usability-heuristics/) |
| Visual hierarchy | [NN/g: Visual Hierarchy in UX](https://www.nngroup.com/articles/visual-hierarchy-ux-definition/) |
| Visual design principles | [NN/g: 5 Principles of Visual Design](https://www.nngroup.com/articles/principles-visual-design/) |
| Interface patterns | [NN/g: Design-Pattern Guidelines](https://www.nngroup.com/articles/design-pattern-guidelines/) |
| Error messages | [NN/g: Error-Message Guidelines](https://www.nngroup.com/articles/error-message-guidelines/) |
| Accessibility principles | [W3C Accessibility Principles](https://www.w3.org/WAI/fundamentals/accessibility-principles/) |
| Accessibility standard | [WCAG 2.2](https://www.w3.org/TR/WCAG22/) |
| Material design foundations | [Material Design 3 Foundations](https://m3.material.io/foundations) |
| Material components | [Material Design 3 Components](https://m3.material.io/components) |
| Apple platform guidance | [Apple Human Interface Guidelines](https://developer.apple.com/design/human-interface-guidelines) |
| Apple feedback guidance | [Apple HIG: Feedback](https://developer.apple.com/design/human-interface-guidelines/feedback) |
| Microsoft design system | [Fluent 2 Design System](https://fluent2.microsoft.design/) |
| Design tokens | [Fluent 2 Design Tokens](https://fluent2.microsoft.design/design-tokens) |
| Prototyping and design practice | [Stanford d.school Tools](https://dschool.stanford.edu/innovate/tools) |

^theory-interface-forge-end
