![[house.png|1000]]
# Design

This page is about design. The [[Experiment]] page checks whether the design works for real users. This page explains how to shape the interface so that fewer barriers appear in the first place.

> [!quote] Design rule
> Accessible design is not a decoration layer. It is a set of structural choices that help people perceive, operate, understand, and rely on a system.

## What inclusive design means here

Inclusive design starts from human variation. Users differ in vision, hearing, mobility, attention, language, memory, device access, technical skill, stress, fatigue, and context. A design becomes more inclusive when it reduces unnecessary demands on those users.

> What barrier could this page create, and how can the design remove or reduce that barrier?

This does not mean that one page can solve every accessibility need. It means that design choices should not create avoidable exclusion.

## Inclusive design map

```mermaid
flowchart TB
    A((Inclusive Design))

    A --> B[Information Structure]
    A --> C[Visual Access]
    A --> D[Interaction Access]
    A --> E[Language + Cognition]
    A --> F[Reusable Components]
    A --> G[Fallback Routes]
    A --> H[Accountability]

    B --> B1[Headings, landmarks,<br/>reading order]
    C --> C1[Contrast, type,<br/>spacing, diagrams]
    D --> D1[Keyboard, focus,<br/>target size]
    E --> E1[Plain language,<br/>labels, recovery]
    F --> F1[Links, tables,<br/>callouts, forms]
    G --> G1[Works when CSS<br/>or plugins fail]
    H --> H1[Document risks,<br/>choices, limits]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G,H node;
    class B1,C1,D1,E1,F1,G1,H1 detail;
```

## CS2023 grounding

CS2023 places accessibility inside HCI. In this guide, that means accessibility is part of how interactive systems are designed, implemented, evaluated, and justified. It is not an optional polish step after the interface is finished.

```mermaid
flowchart TB
    A((CS2023 Design Gate))

    A --> B[Accessibility]
    A --> C[System Design]
    A --> D[Evaluation]
    A --> E[Accountability]

    B --> B1[Human variation<br/>and access needs]
    C --> C1[Components, states,<br/>input, layout]
    D --> D1[Checks, tests,<br/>evidence]
    E --> E1[Responsibility,<br/>risk, repair]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

- **HCI-Accessibility:** Design for disability, assistive technology, flexible use, and participation
- **HCI-Design:** Build accessibility into navigation, layout, components, states, and prototypes
- **HCI-Evaluation:** Test whether access actually works in practice
- **HCI-Accountability:** Document design choices, remaining barriers, repair plans, and limits

## Local UVT design layer

## Principle 1: Start from exclusion

Inclusive design begins by asking who is excluded by the current design. The useful question is not “How can this look better?” The useful question is “What demand does this design make, and who cannot meet that demand?”

```mermaid
flowchart LR
    A[Design demand] --> B[Possible exclusion]
    B --> C[Barrier]
    C --> D[Alternative route]
    D --> E[Inclusive repair]

    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B,C,D node;
    class E final;
```

## Principle 2: Use POUR as a design skeleton

WCAG organises accessibility around four principles: perceivable, operable, understandable, and robust. These principles are useful for design because they turn accessibility into concrete interface questions.

```mermaid
flowchart TB
    A((POUR))

    A --> B[Perceivable]
    A --> C[Operable]
    A --> D[Understandable]
    A --> E[Robust]

    B --> B1[Can users access<br/>the information?]
    C --> C1[Can users control<br/>the interface?]
    D --> D1[Can users understand<br/>what to do?]
    E --> E1[Does it work across<br/>tools and contexts?]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

- **Perceivable:** Text, diagrams, labels, and sources must be readable and not depend only on colour
- **Operable:** Links and routes must be reachable by keyboard and not rely on hover-only behavior
- **Robust:** Markdown, links, assets, and CSS should remain usable across viewers

## Information structure design

Structure is part of accessibility. It helps screen reader users, keyboard users, tired students, and professors who scan the page quickly.

```mermaid
flowchart TB
    A((Information Structure))

    A --> B[Title]
    A --> C[Opening Meaning]
    A --> D[Headings]
    A --> E[Route Links]
    A --> F[Tables]
    A --> G[Academic Anchors]

    B --> B1[What page is this?]
    C --> C1[Why does it matter?]
    D --> D1[Where am I?]
    E --> E1[Where can I go?]
    F --> F1[How do ideas compare?]
    G --> G1[Why trust the page?]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Opening callout:** State the CS2023 label, page purpose, and local-global role
- **Headings:** Use headings as navigation, not decoration
- **Backlink:** Every page should have a clear route back to its area overview
- **Tables:** Use tables for comparisons and decisions
- **Academic anchors:** Separate curriculum, standards, research venues, practice guidance, and local UVT sources
- **End synthesis:** Close with one clear question or design principle

## Visual access design

Visual design should reduce effort. It should not ask the user to decode low contrast, crowded diagrams, tiny labels, or meaning carried only by colour.

```mermaid
flowchart TB
    A((Visual Access))

    A --> B[Contrast]
    A --> C[Typography]
    A --> D[Spacing]
    A --> E[Hierarchy]
    A --> F[Diagram Readability]
    A --> G[Non-Colour Meaning]

    B --> B1[Text and focus<br/>are visible]
    C --> C1[Readable size<br/>and line length]
    D --> D1[Clear grouping]
    E --> E1[Important content<br/>stands out]
    F --> F1[Compact nodes<br/>and clear labels]
    G --> G1[Labels carry<br/>the meaning]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

## Interaction access design

Interaction access means that users can act. A page is not accessible if users can read it but cannot move through it, open links, recover from mistakes, or understand where they are.

```mermaid
flowchart TB
    A((Interaction Access))

    A --> B[Keyboard Path]
    A --> C[Focus Visibility]
    A --> D[Target Size]
    A --> E[Link Clarity]
    A --> F[Recovery]
    A --> G[Input Flexibility]

    B --> B1[Tab, Enter,<br/>Shift + Tab]
    C --> C1[Current location<br/>is visible]
    D --> D1[Targets are easy<br/>to activate]
    E --> E1[Destination is clear]
    F --> F1[Back, undo,<br/>repair route]
    G --> G1[No single input<br/>method required]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

## Component design rules

Accessibility scales through components. A consistent accessible link pattern, table pattern, callout pattern, and diagram pattern improves the whole vault. A broken pattern spreads the same barrier across pages.

```mermaid
flowchart TB
    A((Accessible Components))

    A --> B[Link]
    A --> C[Button or Action]
    A --> D[Table]
    A --> E[Diagram]
    A --> F[Callout]
    A --> G[Source Block]

    B --> B1[Meaningful<br/>destination]
    C --> C1[Clear action<br/>and state]
    D --> D1[Headers and<br/>comparison]
    E --> E1[Readable and<br/>described]
    F --> F1[Purpose visible]
    G --> G1[Trust category<br/>clear]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Link:** Link text should describe the destination or purpose
- **Button or action:** The user should know what will happen before activation
- **Table:** Use a header row and keep comparisons simple
- **Diagram:** Keep it compact and repeat the core idea in text
- **Source block:** Group sources by role: curriculum, standard, research, local UVT, practice

## Accessible Mermaid design

```mermaid
flowchart TB
    A((Accessible Mermaid))

    A --> B[One Concept]
    A --> C[Compact Shape]
    A --> D[Readable Text]
    A --> E[No Colour-Only Meaning]
    A --> F[Text Alternative]

    B --> B1[No huge graph]
    C --> C1[Does not overflow]
    D --> D1[Dark text on<br/>light nodes]
    E --> E1[Labels carry<br/>meaning]
    F --> F1[Table or paragraph<br/>repeats idea]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

## Cognitive design rules

```mermaid
flowchart TB
    A((Cognitive Design))

    A --> B[Plain Meaning]
    A --> C[Consistent Labels]
    A --> D[Chunking]
    A --> E[Examples]
    A --> F[Memory Support]
    A --> G[Low Surprise]

    B --> B1[Translate metaphor]
    C --> C1[Use the same term<br/>across pages]
    D --> D1[Short sections]
    E --> E1[Concrete local<br/>examples]
    F --> F1[Repeat area purpose]
    G --> G1[Predictable structure]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **User forgets where they are:** Add consistent backlinks and area identity
- **User is overwhelmed by sources:** Group sources by type
- **User cannot connect local and global ideas:** Put UVT and global HCI in the same comparison table
- **User sees a diagram but misses the concept:** Add a short explanation after the diagram
- **User cannot distinguish theory from experiment:** Use page-role callouts at the top
- **User reads on a small screen:** Use shorter paragraphs and compact visual blocks

## Form and error design

Even if the current vault is mostly Markdown pages, accessibility design should include forms and errors. Real systems often ask users to enter, submit, correct, and recover.

```mermaid
flowchart TB
    A((Form + Error Design))

    A --> B[Label]
    A --> C[Instruction]
    A --> D[Validation]
    A --> E[Error Message]
    A --> F[Recovery]

    B --> B1[What is required?]
    C --> C1[How to complete it?]
    D --> D1[When is input checked?]
    E --> E1[What went wrong?]
    F --> F1[How can the user<br/>fix it?]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

- **Label:** Visible and programmatically connected to the input
- **Required field:** Marked in text, not only by colour
- **Instruction:** Placed before the user makes the error
- **Validation:** Does not erase user input
- **Error message:** Explains what happened and how to fix it
- **Focus after error:** Moves users to the problem or clearly identifies it
- **Recovery:** Allows correction without restarting

## Design-system tokens

```mermaid
flowchart TB
    A((Design Tokens))

    A --> B[Colour]
    A --> C[Typography]
    A --> D[Spacing]
    A --> E[Focus]
    A --> F[Motion]
    A --> G[Mermaid Classes]

    B --> B1[Contrast-safe pairs]
    C --> C1[Readable size<br/>and line height]
    D --> D1[Clear grouping]
    E --> E1[Visible keyboard state]
    F --> F1[Reduced motion option]
    G --> G1[Readable diagram nodes]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Text colour:** High contrast against the page background
- **Accent colour:** Helps emphasis but does not carry meaning alone
- **Background colour:** Supports long reading
- **Font size:** Large enough and user-adjustable
- **Line height:** Comfortable for academic pages
- **Focus outline:** Visible against all relevant backgrounds
- **Spacing:** Separates routes, sections, diagrams, and source blocks
- **Mermaid class:** Uses light fills and dark readable text

## Robustness and fallback design

## Recommended page pattern

```mermaid
flowchart TB
    A((Inclusive Page Pattern))

    A --> B[Title + CS2023 Label]
    B --> C[Real-Life Meaning]
    C --> D[Local Context]
    D --> E[Global Rule]
    E --> F[Design Pattern]
    F --> G[Barrier + Repair Table]
    G --> H[Academic Anchors]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class H final;
```

- **Title + CS2023 label:** Prevents metaphor confusion
- **Real-life meaning:** Gives immediate cognitive access
- **Local context:** Grounds the page in real users and tools
- **Global rule:** Connects the page to field knowledge
- **Design pattern:** Shows how to build the interface
- **Barrier + repair table:** Makes exclusion and repair visible
- **Academic anchors:** Shows source credibility

## Inclusive design checklist

Use this checklist before evaluation.

- **Does the page state its official CS2023 meaning?:** The academic label appears near the title
- **Is the heading structure logical?:** Headings describe the page path
- **Is link text meaningful?:** Links describe destination or purpose
- **Are diagrams readable?:** They are compact, light, high-contrast, and explained in text
- **Is colour used safely?:** Meaning does not depend only on colour
- **Can the page be navigated by keyboard?:** Links and controls are reachable and focus is visible
- **Is the text cognitively manageable?:** Sections are chunked and supported by examples
- **Does the page work without custom CSS?:** Core content remains readable in fallback view
- **Are local and global sources clear?:** UVT, CS2023, standards, venues, and practice sources are grouped

## Local and global design comparison

## Academic anchors

| Route | Source |
|---|---|
| CS2023 HCI Accessibility basis | [CS2023 HCI Version Gamma](https://csed.acm.org/wp-content/uploads/2023/09/HCI-Version-Gamma.pdf) |
| WCAG 2.2 standard | [W3C WCAG 2.2](https://www.w3.org/TR/WCAG22/) |
| WCAG overview | [W3C WAI WCAG 2 Overview](https://www.w3.org/WAI/standards-guidelines/wcag/) |
| WCAG quick reference | [How to Meet WCAG 2.2](https://www.w3.org/WAI/WCAG22/quickref/) |
| Understanding WCAG 2.2 | [W3C Understanding WCAG 2.2](https://www.w3.org/WAI/WCAG22/Understanding/) |
| WCAG techniques | [W3C WCAG Techniques](https://www.w3.org/WAI/WCAG22/Techniques/) |
| Accessibility principles | [W3C WAI Accessibility Principles](https://www.w3.org/WAI/fundamentals/accessibility-principles/) |
| Accessibility evaluation | [W3C Evaluating Web Accessibility](https://www.w3.org/WAI/test-evaluate/) |
| Inclusive design method | [Microsoft Inclusive Design](https://inclusive.microsoft.design/) |
| Inclusive design guidebook | [Microsoft Inclusive 101 Guidebook](https://inclusive.microsoft.design/tools-and-activities/Inclusive101Guidebook.pdf) |
| Universal Design principles | [The Center for Universal Design](https://design.ncsu.edu/research/center-for-universal-design/) |
| Ability-Based Design paper | [Ability-Based Design: Concept, Principles and Examples](https://kgajos.seas.harvard.edu/papers/wobbrock11abd.pdf) |
| Apple accessibility guidance | [Apple HIG: Accessibility](https://developer.apple.com/design/human-interface-guidelines/accessibility) |
| Apple inclusion guidance | [Apple HIG: Inclusion](https://developer.apple.com/design/human-interface-guidelines/inclusion) |
| Material accessibility | [Material Design Accessibility](https://m2.material.io/design/usability/accessibility.html) |
| Material target size guidance | [Material Design Structure](https://m3.material.io/foundations/designing/structure) |
| GOV.UK accessible services | [GOV.UK: Making your service accessible](https://www.gov.uk/service-manual/helping-people-to-use-your-service/making-your-service-accessible-an-introduction) |
| IBM Carbon accessibility | [Carbon Design System Accessibility](https://carbondesignsystem.com/guidelines/accessibility/overview/) |
| Practical accessibility | [WebAIM](https://webaim.org/) |
| Accessibility research community | [ACM SIGACCESS](https://www.sigaccess.org/) |
| Accessibility conference | [ACM ASSETS](https://dl.acm.org/conference/assets) |
| UVT accessibility for students with disabilities | [UVT: Accessibility for students with disabilities](https://uvt.ro/en/educatie/info-studenti-proces-educational/accesibilitate-pentru-studentii-cu-dizabilitati/) |
| UVT Faculty of Informatics | [Faculty of Informatics UVT](https://info.uvt.ro/en/) |

^design-accessibility-inclusive-design-end
