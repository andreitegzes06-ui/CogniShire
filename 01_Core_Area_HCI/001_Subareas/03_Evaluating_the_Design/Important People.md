---
title: Important People
area: Evaluating the Design
category: Researcher Roadmap
cs2023_unit: HCI-Evaluation
cssclasses:
tags:
  - HCI
  - CS2023
  - HCI-Evaluation
  - important-people
  - usability-testing
  - UX-metrics
  - evaluation-methods
  - accessibility-evaluation
  - research-methods
  - qualitative-methods
  - quantitative-methods
  - professor-roadmap
status: expanded-polished-draft
---
![[suns.jpg|1000]]
# Important People

> [!abstract] Researcher Roadmap
> This page is a study map for **CS2023 HCI-Evaluation: Evaluating the Design**. It points to researchers and practitioners whose work can help you learn usability testing, UX metrics, study validity, accessibility evaluation, field studies, and experience evaluation.

The academic label is **HCI-Evaluation: Evaluating the Design**.  
The practical question is simple: **Who should I read if I want to learn how interactive systems are evaluated?**

## Roadmap Compass

```mermaid
flowchart TB
    A((Evaluation People))

    A --> B[Usability testing]
    A --> C[UX metrics]
    A --> D[Validity and methods]
    A --> E[Accessibility evaluation]
    A --> F[Field evaluation]
    A --> G[Experience evaluation]

    B --> B1[Nielsen<br/>Molich<br/>Hertzum]
    C --> C1[Sauro<br/>Lewis<br/>Law]
    D --> D1[Hornbæk<br/>Lazar<br/>Wobbrock]
    E --> E1[Lazar<br/>Wobbrock<br/>Findlater]
    F --> F1[Rogers<br/>Fitzpatrick]
    G --> G1[Hassenzahl<br/>Law]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

## CS2023 Evaluation Anchor

CS2023 describes HCI-Evaluation as a unit about evaluating design with users and evidence. It includes formative and summative evaluation, qualitative and quantitative methods, usability evaluation, observation, interviews, surveys, focus groups, study planning, hypothesis design, and defensible conclusions.

```mermaid
flowchart TB
    A((CS2023<br/>HCI-Evaluation))

    A --> B[Formative evaluation]
    A --> C[Summative evaluation]
    A --> D[Qualitative evidence]
    A --> E[Quantitative evidence]

    B --> B1[Improve during design]
    C --> C1[Judge a finished design]
    D --> D1[Explain user behaviour]
    E --> E1[Measure and compare]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

The people below are organised around this curriculum logic. Some are professors. Some are professional researchers or consultants. The shared value is methodological: each route helps you decide what to test, how to test it, and how far your evidence can support your conclusion.

## Route I: Usability Testing and Evaluation Practice

Usability testing examines how people use an interface to complete tasks. It helps evaluators find breakdowns, confusion, delays, and errors. In HCI, this route matters because a design can look clear to its creator and still fail during real use.

### Jakob Nielsen

- **Main context:** Nielsen Norman Group; UX Tigers
- **Current status:** Co-founder of NN/g; retired from NN/g in 2023
- **Evaluation focus:** Usability testing, heuristic evaluation, web usability, practical UX guidance
- **Why to read him:** Nielsen helped make usability methods teachable and usable in industry settings
- **Best first reading:** NN/g articles on usability testing, heuristic evaluation, severity ratings, and method choice
- **Use with care:** Use this route for applied method vocabulary. Do not treat every NN/g rule as a universal law
- **Official sources:** [NN/g profile](https://www.nngroup.com/people/jakob-nielsen/), [NN/g Jakob Nielsen articles](https://www.nngroup.com/articles/author/jakob-nielsen/), [UX Tigers profile](https://www.uxtigers.com/about/people)

### Rolf Molich

- **Main context:** DialogDesign
- **Evaluation focus:** Comparative Usability Evaluation studies, usability test quality, evaluation reproducibility
- **Why to read him:** The CUE studies show that different usability teams can evaluate the same system and find different problems
- **What this teaches:** Usability findings depend on evaluator skill, method choices, task design, and reporting decisions
- **Best research use:** Compare two evaluation reports for the same interface and ask why their findings differ
- **Official sources:** [DialogDesign CUE Studies](https://www.dialogdesign.dk/cue-studies/), [About Rolf Molich](https://www.dialogdesign.dk/about-rolf-molich/), [ACM Interactions CUE article](https://dl.acm.org/doi/fullHtml/10.1145/3278154)

### Morten Hertzum

- **University:** Roskilde University
- **Public email:** `mhz@ruc.dk`
- **Current role:** Professor of Digital Technologies and Welfare
- **Evaluation focus:** Usability testing, HCI, CSCW, health informatics, information seeking, work systems
- **Why to read him:** Hertzum is useful when usability testing must be treated as a structured research method
- **Best first reading:** *Usability Testing: A Practitioner’s Guide to Evaluating the User Experience*
- **Before contacting:** Ask a focused question about usability testing, work systems, healthcare contexts, or CSCW
- **Official sources:** [Roskilde profile](https://forskning.ruc.dk/en/persons/mhz/), [personal page](https://mortenhertzum.dk/), [book record](https://forskning.ruc.dk/en/publications/usability-testing-a-practitioners-guide-to-evaluating-the-user-ex/)

## Route II: UX Metrics and Quantitative Evaluation

### Jeff Sauro

- **Organisation:** MeasuringU
- **Current role:** Founder and CEO
- **Evaluation focus:** Quantitative UX, usability metrics, benchmarking, survey interpretation, confidence intervals
- **Why to read him:** Sauro gives an applied route into making UX evidence measurable
- **Best first reading:** MeasuringU guides on task success, SUS, confidence intervals, sample size, and benchmarking
- **Use with care:** Metrics are useful only when the task, sample, and construct are clear
- **Official sources:** [MeasuringU About](https://measuringu.com/about/), [Jeff Sauro author page](https://measuringu.com/author/admin/), [Essential UX metrics](https://measuringu.com/essential-metrics/)

### James R. Lewis

- **Organisation:** MeasuringU; formerly IBM
- **Current role:** Distinguished User Experience Researcher at MeasuringU
- **Evaluation focus:** Perceived usability, SUS, CSUQ, UMUX, confidence intervals, sample size estimation
- **Why to read him:** Lewis is a strong route for standard questionnaires and practical statistics in usability studies
- **Best research use:** Choose a questionnaire, explain what it measures, and state what it cannot prove
- **Before contacting:** Ask about a measurement choice, not a general UX career question
- **Official sources:** [personal website](https://www.jimlewisux.com/), [MeasuringU author page](https://measuringu.com/author/james-r-lewis-phd/), [MeasuringU About](https://measuringu.com/about/)

### Effie Lai-Chong Law

- **University:** Durham University
- **Current role:** Professor in Human-Computer Interaction
- **Evaluation focus:** HCI methodologies, usability, user experience methodologies, games, learning technology evaluation
- **Why to read her:** Law connects UX evaluation with method choice and user-group differences
- **Best research use:** Compare whether different users experience the same system in different ways
- **Before contacting:** Ask about UX methodology, learning technologies, games, or evaluation design
- **Official sources:** [Durham profile](https://www.durham.ac.uk/staff/lai-chong-law/), [Durham HCI group](https://aihs.webspace.durham.ac.uk/human-computer-interaction/)

## Route III: Validity, HCI Methods, and Study Design

### Kasper Hornbæk

- **University:** University of Copenhagen
- **Public email:** `kash@di.ku.dk`
- **Current role:** Professor, Human-Centred Computing
- **Evaluation focus:** HCI, usability research, empirical methods, interaction theory, measurement
- **Best first reading:** Papers on usability measurement, HCI theory, empirical methods, and interaction research
- **Before contacting:** Ask a precise question about measures, theory, or study validity
- **Official sources:** [University of Copenhagen staff profile](https://di.ku.dk/english/staff/?pure=en%2Fpersons%2F141851), [personal research page](https://www.kasperhornbaek.dk/)

### Jonathan Lazar

- **University:** University of Maryland
- **Current role:** Professor in the College of Information; Executive Director of the Maryland Initiative for Digital Accessibility
- **Evaluation focus:** HCI research methods, ICT accessibility, user-centred design, assistive technologies, accessibility law and policy
- **Why to read him:** Lazar connects research methods with accessibility, policy, and social impact
- **Best first reading:** *Research Methods in Human-Computer Interaction* and work on digital accessibility
- **Before contacting:** Ask about research methods, accessibility evaluation, policy, or assistive technology
- **Official sources:** [UMD profile](https://ischool.umd.edu/directory/jonathan-lazar/), [MIDA](https://mida.umd.edu/)

### Jacob O. Wobbrock

- **University:** University of Washington
- **Public email:** `wobbrock@uw.edu`
- **Current role:** Professor in the Information School; Adjunct Professor in the Paul G. Allen School of Computer Science & Engineering; Director of ACE Lab
- **Evaluation focus:** HCI methods, accessible computing, input techniques, human performance measurement, interaction modelling
- **Why to read him:** Wobbrock is useful when an evaluation involves performance, input, accessibility, and statistical method choice
- **Best research use:** Evaluate an input technique and justify the task, measure, and analysis
- **Before contacting:** Bring a clear method question about an interaction technique or accessibility study
- **Official sources:** [UW personal page](https://faculty.washington.edu/wobbrock/), [CREATE profile](https://create.uw.edu/people-directors-wobbrock/)

## Route IV: Accessibility Evaluation

Accessibility evaluation asks whether people with disabilities can use the system. It includes standards checks, assistive technology testing, keyboard testing, user studies, and barrier analysis. In HCI, accessibility is a design and evaluation responsibility, not a final decoration.

### Leah Findlater

### Jonathan Lazar

- **Why repeated here:** Lazar links accessibility evaluation to process, policy, law, and user-centred design
- **Use this route when:** You need to explain accessibility as a technical, organisational, and legal issue
- **Good student task:** Build an accessibility issue log that records barrier, affected user, WCAG reference, and design repair
- **Official sources:** [UMD profile](https://ischool.umd.edu/directory/jonathan-lazar/), [MIDA](https://mida.umd.edu/)

### Jacob O. Wobbrock

- **Why repeated here:** Wobbrock’s work is especially relevant for accessible input, touch, gesture, text entry, and performance measurement
- **Use this route when:** You need to evaluate an interaction technique for people with different abilities
- **Good student task:** Compare two input methods using task success, time, error rate, and user comments
- **Official sources:** [UW personal page](https://faculty.washington.edu/wobbrock/), [CREATE profile](https://create.uw.edu/people-directors-wobbrock/)

## Route V: Field, Qualitative, and Real-World Evaluation

Field evaluation studies technology in natural or semi-natural settings. It looks at work practices, routines, social interaction, setting, and long-term use. This route matters because many HCI problems appear only when systems meet real context.

### Yvonne Rogers

- **University:** University College London, UCL Interaction Centre
- **Current role:** Professor of Interaction Design
- **Evaluation focus:** HCI, interaction design, ubiquitous computing, human-centred AI, research in the wild
- **Why to read her:** Rogers is a strong route for evaluating technology in everyday, learning, work, and public settings
- **Best first reading:** Work on interaction design, ubiquitous computing, and research in the wild
- **Best research use:** Design a field observation or classroom evaluation rather than a lab-only task
- **Official sources:** [UCL profile](https://profiles.ucl.ac.uk/33314-yvonne-rogers), [Royal Society profile](https://royalsociety.org/people/yvonne-rogers-35840/)

### Geraldine Fitzpatrick

- **Main public route:** TU Wien Informatics and personal website
- **Current wording:** Former Professor of Technology Design and Assessment and former Head of the HCI Group at TU Wien; public profile route remains available
- **Evaluation focus:** HCI, CSCW, technology design and assessment, health informatics, social interaction, collaboration
- **Why to read her:** Fitzpatrick is useful for evaluation that connects technical systems with social practice
- **Best research use:** Study how a technology fits into a collaborative, health, or everyday routine
- **Before contacting:** Use the public profile route and ask a focused question about social or health-related technology evaluation
- **Official sources:** [TU Wien profile](https://informatics.tuwien.ac.at/people/geraldine-fitzpatrick), [personal page](https://www.geraldinefitzpatrick.com/home/about-me/)

## Route VI: Experience, Meaning, and Affective Evaluation

Experience evaluation studies more than task completion. It asks whether interaction feels meaningful, motivating, pleasant, appropriate, or socially acceptable. This route is useful when a system is meant to support learning, creativity, wellbeing, entertainment, or long-term engagement.

### Marc Hassenzahl

### Effie Lai-Chong Law

- **Why repeated here:** Law is relevant for UX methodology and evaluation in games and learning systems
- **Use this route when:** Your system depends on enjoyment, motivation, perceived quality, or learning experience
- **Good student task:** Combine a small task study with an experience questionnaire and two interview questions
- **Official sources:** [Durham profile](https://www.durham.ac.uk/staff/lai-chong-law/), [Durham HCI group](https://aihs.webspace.durham.ac.uk/human-computer-interaction/)

## Study Route by Evaluation Interest

```mermaid
flowchart TB
    A((Choose a route))

    A --> B[Run a usability test]
    A --> C[Measure UX]
    A --> D[Design a valid study]
    A --> E[Test accessibility]
    A --> F[Study real use]
    A --> G[Evaluate experience]

    B --> B1[Nielsen<br/>Hertzum<br/>Molich]
    C --> C1[Sauro<br/>Lewis<br/>Law]
    D --> D1[Hornbæk<br/>Lazar<br/>Wobbrock]
    E --> E1[Lazar<br/>Wobbrock<br/>Findlater]
    F --> F1[Rogers<br/>Fitzpatrick]
    G --> G1[Hassenzahl<br/>Law]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **How to run a usability test:** start with...: Nielsen, Hertzum, Molich; build this small study: A 3-user think-aloud test with an issue log and severity ratings
- **How to quantify UX:** start with...: Sauro, Lewis, Law; build this small study: A small benchmark with task success, time, SUS, and confidence intervals
- **How to evaluate accessibility:** start with...: Lazar, Wobbrock, Findlater; build this small study: A keyboard test, screen reader check, WCAG issue log, and user-impact summary
- **How to study real use:** start with...: Rogers, Fitzpatrick; build this small study: A field observation or diary study in a real setting
- **How to evaluate experience:** start with...: Hassenzahl, Law; build this small study: A study that combines task evidence, experience ratings, and short interviews

## Contact Protocol

```mermaid
flowchart LR
    A[Pick topic] --> B[Read official profile]
    B --> C[Read one work]
    C --> D[Build one question]
    D --> E[Write short email]
    E --> F[Wait respectfully]
    F --> G[Use official route]

    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B,C,D,E,F node;
    class G final;
```

## Reading Sequence

- **1:** what to read: CS2023 HCI-Evaluation; why: Learn the official curriculum scope
- **2:** what to read: NN/g usability testing articles; why: Learn basic applied method vocabulary
- **3:** what to read: Hertzum or Lazar methods texts; why: Learn structured research-method thinking
- **4:** what to read: Sauro and Lewis on UX metrics; why: Learn quantitative UX measurement
- **5:** what to read: Hornbæk and Wobbrock; why: Learn validity, measurement, and method limits
- **6:** what to read: W3C/WCAG plus Lazar, Findlater, and Wobbrock; why: Learn accessibility evaluation
- **7:** what to read: Rogers and Fitzpatrick; why: Learn field and qualitative evaluation
- **8:** what to read: Hassenzahl and Law; why: Learn experience and meaning-focused evaluation

## Academic Anchors

| Route | Source |
|---|---|
| CS2023 HCI-Evaluation basis | [CS2023 HCI Version Gamma PDF](https://csed.acm.org/wp-content/uploads/2023/09/HCI-Version-Gamma.pdf) |
| Human-centred design standard | [ISO 9241-210:2019](https://www.iso.org/standard/77520.html) |
| Human-centred design summary | [NIST Human Centered Design](https://www.nist.gov/itl/iad/human-centered-technologies/human-factors-human-centered-design) |
| Accessibility standard | [W3C WCAG 2.2](https://www.w3.org/TR/WCAG22/) |
| WCAG overview | [W3C WAI WCAG Overview](https://www.w3.org/WAI/standards-guidelines/wcag/) |
| Applied usability methods | [Nielsen Norman Group Articles](https://www.nngroup.com/articles/) |
| Jakob Nielsen | [NN/g profile](https://www.nngroup.com/people/jakob-nielsen/) |
| Comparative Usability Evaluation | [DialogDesign CUE Studies](https://www.dialogdesign.dk/cue-studies/) |
| CUE reproducibility discussion | [ACM Interactions article](https://dl.acm.org/doi/fullHtml/10.1145/3278154) |
| Morten Hertzum | [Roskilde University profile](https://forskning.ruc.dk/en/persons/mhz/) |
| Quantitative UX practice | [MeasuringU About](https://measuringu.com/about/) |
| Jeff Sauro | [MeasuringU author page](https://measuringu.com/author/admin/) |
| James R. Lewis | [personal website](https://www.jimlewisux.com/) |
| Effie Law | [Durham University profile](https://www.durham.ac.uk/staff/lai-chong-law/) |
| Kasper Hornbæk | [University of Copenhagen profile](https://di.ku.dk/english/staff/?pure=en%2Fpersons%2F141851) |
| Jonathan Lazar | [UMD profile](https://ischool.umd.edu/directory/jonathan-lazar/) |
| Jacob Wobbrock | [UW personal page](https://faculty.washington.edu/wobbrock/) |
| Leah Findlater | [UW HCDE profile](https://www.hcde.washington.edu/findlater) |
| Yvonne Rogers | [UCL profile](https://profiles.ucl.ac.uk/33314-yvonne-rogers) |
| Geraldine Fitzpatrick | [TU Wien profile](https://informatics.tuwien.ac.at/people/geraldine-fitzpatrick) |
| Marc Hassenzahl | [University of Siegen HCI profile](https://hci-siegen.de/faculty-profile/) |

^important-people-evaluating-design-end
