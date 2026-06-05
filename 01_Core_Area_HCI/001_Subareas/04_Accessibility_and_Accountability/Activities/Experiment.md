![[turtle.jpg|1000]]
# Experiment

The real CS2023 label is **HCI-Accessibility: Accessibility and Inclusive Design**.  
The connected responsibility route is **HCI-Accountability: Accountability and Responsibility in Design**.  
The real-life meaning is **collecting evidence about who can perceive, operate, understand, and rely on an interactive system**.

This page goes beyond running one automated accessibility checker. Automated tools are useful, but they detect only part of the problem. Inclusive experimentation also needs manual inspection, keyboard testing, screen reader checks, cognitive accessibility tasks, local user feedback, and honest reporting about what was not tested.

> [!quote] Lab rule
> An accessibility experiment is useful when it reveals barriers clearly enough that the design can be repaired and retested.

## Experiment Map

```mermaid
flowchart TB
    A((Inclusive Experiment Lab))

    A --> B[Automated Scan]
    A --> C[Manual Review]
    A --> D[Keyboard Trial]
    A --> E[Assistive Technology Check]
    A --> F[Cognitive Access Trial]
    A --> G[Local UVT Study]
    A --> H[Repair + Retest]

    B --> B1[Detect visible rule violations]
    C --> C1[Inspect structure and meaning]
    D --> D1[Test operability]
    E --> E1[Test real tool behaviour]
    F --> F1[Test understanding and overload]
    G --> G1[Test with local students and professor context]
    H --> H1[Fix barriers and check again]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef method fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G,H method;
    class B1,C1,D1,E1,F1,G1,H1 detail;
```

## CS2023 Experiment Gate

CS2023 treats accessibility and inclusive design as part of HCI, and evaluation as part of deciding whether a design works. This experiment page connects those units. Accessibility concepts must become testable evidence.

```mermaid
flowchart TB
    A((CS2023 HCI))

    A --> B[Accessibility + Inclusive Design]
    A --> C[Evaluating the Design]
    A --> D[Accountability]

    B --> B1[Standards, assistive tech, inclusive frameworks]
    C --> C1[Testing, observation, evidence, interpretation]
    D --> D1[Responsibility, harm, fairness, reporting]

    B --> E[Inclusive experiment]
    C --> E
    D --> E

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef area fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D area;
    class B1,C1,D1 detail;
    class E final;
```

- **Accessibility standards:** Test selected pages against WCAG-oriented criteria
- **Assistive technologies:** Check screen reader, keyboard, zoom, and other relevant access paths
- **Inclusive frameworks:** Identify who is excluded and what mismatch creates the barrier
- **Universal design:** Test whether one design supports multiple ways of using it
- **Accountability:** Record evidence, limits, risk, and responsibility honestly
- **Evaluation methods:** Use tasks, observation, metrics, notes, and repair cycles

## Local UVT Experiment Layer

## Experiment Protocol Spine

Every experiment in this page should follow the same spine.

```mermaid
flowchart TB
    A((Protocol Spine))

    A --> B[Barrier Hypothesis]
    B --> C[Test Task]
    C --> D[Evidence]
    D --> E[Finding]
    E --> F[Repair]
    F --> G[Retest]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef step fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef repair fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E step;
    class F,G repair;
```

## Experiment I: Automated Accessibility Scan

An automated scan is a useful starting point, not a complete experiment. It can identify some missing labels, contrast issues, heading problems, and code-level barriers. It cannot understand all design meaning, cognitive load, assistive-technology behaviour, or user experience.

```mermaid
flowchart TB
    A((Automated Scan))

    A --> B[Select page]
    B --> C[Run checker]
    C --> D[Record issues]
    D --> E[Classify severity]
    E --> F[Manual verification]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef step fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E step;
    class F final;
```

## Experiment II: Keyboard-Only Navigation Trial

Keyboard access is a core operability test. The user should complete main tasks without a mouse.

```mermaid
flowchart LR
    A[Tester uses keyboard] --> B[Page focus moves]
    B --> C[User activates links<br/>and controls]
    C --> D[Tester records success,<br/>traps, skipped content,<br/>and focus problems]

    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A,B,C node;
    class D detail;
```

- **Open the overview page:** User can reach and activate the target link
- **Move through page links:** Focus order follows visible reading order
- **Open a source link:** Link can be reached and activated without mouse
- **Return to previous page:** User can navigate back without losing context
- **Read a Mermaid diagram section:** User can skip past the diagram or access equivalent explanation
- **Complete a local navigation task:** User can find Theory, Experiment, Local and Global, and Open Problems

- **Invisible focus:** User cannot see where keyboard focus is
- **Keyboard trap:** User enters a component and cannot leave
- **Illogical order:** Focus jumps unpredictably
- **Mouse-only action:** An action cannot be completed from keyboard
- **Ambiguous link text:** User cannot tell where a link goes
- **Overloaded navigation:** Too many links create fatigue without structure

## Experiment III: Screen Reader Structure Check

A screen reader structure check tests whether the page has meaningful structure. This also supports navigation, search, scanning, and fallback reading. Good semantic structure also improves navigation, search, scanning, and robustness.

```mermaid
flowchart TB
    A((Screen Reader Check))

    A --> B[Headings]
    A --> C[Links]
    A --> D[Tables]
    A --> E[Diagrams]
    A --> F[Reading Order]

    B --> B1[Logical hierarchy]
    C --> C1[Meaningful destination]
    D --> D1[Headers and readable cells]
    E --> E1[Text alternative or explanation]
    F --> F1[Content makes sense in order]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef target fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;
    classDef check fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F target;
    class B1,C1,D1,E1,F1 check;
```

- **Heading navigation:** Can the user jump by headings and understand the page structure?
- **Link text:** Does the link text describe the destination without needing surrounding text?
- **Table reading:** Are table headers meaningful and not decorative only?
- **Diagram fallback:** Is the diagram explained in nearby text or table?
- **Source section:** Can the user identify official sources, standards, research venues, and practice sources?
- **Reading order:** Does the page make sense from top to bottom without visual layout?

For a Markdown vault, the core repair is often structural: use real headings, meaningful links, tables with headers, and explanation near diagrams.

## Experiment IV: Contrast, Zoom, and Visual Readability

Visual accessibility includes more than colour. It includes contrast, font size, spacing, diagram text, line length, theme dependence, and readability after zooming.

```mermaid
flowchart TB
    A((Visual Readability Test))

    A --> B[Contrast]
    A --> C[Zoom]
    A --> D[Diagram Text]
    A --> E[Theme Failure]
    A --> F[Projector View]

    B --> B1[Text visible against background]
    C --> C1[Readable at larger sizes]
    D --> D1[Dark text on light nodes and compact diagrams]
    E --> E1[Content still usable without CSS]
    F --> F1[Readable in classroom conditions]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef test fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef evidence fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F test;
    class B1,C1,D1,E1,F1 evidence;
```

- **Normal text contrast:** Text has sufficient contrast against the background
- **Link contrast:** Links are visible and distinguishable
- **Focus visibility:** Keyboard focus is clearly visible
- **Zoom to 200%:** Content remains readable without horizontal scrolling where possible
- **Diagram readability:** Mermaid text is readable, compact, and not dependent on colour alone
- **Theme disabled:** Main content still works when CSS or theme styling fails
- **Projector test:** Title, callouts, diagrams, and tables remain legible from classroom distance

## Experiment V: Cognitive Accessibility Comprehension Trial

```mermaid
flowchart TB
    A((Comprehension Trial))

    A --> B[Read section]
    B --> C[Explain meaning]
    C --> D[Find route]
    D --> E[Answer concept question]
    E --> F[Confidence rating]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef step fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E step;
    class F final;
```

## Experiment VI: Inclusive Mismatch Probe

The mismatch probe asks where the design demands something that some users cannot provide.

```mermaid
flowchart TB
    A((Mismatch Probe))

    A --> B[What does the system demand?]
    B --> C[Who may not be able to meet that demand?]
    C --> D[What barrier appears?]
    D --> E[What alternative route exists?]
    E --> F[What repair is needed?]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef probe fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef repair fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E probe;
    class F repair;
```

## Experiment VII: Diagram Accessibility Experiment

```mermaid
flowchart TB
    A((Diagram Test))

    A --> B[Diagram Version]
    A --> C[Text/Table Version]
    B --> D[Comprehension Question]
    C --> D
    D --> E[Compare Results]
    E --> F[Repair Diagram]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef condition fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef result fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E condition;
    class F result;
```

## Experiment VIII: Local UVT Accessibility Trial

```mermaid
flowchart TB
    A((UVT Accessibility Trial))

    A --> B[3 local users]
    B --> C[Navigation task]
    C --> D[Comprehension task]
    D --> E[Keyboard pass]
    E --> F[Visual readability pass]
    F --> G[Issue log]
    G --> H[Repair list]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef step fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G step;
    class H final;
```

## Experiment IX: Assistive Technology Smoke Test

A smoke test is a small first pass. It does not replace expert testing or disabled-user testing, but it catches obvious failures.

```mermaid
flowchart TB
    A((Assistive Tech Smoke Test))

    A --> B[Screen Reader]
    A --> C[Keyboard]
    A --> D[Zoom]
    A --> E[Reduced Motion]
    A --> F[High Contrast]

    B --> B1[Headings, links, order]
    C --> C1[Reach and operate]
    D --> D1[Readable when enlarged]
    E --> E1[No essential motion]
    F --> F1[Visible content and focus]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef tool fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef check fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F tool;
    class B1,C1,D1,E1,F1 check;
```

- **Screen reader:** Navigate headings, links, and tables on one page
- **Keyboard:** Complete one page-finding task without mouse
- **Browser zoom:** Increase zoom and inspect wrapping, scrolling, and diagram readability
- **High contrast mode:** Check whether text, links, and focus remain visible
- **Reduced motion:** Confirm that no critical information depends on animation
- **Plain Markdown fallback:** Check whether the page still makes sense if CSS fails

## Experiment X: Accountability Report

An inclusive experiment must report limits. This is where accessibility connects to accountability.

```mermaid
flowchart TB
    A((Accountability Report))

    A --> B[What was tested]
    A --> C[Who was included]
    A --> D[Who was missing]
    A --> E[What failed]
    A --> F[What was repaired]
    A --> G[What still needs testing]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef report fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef risk fill:#ffe0dc,stroke:#d68080,color:#2b160b,stroke-width:2px;
    classDef repair fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,E,F,G report;
    class D risk;
```

- **Scope:** Which pages, tools, devices, and views were tested
- **Participants:** Who participated and what user groups were not represented
- **Methods:** Automated scan, manual review, keyboard test, comprehension task, screen reader check
- **Findings:** Barrier, evidence, affected users, severity, and location
- **Repairs:** What changed in the design
- **Retest:** Whether the repair was checked again
- **Limits:** What the study cannot prove
- **Next step:** What should be tested later

## Evidence Matrix

## Issue Log Template

## Academic Anchors

| Route | Source |
|---|---|
| CS2023 HCI Accessibility basis | [CS2023 HCI Version Gamma](https://csed.acm.org/wp-content/uploads/2023/09/HCI-Version-Gamma.pdf) |
| WCAG 2.2 standard | [W3C WCAG 2.2](https://www.w3.org/TR/WCAG22/) |
| WCAG overview | [W3C WCAG Overview](https://www.w3.org/WAI/standards-guidelines/wcag/) |
| Accessibility principles | [W3C WAI Accessibility Principles](https://www.w3.org/WAI/fundamentals/accessibility-principles/) |
| First accessibility checks | [W3C Easy Checks](https://www.w3.org/WAI/test-evaluate/preliminary/) |
| Accessibility evaluation overview | [W3C Evaluating Web Accessibility](https://www.w3.org/WAI/test-evaluate/) |
| WCAG conformance evaluation | [W3C WCAG-EM Overview](https://www.w3.org/WAI/test-evaluate/conformance/wcag-em/) |
| ARIA authoring practices | [WAI-ARIA Authoring Practices Guide](https://www.w3.org/WAI/ARIA/apg/) |
| Inclusive design method | [Microsoft Inclusive Design](https://inclusive.microsoft.design/) |
| Ability-Based Design paper | [Ability-Based Design: Concept, Principles and Examples](https://kgajos.seas.harvard.edu/papers/wobbrock11abd.pdf) |
| Accessibility research community | [ACM SIGACCESS](https://www.sigaccess.org/) |
| Accessibility conference | [ACM ASSETS](https://dl.acm.org/conference/assets) |
| Web accessibility conference | [Web4All](https://www.w4a.info/) |
| Practical accessibility resource | [WebAIM](https://webaim.org/) |
| UVT accessibility for students with disabilities | [UVT: Accessibility for students with disabilities](https://uvt.ro/en/educatie/info-studenti-proces-educational/accesibilitate-pentru-studentii-cu-dizabilitati/) |
| UVT Faculty of Informatics | [Faculty of Informatics UVT](https://info.uvt.ro/en/) |

^experiment-accessibility-inclusive-design-end
