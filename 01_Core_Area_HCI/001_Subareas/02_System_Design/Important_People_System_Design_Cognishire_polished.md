---
title: Important People
area: System Design
category: Professor Roadmap
cssclasses:
  - interface-forge
tags:
  - HCI
  - CS2023
  - HCI-Design
  - system-design
  - interface-design
  - interaction-design
  - prototyping
  - design-patterns
  - interaction-techniques
  - immersive-systems
  - fabrication
  - professors
  - university-roadmap
status: polished-rpg-readable-draft
---

# Important People

Back to [[01_Core_Area_HCI/001_Subareas/02_System_Design/Overview|The Interface Forge]].

> [!abstract] Forge Masters Roadmap
> This page maps active researchers, professors, and labs connected to **CS2023 HCI-Design: System Design**. In the Cognishire metaphor, these people are **forge masters** because their work shows how interface ideas become tools, prototypes, interaction techniques, design systems, tangible objects, AR/VR systems, and human-centred interactive systems.

**Fantasy name:** Forge Masters Roadmap  
**CS2023 name:** HCI-Design: System Design  
**Real meaning:** a practical guide to current academic routes in interface construction.

This is not a hall of fame. It is a route map. Each person represents a path through the Interface Forge: prototyping, design tools, interaction techniques, tangible interfaces, fabrication, AR/VR, spatial interaction, or broad interaction design.

> [!warning] Contact rule
> Use public academic contact routes respectfully. Do not mass email professors. Choose one or two people whose work matches your project, read their lab page first, and ask one specific question.

## Quick route compass

```mermaid
flowchart TB
    A((Interface Forge<br/>People Map))

    A --> B[Prototype Gate]
    A --> C[Input Forge]
    A --> D[Tangible Yard]
    A --> E[Spatial Tower]
    A --> F[Human-Centred Bridge]

    B --> B1[Landay<br/>Klemmer<br/>Mackay]
    C --> C1[Grossman<br/>Wigdor<br/>Vogel<br/>Beaudouin-Lafon]
    D --> D1[Ishii<br/>Baudisch]
    E --> E1[Feiner<br/>Billinghurst]
    F --> F1[Rogers<br/>Landay]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef route fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F route;
    class B1,C1,D1,E1,F1 detail;
```

| RPG route | Real HCI route | Best starting names |
|---|---|---|
| Prototype Gate | Prototyping, design tools, human-centred design | James Landay, Scott Klemmer, Wendy Mackay |
| Input Forge | Interaction techniques, input, UI systems | Tovi Grossman, Daniel Wigdor, Daniel Vogel, Michel Beaudouin-Lafon |
| Tangible Yard | Tangible interfaces, fabrication, haptics | Hiroshi Ishii, Patrick Baudisch |
| Spatial Tower | AR, VR, MR, spatial interfaces | Steven Feiner, Mark Billinghurst |
| Human-Centred Bridge | Broad interaction design and ubicomp | Yvonne Rogers, James Landay |

## How to use this page

Do not begin by memorising names. Begin with what you want to build.

```mermaid
flowchart LR
    A[Choose build interest] --> B[Pick route]
    B --> C[Read lab page]
    C --> D[Read two papers]
    D --> E[Build small prototype]
    E --> F[Ask focused question]

    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B,C,D,E node;
    class F final;
```

A weak question is: “I like HCI. Can I work with you?”

A stronger question is: “I am studying CS2023 HCI-Design, especially interaction techniques. I read your lab page on input systems, and I am building a small prototype for touch/gesture navigation. Which paper or course path should I read next?”

## Route I: Prototype Gate

This route is for students who want to turn user needs into sketches, wireframes, design tools, prototypes, and tested interface flows.

### James Landay

| Forge card | Details |
|---|---|
| Institution | Stanford University |
| Public role shown by official pages | Professor of Computer Science at Stanford; Stanford HAI co-founder and Co-Director |
| Route | Human-centred design, interface prototyping, design tools, mobile/ubiquitous computing, human-centred AI |
| Why follow this route | Useful if you want to connect prototyping with real interface systems and human-centred AI products |
| First student action | Build a small prototype, test it with a user, and explain what design principle it uses |
| Contact caution | Use the Stanford profile or directory route. Verify the current email before writing. |
| Official sources | [Stanford profile](https://profiles.stanford.edu/james-landay), [Stanford HAI profile](https://hai.stanford.edu/people/james-landay), [Stanford Engineering profile](https://engineering.stanford.edu/people/james-landay) |

### Scott Klemmer

| Forge card | Details |
|---|---|
| Institution | University of California San Diego |
| Public role shown by official pages | Professor of Cognitive Science and Computer Science & Engineering |
| Route | Design tools, prototyping, interaction design education, creativity support, social learning |
| Why follow this route | Useful if you want to understand how people design, learn, program, and create with interactive tools |
| First student action | Make a small tool or interface that helps someone create, learn, or organise work |
| Contact caution | Connect your message to a project or course route, not only general UX interest. |
| Official sources | [UCSD faculty profile](https://cogsci.ucsd.edu/people/faculty/scott-klemmer.html), [personal/lab page](https://d.ucsd.edu/srk/about/) |

### Wendy Mackay

| Forge card | Details |
|---|---|
| Institution | Inria and Université Paris-Saclay, Ex Situ HCI group |
| Public role shown by official pages | Inria Research Director; Professor Attaché at Université Paris-Saclay |
| Route | Participatory design, co-design, prototyping, mixed reality, human-computer partnerships |
| Why follow this route | Useful if you want users to help shape the design direction, not just test a finished interface |
| First student action | Run a small co-design session and turn participant feedback into a prototype revision |
| Contact caution | Read an Ex Situ project first and ask about participatory design or human-computer partnership work. |
| Official sources | [Inria profile](https://www.inria.fr/en/wendy-mackay), [personal/lab page](https://www.lri.fr/~mackay/), [Collège de France biography](https://www.college-de-france.fr/en/chair/wendy-mackay-computer-sciences-and-digital-technologies-annual-chair/biography) |

## Route II: Input Forge

This route is for students who want to design new ways of acting inside systems: touch, gesture, pen, keyboard, haptics, large displays, interface tools, and UI software.

### Tovi Grossman

| Forge card | Details |
|---|---|
| Institution | University of Toronto |
| Public role shown by official pages | Associate Professor in Computer Science |
| Route | Input, interaction techniques, design tools, learnability, creative interfaces |
| Why follow this route | Useful if you want to design tools and interaction techniques that help users act more effectively |
| First student action | Build a small interaction technique demo and define how you would test speed, errors, and learnability |
| Contact caution | Mention a concrete interest such as input, design tools, interaction techniques, or learning interfaces. |
| Official sources | [University of Toronto research profile](https://discover.research.utoronto.ca/4643-tovi-grossman), [personal page](https://www.tovigrossman.com/) |

### Daniel Wigdor

| Forge card | Details |
|---|---|
| Institution | University of Toronto |
| Public role shown by official pages | Professor and Associate Chair, Partnerships and Innovation, Department of Computer Science |
| Route | Natural user interfaces, touch, gesture, sensing, haptics, software systems |
| Why follow this route | Useful if you want to study new input methods, devices, and interaction architectures |
| First student action | Prototype a touch, gesture, or haptic interaction and write down what user action it supports |
| Contact caution | Avoid a generic UX message. Link your question to touch, gesture, natural interaction, sensing, or haptics. |
| Official sources | [University of Toronto research profile](https://discover.research.utoronto.ca/22832-daniel-wigdor), [personal page](https://danielwigdor.com/) |

### Daniel Vogel

| Forge card | Details |
|---|---|
| Institution | University of Waterloo |
| Public role shown by official pages | Professor, Cheriton School of Computer Science |
| Route | Input devices, interaction techniques, large displays, touch, tangibles, mid-air gestures, mixed reality |
| Why follow this route | Useful if you want to understand how physical input and new device forms become usable interfaces |
| First student action | Build or sketch a small input technique and define the user task it improves |
| Contact caution | Show how you would evaluate the interaction, not only how it looks. |
| Official sources | [Waterloo CS profile](https://cs.uwaterloo.ca/contacts/daniel-vogel), [Waterloo interaction research news](https://cs.uwaterloo.ca/news/daniel-vogel-colleagues-form-inria-associate-team-to-explore-input-for-real-time-interaction), [personal page](https://www.nonsequitoria.com/) |

### Michel Beaudouin-Lafon

| Forge card | Details |
|---|---|
| Institution | Université Paris-Saclay and LISN |
| Public role shown by official pages | Professor of Computer Science; HCI researcher in Ex Situ |
| Route | Fundamental interaction models, novel interaction techniques, engineering interactive systems, CSCW |
| Why follow this route | Useful if you want to understand interface design as an engineered interaction system, not just screen layout |
| First student action | Read about interaction models, then map one model to a small interface prototype |
| Contact caution | Ask a precise systems or theory question about interaction models, not a general design question. |
| Official sources | [personal page](https://www.lri.fr/~mbl/eintroduction.html), [ACM People profile](https://www.acm.org/articles/people-of-acm/2019/michel-beaudouin-lafon), [Université Paris-Saclay article](https://www.universite-paris-saclay.fr/en/news/michel-beaudouin-lafon-seeing-it-collaborative-tool) |

## Route III: Tangible Yard

This route is for students who want to move beyond flat screens into physical-digital interaction, fabrication, haptics, materials, and tangible systems.

### Hiroshi Ishii

| Forge card | Details |
|---|---|
| Institution | MIT Media Lab, Tangible Media Group |
| Public role shown by official pages | Jerome B. Wiesner Professor of Media Arts and Sciences; leader of Tangible Media Group |
| Route | Tangible user interfaces, Tangible Bits, Radical Atoms, shape-changing interfaces, physical-digital interaction |
| Why follow this route | Useful if you want digital information to become physical, graspable, spatial, or material |
| First student action | Build a simple physical-digital prototype, even if it is rough, and explain what action the object affords |
| Contact caution | A portfolio-style idea matters more than a generic message. |
| Official sources | [Tangible Media profile](https://tangible.media.mit.edu/person/hiroshi-ishii), [Tangible Media Group](https://tangible.media.mit.edu/) |

### Patrick Baudisch

| Forge card | Details |
|---|---|
| Institution | Hasso Plattner Institute |
| Public role shown by official pages | Professor; Head of Human Computer Interaction group |
| Route | Fabrication, haptics, physical interaction devices, 3D printing, laser cutting, physical VR |
| Why follow this route | Useful if you want to combine computer science, fabrication, hardware, and interface design |
| First student action | Build a small technical prototype or fabrication concept with a clear interaction goal |
| Contact caution | This route values working systems. Explain what you can build and how you would test it. |
| Official sources | [HPI HCI Lab](https://hpi.de/baudisch/home.html), [HPI research group](https://hpi.de/en/research/research-groups/human-computer-interaction/) |

## Route IV: Spatial Tower

This route is for students interested in AR, VR, MR, spatial interfaces, wearable computing, 3D UI, and immersive interaction.

### Steven K. Feiner

| Forge card | Details |
|---|---|
| Institution | Columbia University |
| Public role shown by official pages | Wang Family Professor of Computer Science; Director of the Computer Graphics and User Interfaces Lab |
| Route | AR/VR, 3D user interfaces, wearable computing, graphics, visualization, view management |
| Why follow this route | Useful if you want to design interfaces that live in space rather than on a flat page |
| First student action | Design a small spatial UI and define how users would know where to look, move, and recover |
| Contact caution | Ask about AR/VR interaction, visualization, or system design for a specific task. |
| Official sources | [Columbia Engineering profile](https://www.engineering.columbia.edu/faculty-staff/directory/steven-k-feiner), [Columbia personal page](https://www.cs.columbia.edu/~feiner/) |

### Mark Billinghurst

| Forge card | Details |
|---|---|
| Institution | University of South Australia and Adelaide research profile context |
| Public role shown by official pages | Professor of Human Computer Interaction; Director of the Australian Research Centre for Interactive and Virtual Environments according to public profiles |
| Route | Augmented reality, virtual reality, mixed reality, wearable computing, mobile interfaces, empathic computing |
| Why follow this route | Useful if you want to merge virtual and real worlds through AR/MR systems |
| First student action | Build or sketch a collaborative AR/MR prototype and write an evaluation question |
| Contact caution | Show awareness of user studies and spatial context, not only technical novelty. |
| Official sources | [Adelaide researcher profile](https://researchers.adelaide.edu.au/profile/mark.billinghurst), [Adelaide profile page](https://adelaide.edu.au/people/mark.billinghurst), [Empathic Computing Lab](https://empathiccomputing.org/team/mark-billinghurst/) |

## Route V: Human-Centred Bridge

This route connects system design to broad interaction design, everyday technology, ubiquitous computing, human-data interaction, and human-centred AI.

### Yvonne Rogers

| Forge card | Details |
|---|---|
| Institution | University College London, UCL Interaction Centre |
| Public role shown by official pages | Professor of Interaction Design at UCL; public profiles list work in HCI and human-centred AI |
| Route | Interaction design, ubiquitous computing, human-data interaction, human-centred AI, everyday systems |
| Why follow this route | Useful if you want to design interactive systems that support learning, work, collaboration, and everyday activity |
| First student action | Read one UCLIC project and connect it to a small interaction design prototype |
| Contact caution | Check UCLIC programmes and write one focused question about interaction design or human-centred AI. |
| Official sources | [UCL profile](https://profiles.ucl.ac.uk/33314-yvonne-rogers), [UCL CS page](https://www0.cs.ucl.ac.uk/people/Y.Rogers.html), [Royal Society profile](https://royalsociety.org/people/yvonne-rogers-35840/) |

## Study route by build goal

| If you want to build... | Start with these route cards | First prototype |
|---|---|---|
| A better app interface | Landay, Klemmer, Rogers | Clickable flow with clear labels, feedback, and task-based navigation |
| A design or creativity tool | Klemmer, Grossman, Mackay | Small tool that helps users make, edit, or learn something |
| A new input technique | Grossman, Wigdor, Vogel, Beaudouin-Lafon | Touch, gesture, pen, keyboard, or large-display interaction demo |
| A physical interactive object | Ishii, Baudisch | Tangible object or haptic prototype |
| An AR/VR interface | Feiner, Billinghurst | Spatial UI prototype with an evaluation plan |
| A participatory design study | Mackay, Rogers | Co-design session that produces a prototype revision |
| An engineered interactive system | Beaudouin-Lafon, Baudisch | Working system with states, architecture, and evaluation criteria |

## Contact protocol

```mermaid
flowchart LR
    A[Match route] --> B[Read lab page]
    B --> C[Read two papers]
    C --> D[Build small evidence]
    D --> E[Write focused email]
    E --> F[Use official programme route]

    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B,C,D,E node;
    class F final;
```

| Email part | Keep it short |
|---|---|
| Subject | “Student interested in HCI system design and [specific route]” |
| Opening | Who you are and what you are studying |
| Fit | One sentence about the lab or paper you read |
| Evidence | One small prototype, reading path, or project idea |
| Ask | One specific question about papers, courses, or programme fit |
| Close | Thanks and a GitHub or portfolio link if relevant |

### Minimal template

> [!example] Focused contact message
> Dear Professor [Name],  
> I am studying **CS2023 HCI-Design: System Design**, especially [route]. I read your page on [specific lab/project], and I am building a small prototype about [project].  
>  
> Would you recommend one or two papers, courses, or lab resources as a starting path for this topic?  
>  
> Best regards,  
> [Name]

## What this page should not claim

| Avoid this claim | Safer wording |
|---|---|
| “These are the only important people in System Design.” | “These are useful routes into System Design.” |
| “Every person here is currently recruiting.” | “Check current supervision and programme pages before writing.” |
| “A famous professor is automatically the best fit.” | “Choose fit by topic, lab, and project match.” |
| “System Design means visual design only.” | “System Design includes prototypes, interaction techniques, tools, systems, accessibility, and platform constraints.” |
| “A generic email is enough.” | “Read first, build small evidence, then ask a focused question.” |

## Venue routes for these people

| Venue | Why it matters for this roadmap |
|---|---|
| [ACM UIST](https://uist.acm.org/2026/) | Interface software, input/output devices, interaction techniques, tangible/ubiquitous computing, AR/VR |
| [ACM DIS](https://dis.acm.org/2026/) | Design-led HCI, interactive systems, design processes, artifacts, research through design |
| [ACM EICS](https://eics.acm.org/) | Engineering usable and effective interactive computing systems |
| [ACM TEI](https://tei.acm.org/) | Tangible, embedded, and embodied interaction |
| [ACM CHI](https://dl.acm.org/conference/chi) | Broad HCI research, including design, evaluation, accessibility, interaction, and systems |
| [CS2023 Knowledge Areas](https://csed.acm.org/knowledge-areas/) | Official curriculum route that places HCI inside computer science |

## Roadmap synthesis

The Forge Masters Roadmap shows how **CS2023 HCI-Design: System Design** becomes a set of academic routes. For prototyping and design tools, begin with Landay, Klemmer, and Mackay. For interaction techniques and UI systems, begin with Grossman, Wigdor, Vogel, and Beaudouin-Lafon. For tangible interfaces and fabrication, begin with Ishii and Baudisch. For immersive systems, begin with Feiner and Billinghurst. For broad interaction design and ubiquitous human-centred systems, begin with Rogers.

This page connects to [[Theory]] because these researchers provide models and principles. It connects to [[Design]] because their work produces tools, artifacts, patterns, and prototypes. It connects to [[Experiment]] because system-design claims require evaluation. It connects to [[Connections]] because System Design crosses software engineering, design, graphics, fabrication, spatial computing, and human-centred systems.

## Academic anchors

| Anchor | Source |
|---|---|
| CS2023 HCI Knowledge Area | [CS2023 Knowledge Areas](https://csed.acm.org/knowledge-areas/) |
| CS2023 HCI-Design basis | [CS2023 HCI Version Gamma PDF](https://csed.acm.org/wp-content/uploads/2023/09/HCI-Version-Gamma.pdf) |
| HCI community | [ACM SIGCHI](https://sigchi.org/) |
| Interface software and technology | [ACM UIST](https://uist.acm.org/2026/) |
| Designing interactive systems | [ACM DIS](https://dis.acm.org/2026/) |
| Engineering interactive computing systems | [ACM EICS](https://eics.acm.org/) |
| Tangible and embodied interaction | [ACM TEI](https://tei.acm.org/) |
| General HCI research | [ACM CHI](https://dl.acm.org/conference/chi) |
| Human-centred design standard | [ISO 9241-210](https://www.iso.org/standard/77520.html) |
| James Landay | [Stanford profile](https://profiles.stanford.edu/james-landay) |
| Scott Klemmer | [UCSD faculty profile](https://cogsci.ucsd.edu/people/faculty/scott-klemmer.html) |
| Wendy Mackay | [Inria profile](https://www.inria.fr/en/wendy-mackay) |
| Tovi Grossman | [University of Toronto profile](https://discover.research.utoronto.ca/4643-tovi-grossman) |
| Daniel Wigdor | [University of Toronto profile](https://discover.research.utoronto.ca/22832-daniel-wigdor) |
| Daniel Vogel | [Waterloo CS profile](https://cs.uwaterloo.ca/contacts/daniel-vogel) |
| Michel Beaudouin-Lafon | [personal page](https://www.lri.fr/~mbl/eintroduction.html) |
| Hiroshi Ishii | [MIT Tangible Media profile](https://tangible.media.mit.edu/person/hiroshi-ishii) |
| Patrick Baudisch | [HPI HCI Lab](https://hpi.de/baudisch/home.html) |
| Steven K. Feiner | [Columbia Engineering profile](https://www.engineering.columbia.edu/faculty-staff/directory/steven-k-feiner) |
| Mark Billinghurst | [Adelaide researcher profile](https://researchers.adelaide.edu.au/profile/mark.billinghurst) |
| Yvonne Rogers | [UCL profile](https://profiles.ucl.ac.uk/33314-yvonne-rogers) |

^important-people-system-design-end
