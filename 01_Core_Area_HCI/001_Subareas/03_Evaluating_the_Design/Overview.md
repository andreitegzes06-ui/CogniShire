![[experiment_room.jpg|1000]]
# Evaluating the Design

The local dimension is the **Faculty of Informatics / Computer Science context at UVT**.  
The global dimension is the wider HCI evaluation field: CS2023, CHI, UXPA, ASSETS, CSCW, ESEM, W3C/WCAG, usability testing, validity, accessibility evaluation, reproducibility, and long-term evidence.

> [!quote] Section rule
> A design is not good because it looks good. It is good when evidence shows that real users can understand it, use it, recover from problems, and reach their goals in a defined context.

## What this area does

> What evidence shows that this design works, and what are the limits of that evidence?

A design can be attractive and still fail. Users may not understand the labels. They may take too long to find a page. They may use the system only because the researcher helps them. They may complete a task but feel uncertain. They may be excluded by poor contrast, missing headings, broken keyboard navigation, or a diagram that cannot be read by assistive technology.

Evaluation turns these problems into evidence. It helps a student move from opinion to method.

## Section entrance

## Area identity

## What this area measures

```mermaid
flowchart TB
    A((Evaluation Evidence))

    A --> B[Effectiveness]
    A --> C[Efficiency]
    A --> D[Satisfaction]
    A --> E[Accessibility]
    A --> F[Understanding]
    A --> G[Trust]

    B --> B1[Can users finish<br/>the goal?]
    C --> C1[How much time<br/>and effort?]
    D --> D1[How acceptable<br/>is the experience?]
    E --> E1[Who can perceive<br/>and operate it?]
    F --> F1[Do users know<br/>what it means?]
    G --> G1[Do users rely on it<br/>appropriately?]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

## Local UVT evaluation layer

## Global HCI evaluation layer

- **CS2023 HCI-Evaluation:** Official Computer Science curriculum structure for evaluation methods and learning outcomes
- **ISO 9241-11:** Usability framing around effectiveness, efficiency, satisfaction, users, goals, and context of use
- **NN/g / UXPA / JUS / MeasuringU:** Applied usability methods, task testing, severity ratings, and UX metrics
- **W3C / WCAG / ASSETS / WebAIM:** Accessibility evaluation, standards, assistive technology, and inclusive testing
- **CHI / TOCHI / PACM HCI / IJHCS:** Peer-reviewed HCI evaluation research
- **CSCW / IMWUT:** Field studies, social contexts, long-term use, and situated evaluation
- **ESEM / MSR:** Software-system, workflow, repository, and tool-evaluation methods

## The evidence engine

```mermaid
flowchart LR
    A[Design enters] --> B[User acts]
    B --> C[Observation records]
    C --> D[Method organises]
    E --> F[Revision repairs]
    F --> G[New version tested]

    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B,C,D,E,F node;
    class G final;
```

```mermaid
flowchart TB

    A --> B[Observation]
    B --> C[Pattern]
    C --> D[Finding]

    B --> B1[One user was confused]
    C --> C1[Several local users<br/>were confused]
    D --> D1[The label creates<br/>uncertainty]
    E --> E1[UVT test supports<br/>revision]
    F --> F1[Needs broader<br/>evidence]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

## Section trial: minimal local study

```mermaid
flowchart TB
    A((Minimal UVT Trial))

    A --> B[3 to 5 local users]
    B --> C[4 navigation tasks]
    C --> D[2 explanation tasks]
    D --> E[1 accessibility pass]
    E --> F[1 clone/setup test]
    F --> G[Revision list]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class G final;
```

## Validity watch

```mermaid
flowchart TB
    A((Validity Watch))

    A --> B[Construct Validity]
    A --> C[Internal Validity]
    A --> D[External Validity]
    A --> E[Ecological Validity]
    A --> F[Accessibility Validity]

    B --> B1[Are we measuring<br/>the right thing?]
    C --> C1[What caused<br/>the result?]
    D --> D1[Who does this<br/>apply to?]
    E --> E1[Does it match<br/>real use?]
    F --> F1[Who can use it?]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

## Portfolio value

This area is useful for career preparation because evaluation produces artifacts that show method skill. A student interested in UX research, accessibility evaluation, HCI research, empirical software engineering, or human-AI evaluation should save the materials, not only the final design.

- **Evaluation protocol:** You can plan a study before collecting data
- **Task script:** You can write user tasks without leading the participant
- **Observation sheet:** You can collect behavioural evidence
- **Issue log:** You can turn observations into repair priorities
- **Accessibility checklist:** You understand access as part of evaluation
- **Clone/setup test:** You can evaluate portability and reproducibility
- **Before/after screenshots:** You can show design iteration

## Academic anchors

| Route | Source |
|---|---|
| CS2023 HCI-Evaluation | [CS2023 HCI SIGCSE 2022 version](https://csed.acm.org/knowledge-areas-human-computer-interaction-hci-sigcse-2022-version/) |
| CS2023 HCI Version Gamma | [Human-Computer Interaction PDF](https://csed.acm.org/wp-content/uploads/2023/09/HCI-Version-Gamma.pdf) |
| CS2023 Knowledge Areas | [CS2023 Knowledge Areas](https://csed.acm.org/knowledge-areas/) |
| UVT Faculty of Informatics | [Faculty of Informatics UVT](https://info.uvt.ro/en/) |
| UVT Faculty departments | [Faculty of Informatics Departments](https://info.uvt.ro/en/departamente/) |
| UVT CSAI Department | [Department of Computational Sciences and Artificial Intelligence](https://info.uvt.ro/en/departamente/csai/) |
| UVT DTSE Department | [Department of Digital Technologies and Software Engineering](https://info.uvt.ro/en/departamente/dtse/) |
| UVT researcher routes | [UVT Informatics Researchers](https://research.info.uvt.ro/researchers/) |
| Usability and context of use | [ISO 9241-11](https://www.iso.org/obp/ui/) |
| Usability definition route | [NIST usability glossary](https://csrc.nist.gov/glossary/term/usability) |
| Usability testing | [NN/g: Usability Testing 101](https://www.nngroup.com/articles/usability-testing-101/) |
| UX method selection | [NN/g: Which UX Research Methods to Use](https://www.nngroup.com/articles/which-ux-research-methods/) |
| UX metrics | [MeasuringU Essential Metrics](https://measuringu.com/essential-metrics/) |
| Accessibility evaluation | [W3C: Evaluating Web Accessibility Overview](https://www.w3.org/WAI/test-evaluate/) |
| Accessibility standard | [WCAG 2.2](https://www.w3.org/TR/WCAG22/) |
| WCAG understanding documents | [Understanding WCAG 2.2](https://www.w3.org/WAI/WCAG22/Understanding/) |
| Core HCI venue | [ACM CHI](https://dl.acm.org/conference/chi) |
| Accessibility research venue | [ACM ASSETS](https://dl.acm.org/conference/assets) |
| Empirical software evaluation | [ESEM](https://www.esem-conferences.org/) |
| Field and social evaluation | [ACM CSCW](https://cscw.acm.org/) |
| HCI archival journal | [ACM TOCHI](https://dl.acm.org/journal/tochi) |
| HCI proceedings journal | [PACM HCI](https://dl.acm.org/journal/pacmhci) |

^overview-evaluating-design-cool-end
