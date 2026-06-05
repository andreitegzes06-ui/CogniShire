![[stretcyber.gif|1000]]
# Connections

> [!abstract] Oracle Connection Map
> This page maps the fields that support **Human-AI Interaction**. AI interaction is not only a model problem. It is also a user problem, an interface problem, a data problem, a software problem, an ethics problem, an accessibility problem, and an institutional problem.

The academic topic is **Human-AI Interaction**.  
The CS2023 grounding is a bridge between **Human-Computer Interaction**, **Artificial Intelligence**, **Software Engineering**, **Security**, **Accessibility**, and **Society, Ethics, and Professionalism**.

The practical meaning is simple: an AI system becomes meaningful only when a person must use it. A model produces an output. The interface frames that output. The user interprets it. Data and deployment shape it. Institutions decide where it is used. Someone must still be responsible for the consequences.

> [!quote] Connection rule
> Human-AI Interaction needs several fields because no single field can explain the whole loop from model output to human judgement.

## Fact-checked basis

|---|---|
| Human-AI Interaction is a bridge topic | CS2023 includes HCI, AI, software engineering, security, data, accessibility, and society/ethics areas. This page treats Human-AI Interaction as an interdisciplinary bridge, not as a single isolated CS2023 unit. |
| Human-AI design needs explicit interaction guidance | Microsoft Research published Guidelines for Human-AI Interaction and the HAX Toolkit as practical design resources for AI systems. |
| Human-centered AI design is an established design route | Google PAIR and Stanford HAI both present human-centered AI as a design and research direction. |
| AI risk management needs process and governance | NIST AI RMF organises AI risk work through Govern, Map, Measure, and Manage. |
| Human oversight is a formal concern in AI governance | The EU AI Act includes human oversight requirements for high-risk AI systems. |

## Main connection map

## CS2023 connection point

```mermaid
flowchart TB
    A((CS2023 Oracle Gate))

    A --> B[HCI]
    A --> C[AI]
    A --> D[Society and Ethics]
    A --> E[Data Management]
    A --> F[Software Engineering]
    A --> G[Security]
    A --> H[Accessibility]

    B --> B1[Design, users,<br/>evaluation]
    C --> C1[Models, prediction,<br/>generation]
    D --> D1[Responsibility,<br/>risk, social impact]
    E --> E1[Data quality,<br/>provenance]
    F --> F1[Implementation,<br/>logs, maintenance]
    G --> G1[Threats and<br/>misuse]
    H --> H1[Inclusive and<br/>assistive interaction]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G,H node;
    class B1,C1,D1,E1,F1,G1,H1 detail;
```

- **HCI:** Prompts, outputs, explanations, feedback, usability, trust, control
- **AI:** Training data, inference, prediction, generation, ranking, adaptation
- **Society and Ethics:** Fairness, privacy, transparency, accountability, professional responsibility
- **Data Management:** Provenance, missing data, bias, evidence quality, data lifecycle
- **Software Engineering:** Deployment, logging, monitoring, testing, versioning, rollback
- **Security:** Prompt injection, unsafe tool use, adversarial input, data leakage
- **Accessibility:** Assistive AI, accessible AI interfaces, inclusive outputs, disabled-user evidence

## Local UVT layer

> UVT has AI, ML, software systems, recommender, e-health, XAI-related, workflow, and Computer Science routes that can support Human-AI Interaction questions.

## Romanian layer

```mermaid
flowchart TB
    A((Romanian Oracle Layer))

    A --> B[RoCHI]
    A --> C[ABILITIES]
    A --> D[USV and MintViz]
    A --> E[Assistive AI]
    A --> F[Romanian Language]
    A --> G[Public and University Systems]

    B --> B1[National HCI route]
    C --> C1[Generative AI<br/>for digital accessibility]
    D --> D1[HCI, XR,<br/>accessible computing]
    E --> E1[Speech, wearables,<br/>adaptive support]
    F --> F1[Terminology and<br/>localisation]
    G --> G1[Institutional trust<br/>and accountability]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **RoCHI:** National HCI grounding and Romanian HCI proceedings route
- **A(I)BILITIES:** Romanian route for generative AI and digital accessibility
- **Radu-Daniel Vatavu / USV:** HCI, XR, ambient intelligence, accessible computing, and interaction research route
- **Ovidiu-Andrei Schipor:** Assistive technology, speech therapy systems, wearable or supportive interaction route
- **Romanian language:** AI explanations, translation quality, local terminology, and source comprehension
- **Public and university systems:** Institutional trust, accessibility, accountability, and AI use in public contexts

## HCI bridge

Human-AI Interaction remains a branch of HCI because the AI reaches people through an interface. The design must shape what users can ask, see, check, edit, reject, and learn.

```mermaid
flowchart TB
    A((HCI Bridge))

    A --> B[User Research]
    A --> C[Interface Design]
    A --> D[Interaction Design]
    A --> E[Evaluation]
    A --> F[Accessibility]
    A --> G[User Experience]

    B --> B1[Needs, goals,<br/>context]
    C --> C1[Output cards,<br/>source panels, controls]
    D --> D1[Prompts, feedback,<br/>correction]
    E --> E1[Trust, verification,<br/>task success]
    F --> F1[Who can access<br/>the AI system?]
    G --> G1[Confidence, effort,<br/>usefulness]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Affordance:** What does the AI invite the user to do?
- **Feedback:** Does the user know what the AI did and what changed?
- **Mental model:** What does the user believe the AI can do?
- **Error recovery:** Can the user correct, reject, undo, or report a wrong output?
- **Usability testing:** Can users complete tasks while trusting the system appropriately?
- **Accessibility:** Can different users access both the AI interface and AI-generated outputs?
- **User experience:** Does AI reduce effort, or does it create anxiety, dependence, or confusion?

## AI bridge

AI gives the system its behaviour. The interface must represent the type of AI involved because a recommender, a classifier, a generator, and an agent create different risks.

```mermaid
flowchart TB
    A((AI Bridge))

    A --> B[Machine Learning]
    A --> C[Generative AI]
    A --> D[Recommender Systems]
    A --> E[Classifiers]
    A --> F[Agents]
    A --> G[Explainable AI]

    B --> B1[Prediction from data]
    C --> C1[Text, image, code,<br/>audio generation]
    D --> D1[Ranking and<br/>personalisation]
    E --> E1[Labels and<br/>categories]
    F --> F1[Planning and<br/>action]
    G --> G1[Reasons, evidence,<br/>interpretability]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Machine learning predictor:** interaction problem: Users need to understand probability, limits, and uncertainty; interface requirement: Show confidence carefully, explain input factors, support review
- **Recommender system:** interaction problem: Users need to know why something was ranked; interface requirement: Show reason codes, alternatives, and control over preferences
- **Classifier:** interaction problem: Users need to understand label uncertainty; interface requirement: Show ambiguity, allow correction, explain label meaning
- **Agent:** interaction problem: Users need permission, preview, undo, and logs; interface requirement: Require confirmation before high-impact actions
- **Explainable AI:** interaction problem: Explanations must support decisions; interface requirement: Design explanations around user tasks, not technical display alone

## Cognitive science and psychology bridge

These fields explain why AI can mislead people even when the output sounds well written. Human-AI systems must be designed for actual human judgement, not ideal judgement.

```mermaid
flowchart TB
    A((Human Judgement Bridge))

    A --> B[Mental Models]
    A --> C[Attention]
    A --> D[Memory]
    A --> E[Reasoning]
    A --> F[Trust]
    A --> G[Automation Bias]

    B --> B1[What the user<br/>thinks AI does]
    C --> C1[What the user<br/>notices]
    D --> D1[What the user<br/>remembers]
    E --> E1[How the user<br/>judges evidence]
    F --> F1[How much the user<br/>relies on AI]
    G --> G1[User follows AI<br/>too easily]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Cognitive overload:** ai risk: Too many outputs confuse the user; design response: Group information and prioritise what needs review
- **Anchoring:** ai risk: The first AI answer dominates thinking; design response: Show alternatives and encourage comparison
- **Automation bias:** ai risk: User accepts AI too quickly; design response: Add verification prompts before high-impact use
- **Memory burden:** ai risk: User forgets assumptions or constraints; design response: Show prompt history, assumptions, and version notes
- **Weak metacognition:** ai risk: User thinks they understand because the AI explained it; design response: Ask the user to explain the idea in their own words

## Data science bridge

Human-AI systems are shaped by data. The user usually sees the answer, not the dataset, labels, assumptions, or gaps behind it.

```mermaid
flowchart TB
    A((Data Science Bridge))

    A --> B[Data Provenance]
    A --> C[Data Quality]
    A --> D[Bias]
    A --> E[Missingness]
    A --> F[Evaluation Metrics]
    A --> G[Drift]

    B --> B1[Where data<br/>came from]
    C --> C1[Noise, accuracy,<br/>coverage]
    D --> D1[Systematic<br/>unfairness]
    E --> E1[Who or what<br/>is absent]
    F --> F1[What performance<br/>actually measures]
    G --> G1[Behaviour changes<br/>over time]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Weak provenance:** The user cannot judge where knowledge came from
- **Biased data:** Output may misrepresent people, groups, or contexts
- **Missing local data:** UVT, Romania, Romanian language, and local institutions may disappear from the output
- **Weak labels:** Predictions or classifications become unreliable
- **Metric mismatch:** Accuracy may improve while usability, fairness, or accessibility worsens
- **Data drift:** Reliability changes after the system is deployed

## Software engineering bridge

AI systems need maintenance. Software engineering makes AI interaction traceable, testable, and repairable.

```mermaid
flowchart TB
    A((Software Engineering Bridge))

    A --> B[Versioning]
    A --> C[Logging]
    A --> D[Testing]
    A --> E[Monitoring]
    A --> F[Deployment]
    A --> G[Rollback]
    A --> H[Documentation]

    B --> B1[Model, prompt,<br/>file version]
    C --> C1[What happened<br/>and why]
    D --> D1[Human and<br/>technical tests]
    E --> E1[Failure and<br/>drift detection]
    F --> F1[Real-world<br/>release]
    G --> G1[Undo bad<br/>changes]
    H --> H1[How to use<br/>and maintain]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G,H node;
    class B1,C1,D1,E1,F1,G1,H1 detail;
```

## Ethics, law, and policy bridge

Human-AI Interaction becomes high-stakes when AI affects rights, opportunities, safety, privacy, access, or institutional judgement.

```mermaid
flowchart TB
    A((Ethics and Policy Bridge))

    A --> B[Fairness]
    A --> C[Privacy]
    A --> D[Transparency]
    A --> E[Human Oversight]
    A --> F[Accountability]
    A --> G[Safety]
    A --> H[Contestability]

    B --> B1[Who is<br/>disadvantaged?]
    C --> C1[What data<br/>is exposed?]
    D --> D1[Can users see<br/>AI involvement?]
    E --> E1[Can humans<br/>intervene?]
    F --> F1[Who is<br/>responsible?]
    G --> G1[What harm<br/>can occur?]
    H --> H1[Can users<br/>challenge output?]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G,H node;
    class B1,C1,D1,E1,F1,G1,H1 detail;
```

- **NIST AI RMF:** Identify, measure, manage, and govern AI risk as a process
- **EU AI Act:** Treat human oversight as a real design and governance requirement in high-risk contexts
- **FAccT and AIES:** Study fairness, accountability, ethics, and social impact
- **AI Incident Database:** Learn from real AI failures and near-failures
- **Responsible AI:** Make risk, limits, review, and responsibility visible
- **Contestability:** Give users a route to challenge or correct AI output

## Accessibility bridge

```mermaid
flowchart TB
    A((AI and Accessibility Bridge))

    A --> B[Assistive AI]
    A --> C[Accessible Interface]
    A --> D[Generated Accessibility]
    A --> E[Bias Against Disabled Users]
    A --> F[User Control]
    A --> G[Verification]

    B --> B1[Captions, summaries,<br/>alt text, communication]
    C --> C1[Keyboard, screen reader,<br/>contrast, structure]
    D --> D1[AI creates accessible<br/>or inaccessible content]
    E --> E1[Data and output can<br/>misrepresent disability]
    F --> F1[User edits, rejects,<br/>personalises]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **AI-generated alt text:** Useful only if accurate, editable, and checked against the image
- **AI summaries:** Helpful only if important meaning is preserved
- **Speech recognition:** Must handle accents, noise, speech differences, and language variation
- **Personalisation:** Must adapt without stereotyping the user
- **AI interface:** Must itself be keyboard-accessible, screen-reader friendly, readable, and understandable
- **Disabled-user involvement:** AI for access should be tested with people who have relevant access needs

## Education bridge

```mermaid
flowchart TB
    A((Education Bridge))

    A --> B[AI Tutor]
    A --> C[AI Writing Assistant]
    A --> D[Academic Integrity]
    A --> E[AI Literacy]
    A --> F[Assessment]
    A --> G[Metacognition]

    B --> B1[Explains and<br/>questions]
    C --> C1[Drafts and<br/>edits]
    D --> D1[Honest use and<br/>source checking]
    E --> E1[Capabilities and<br/>limits]
    F --> F1[Professor can<br/>inspect learning]
    G --> G1[Student knows what<br/>they understand]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Student copies AI output:** Add source verification and comprehension checks
- **AI hides weak understanding:** Ask the student to explain the idea in their own words
- **AI gives generic content:** Require UVT and Romanian grounding where relevant
- **AI replaces practice:** Use AI as tutor, critic, and editor, not as final author
- **Academic integrity risk:** Make AI-assisted work transparent where required by the course

## Security bridge

Natural language can become a control channel. This makes Human-AI Interaction partly a security problem.

```mermaid
flowchart TB
    A((Security Bridge))

    A --> B[Prompt Injection]
    A --> C[Data Leakage]
    A --> D[Tool Misuse]
    A --> E[Malicious Output]
    A --> F[Agentic Action]
    A --> G[Access Control]

    B --> B1[External text<br/>manipulates AI]
    C --> C1[Private data<br/>is exposed]
    D --> D1[AI calls tools<br/>unsafely]
    E --> E1[Harmful instructions<br/>or code]
    F --> F1[AI acts without<br/>enough control]
    G --> G1[Who can do<br/>what?]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Prompt injection:** Treat external text, webpages, documents, and tool outputs as untrusted until inspected
- **Data leakage:** Avoid giving unnecessary private context to AI systems
- **Tool misuse:** Require preview and confirmation before tool actions
- **Malicious output:** Check generated commands, code, and instructions before use
- **Agentic action:** Add permissions, logs, undo, and diffs
- **Access control:** Limit what AI can read, edit, delete, publish, or send

## Visualisation bridge

Visualisation helps users inspect AI behaviour. It should support judgement, not decoration.

```mermaid
flowchart TB
    A((Visualisation Bridge))

    A --> B[Source Map]
    A --> C[Uncertainty Display]
    A --> D[Alternative Outputs]
    A --> E[Decision Trace]
    A --> F[Risk Dashboard]
    A --> G[Version History]

    B --> B1[Where evidence<br/>comes from]
    C --> C1[Where doubt<br/>appears]
    D --> D1[Other possible<br/>answers]
    E --> E1[Why this output<br/>appeared]
    F --> F1[What needs<br/>review]
    G --> G1[What changed<br/>over time]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Source map:** use: Shows where evidence comes from; risk: Can imply support that sources do not really provide
- **Uncertainty display:** use: Shows where doubt, incompleteness, or risk appears; risk: False precision can mislead users
- **Alternative outputs:** use: Reduces anchoring on the first answer; risk: Too many alternatives can overload users
- **Decision trace:** use: Shows how input, model, and interface shaped output; risk: Trace may be incomplete or too technical
- **Version history:** use: Shows what changed after review; risk: Needs discipline to maintain

## Connection-to-design translation

- **HCI:** Prompt helper, output card, source panel, correction button, feedback path
- **AI:** Capability statement, model limitation note, uncertainty label, failure examples
- **Cognitive science:** Short outputs, explanation prompts, comparison views, assumption reminders
- **Psychology:** Trust calibration cues, verification reminders, anti-automation-bias friction
- **Software engineering:** Version history, prompt log, model/version note, rollback path
- **Ethics and law:** Risk category, human review requirement, accountability note, contestability route
- **Accessibility:** Keyboard support, screen reader structure, editable generated content, plain-language output
- **Education:** Comprehension check, reflection prompt, source-check task, AI-use disclosure
- **Visualisation:** Evidence map, uncertainty display, alternatives, decision trace

## Study route

## Academic anchors

| Route | Source |
|---|---|
| CS2023 HCI basis | [CS2023 HCI Version Gamma](https://csed.acm.org/wp-content/uploads/2023/09/HCI-Version-Gamma.pdf) |
| CS2023 Artificial Intelligence basis | [CS2023 AI SIGCSE 2022 version](https://csed.acm.org/knowledge-areas-intelligent-systems-ai-sigcse-2022-version/) |
| CS2023 Knowledge Areas | [CS2023 Knowledge Areas](https://csed.acm.org/knowledge-areas/) |
| Microsoft Human-AI guidelines | [Guidelines for Human-AI Interaction](https://www.microsoft.com/en-us/research/project/guidelines-for-human-ai-interaction/) |
| Microsoft HAX Toolkit | [HAX Toolkit AI Guidelines](https://www.microsoft.com/en-us/haxtoolkit/ai-guidelines/) |
| Google PAIR Guidebook | [People + AI Guidebook](https://pair.withgoogle.com/guidebook/) |
| Google PAIR | [People + AI Research](https://pair.withgoogle.com/) |
| Stanford HAI | [Stanford HAI](https://hai.stanford.edu/) |
| NIST AI RMF | [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) |
| NIST AI RMF Core | [Govern, Map, Measure, Manage](https://airc.nist.gov/airmf-resources/airmf/5-sec-core/) |
| EU AI Act | [European Commission AI Act](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) |
| EU AI Act human oversight | [EU AI Act Article 14](https://artificialintelligenceact.eu/article/14/) |
| AI Incident Database | [AI Incident Database](https://incidentdatabase.ai/) |
| ACM CHI | [ACM CHI](https://dl.acm.org/conference/chi) |
| ACM IUI | [ACM Intelligent User Interfaces](https://iui.acm.org/) |
| ACM FAccT | [ACM FAccT](https://facctconference.org/) |
| ACM ASSETS | [ASSETS Conference](https://www.sigaccess.org/assets/) |
| ACM TiiS | [ACM Transactions on Interactive Intelligent Systems](https://dl.acm.org/journal/tiis) |
| ACM CSCW | [ACM CSCW](https://cscw.acm.org/) |
| ACM AIES | [AAAI/ACM AIES](https://www.aies-conference.com/) |
| UVT Faculty of Informatics | [Faculty of Informatics UVT](https://info.uvt.ro/en/) |
| UVT Faculty departments | [Faculty of Informatics Departments](https://info.uvt.ro/en/departamente/) |
| UVT CSAI Department | [Department of Computational Sciences and Artificial Intelligence](https://info.uvt.ro/en/departamente/csai/) |
| UVT DTSE Department | [Department of Digital Technologies and Software Engineering](https://info.uvt.ro/en/departamente/dtse/) |
| UVT AI and ML research route | [Artificial Intelligence and Machine Learning](https://research.info.uvt.ro/artificial-intelligence-and-machine-learning/) |
| UVT research routes | [Research Center in Computer Science: Researchers](https://research.info.uvt.ro/researchers/) |
| RoCHI proceedings | [Romanian HCI proceedings](https://rochi.utcluj.ro/proceedings/en/) |
| A(I)BILITIES route | [A(I)BILITIES](https://aibilities.ro/en/about/) |
| ASSIST Software A(I)BILITIES | [A(I)BILITIES: Generative AI for Digital Accessibility](https://assist-software.net/project/aibilities) |
| MintViz A(I)BILITIES route | [MintViz A(I)BILITIES](https://mintviz.usv.ro/projects/A%28I%29BILITIES/index.php) |
| Radu-Daniel Vatavu | [Radu-Daniel Vatavu homepage](https://raduvatavu.usv.ro/) |
| Ovidiu-Andrei Schipor | [Ovidiu-Andrei Schipor projects](https://www.eed.usv.ro/~schipor/projects.php) |

^connections-human-ai-interaction-end
