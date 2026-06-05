![[cybertruck.gif|1000]]
# Theory

> [!abstract] Human-AI Interaction Theory
> **Human-AI Interaction** studies how people understand, use, question, verify, correct, and remain responsible when they work with systems that use artificial intelligence.

This page treats AI as a technical and social system. It does not treat AI as magic, personality, or authority. An AI system produces outputs through data, models, prompts, inference, deployment choices, and interface design. A human still has to interpret the output and decide what to do with it.

> [!quote] Oracle law
> An AI interface becomes risky when it turns uncertainty into authority. Good Human-AI Interaction makes capability, evidence, limits, control, and responsibility visible.

## Fact-checked basis

|---|---|
| Human-AI design needs explicit interaction guidance | Microsoft Research published **18 Guidelines for Human-AI Interaction**. The HAX Toolkit organises them around initial interaction, interaction over time, AI failure, and system change. |
| Human-centred AI is a recognised design route | Google PAIR gives practical guidance for designing human-centred AI products. Stanford HAI describes human-centred AI as AI that augments people, responds to societal needs, and draws inspiration from humans. |
| AI risk should be managed as a process | NIST AI RMF uses the functions **Govern, Map, Measure, Manage**. |
| The Romanian layer has real HCI and AI-accessibility routes | RoCHI gives a Romanian HCI route. A(I)BILITIES is a Romanian generative AI initiative for personalised interactive solutions for users with disabilities. |

## Core theory map

```mermaid
flowchart TB
    A((Human-AI<br/>Interaction Theory))

    A --> B[AI capability]
    A --> C[User mental model]
    A --> D[Uncertainty]
    A --> E[Trust calibration]
    A --> F[Explanation]
    A --> G[Human control]
    A --> H[Accountability]

    B --> B1[What the system<br/>can and cannot do]
    C --> C1[What the user thinks<br/>the system does]
    D --> D1[Where error or doubt<br/>can appear]
    E --> E1[Trust matches<br/>actual reliability]
    F --> F1[Reasons help<br/>judgement]
    G --> G1[Inspect, edit,<br/>reject, stop]
    H --> H1[Responsibility<br/>stays visible]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G,H node;
    class B1,C1,D1,E1,F1,G1,H1 detail;
```

## CS2023 grounding

Human-AI Interaction is best treated as a bridge topic. It sits between several CS2023 areas instead of belonging to only one unit.

```mermaid
flowchart TB
    A((CS2023 Bridge))

    A --> B[Human-Computer<br/>Interaction]
    A --> C[Artificial<br/>Intelligence]
    A --> D[Society, Ethics,<br/>Professionalism]
    A --> E[Software<br/>Engineering]
    A --> F[Data and<br/>Models]
    A --> G[Accessibility]

    B --> B1[Users, tasks,<br/>design, evaluation]
    C --> C1[Prediction, ranking,<br/>generation, classification]
    D --> D1[Fairness, privacy,<br/>responsibility]
    E --> E1[Deployment, logs,<br/>monitoring]
    F --> F1[Data quality,<br/>bias, uncertainty]
    G --> G1[Inclusive and<br/>assistive use]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

## Local UVT layer

## Romanian layer

```mermaid
flowchart TB
    A((Romanian Layer))

    A --> B[RoCHI]
    A --> C[ABILITIES]
    A --> D[USV and MintViz]
    A --> E[Assistive<br/>technology]
    A --> F[Romanian<br/>language]
    A --> G[Local institutions]

    B --> B1[National HCI route]
    C --> C1[Generative AI for<br/>digital accessibility]
    D --> D1[HCI, XR,<br/>accessible computing]
    E --> E1[Speech, wearables,<br/>adaptive support]
    F --> F1[Terminology and<br/>localisation]
    G --> G1[Public and<br/>university contexts]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **RoCHI:** National HCI context and Romanian HCI proceedings
- **A(I)BILITIES:** Romanian route for generative AI and personalised accessibility
- **Radu-Daniel Vatavu / USV:** HCI, XR, ambient intelligence, accessible computing
- **Ovidiu-Andrei Schipor:** HCI, assistive technologies, speech therapy systems
- **Romanian language:** AI explanation quality, terminology, translation, and comprehension
- **Romanian institutions:** Local trust, accountability, public systems, and educational use

## AI as a sociotechnical system

The user often sees only an answer, recommendation, label, summary, or generated object. The system behind that output has several layers.

```mermaid
flowchart TB
    A((AI System))

    A --> B[Data]
    B --> C[Model]
    C --> D[Input or prompt]
    D --> E[Inference]
    E --> F[Output]
    F --> G[Interface]
    G --> H[User interpretation]
    H --> I[Action]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G,H node;
    class I final;
```

- **Data:** What examples, omissions, labels, and biases shaped the system?
- **Model:** What pattern has the system learned or approximated?
- **Input or prompt:** What did the user ask, and what context was missing?
- **Inference:** How is an output produced from the input?
- **Output:** Is the answer correct, useful, unsupported, biased, or uncertain?
- **Interface:** How is the output framed, explained, and controlled?
- **User interpretation:** What does the user believe after seeing it?
- **Action:** What happens if the user trusts the output?

The interface matters because it frames the AI. It can make a guess look like evidence. It can also make doubt, limits, and verification visible.

## Probabilistic interaction

Many AI systems classify, rank, recommend, or generate. Their behaviour may change across prompts, data, settings, model versions, and deployment context.

- **A button usually has a fixed action:** A prompt can produce different outputs
- **Errors are often visible:** Errors can be fluent and hidden
- **The user learns stable rules:** The user must learn model limits
- **Testing can cover fixed paths:** Testing must cover uncertainty and misuse
- **Trust often comes from consistency:** Trust must be calibrated to evidence

This is why Human-AI Interaction needs theory. AI changes what the user must judge.

## Mental models

A mental model is the user’s internal explanation of how a system works. In AI systems, mental models are often incomplete or wrong.

```mermaid
flowchart TB
    A((Mental Model Problem))

    A --> B[What the user thinks]
    A --> C[What the AI does]
    B --> D[Mismatch]
    C --> D
    D --> E[Overtrust]
    D --> F[Undertrust]
    D --> G[Misuse]
    D --> H[Design repair]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef risk fill:#ffd6d6,stroke:#c96b6b,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D node;
    class E,F,G risk;
    class H final;
```

- **“The AI understands my full context.”:** risk: User expects personal accuracy (repair: Ask for missing context)
- **“The AI is neutral.”:** risk: User ignores bias (repair: Explain data and representation limits)
- **“The AI is a search engine.”:** risk: User confuses generation with retrieval (repair: Separate retrieval from generation)
- **“The AI is useless because it failed once.”:** risk: User misses useful support (repair: Show suitable tasks and unsuitable tasks)
- **“The AI is the author.”:** risk: Student stops owning the work (repair: Keep human authorship and review visible)

A good AI interface teaches the user what kind of system they are using.

## Trust calibration

Trust calibration means that user trust should match system reliability. The goal is not maximum trust. The goal is justified trust.

```mermaid
flowchart TB
    A((Trust Calibration))

    A --> B[Overtrust]
    A --> C[Appropriate trust]
    A --> D[Undertrust]

    B --> B1[User accepts<br/>wrong output]
    C --> C1[User uses and<br/>verifies]
    D --> D1[User ignores<br/>useful support]

    B --> E[Add limits and<br/>source checks]
    D --> F[Show evidence and<br/>good use cases]
    C --> G[Support informed<br/>collaboration]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef risk fill:#ffd6d6,stroke:#c96b6b,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D node;
    class B1,D1 risk;
    class C1,E,F,G final;
```

- **Undertrust:** example: The user rejects useful drafting support without checking; design response: Show evidence, scope, and examples of appropriate use
- **Appropriate trust:** example: The user uses AI for drafting but verifies facts; design response: Keep verification easy
- **Trust collapse:** example: One error makes the user reject the whole system; design response: Explain the failure and show the repair path
- **False confidence:** example: A polished answer hides weak evidence; design response: Separate answer, evidence, and uncertainty

## Automation bias and deskilling

Automation bias means that users rely too much on automated suggestions. Deskilling means users stop practising a skill because the system does too much for them.

```mermaid
flowchart TB
    A((Automation Risk))

    A --> B[AI suggestion]
    B --> C[User accepts<br/>too quickly]
    C --> D[Error enters work]
    C --> E[Skill practice<br/>decreases]
    D --> F[Misinformation<br/>or harm]
    E --> G[Deskilling]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef risk fill:#ffd6d6,stroke:#c96b6b,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C node;
    class D,E,F,G risk;
```

AI should support learning and judgement. It should not replace them.

## Explanation, transparency, interpretability, and contestability

These terms are related, but they are not the same.

```mermaid
flowchart TB
    A((Understanding AI Output))

    A --> B[Transparency]
    A --> C[Explainability]
    A --> D[Interpretability]
    A --> E[Contestability]
    A --> F[Traceability]

    B --> B1[User knows AI<br/>is involved]
    C --> C1[User receives a<br/>useful reason]
    D --> D1[Logic or model<br/>can be inspected]
    E --> E1[User can challenge<br/>or correct output]
    F --> F1[Output links to<br/>process and evidence]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

- **Transparency:** meaning: The user knows AI is involved; interface example: “This section was AI-assisted and human reviewed.”
- **Explainability:** meaning: The user gets a reason that helps judgement; interface example: “This source is used because it defines Human-AI guidelines.”
- **Interpretability:** meaning: A human can inspect part of the model or logic; interface example: Feature importance, examples, traces, or model card
- **Traceability:** meaning: The output can be linked to evidence or process; interface example: Prompt log, source list, model version, commit history
- **Limitation disclosure:** meaning: The system states where it may fail; interface example: “Current roles must be checked on official pages.”

A good explanation is not necessarily long. It is useful when it improves the user’s next decision.

## Human oversight

Human oversight must be designed. A human is not truly in control if they cannot understand, intervene, or override.

```mermaid
flowchart TB
    A((Human Oversight))

    A --> B[Notice]
    A --> C[Understand]
    A --> D[Intervene]
    A --> E[Override]
    A --> F[Log]
    A --> G[Repair]

    B --> B1[AI involvement<br/>is visible]
    C --> C1[Risk and evidence<br/>are clear]
    D --> D1[Human can<br/>change course]
    E --> E1[Human can<br/>stop or reverse]
    F --> F1[Decision is<br/>recorded]
    G --> G1[System or process<br/>improves]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Rubber-stamp review:** why it fails: Human approves without inspection; better design: Show evidence and risk near the output
- **No authority:** why it fails: Human sees a problem but cannot override; better design: Provide reject, edit, stop, undo, and rollback
- **No time:** why it fails: Human must review too much too quickly; better design: Prioritise risky outputs
- **No expertise:** why it fails: Human cannot judge model limits; better design: Provide explanation, examples, and training
- **No log:** why it fails: Failures disappear; better design: Record issue, version, and repair
- **No accountability:** why it fails: Responsibility is unclear; better design: Define who reviews and who decides

## Human-AI collaboration roles

AI can play different roles. The role must be clear because each role creates different expectations and risks.

```mermaid
flowchart TB
    A((AI Role))

    A --> B[Tool]
    A --> C[Tutor]
    A --> D[Assistant]
    A --> E[Advisor]
    A --> F[Agent]
    A --> G[Infrastructure]

    B --> B1[User directly<br/>controls it]
    C --> C1[AI supports<br/>learning]
    D --> D1[AI helps complete<br/>a task]
    E --> E1[AI recommends<br/>a judgement]
    F --> F1[AI acts across<br/>time or files]
    G --> G1[AI shapes the<br/>background system]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Tool:** user expectation: User controls directly; main risk: User may expect intelligence that is not there
- **Tutor:** user expectation: AI supports learning; main risk: Student may let AI do the thinking
- **Assistant:** user expectation: AI helps with work; main risk: User may delegate too much
- **Advisor:** user expectation: AI recommends decisions; main risk: User may accept advice without checking
- **Agent:** user expectation: AI acts across time or files; main risk: User may lose control
- **Infrastructure:** user expectation: AI ranks, filters, or monitors; main risk: User may not know AI shaped the experience

## Feedback and adaptation

Human-AI systems often form loops. The user gives input. The AI responds. The user reacts. The system or workflow may adapt.

```mermaid
flowchart TB
    A((Human-AI<br/>Feedback Loop))

    A --> B[User input]
    B --> C[AI output]
    C --> D[User judgement]
    D --> E[Correction or<br/>behaviour]
    E --> F[System or process<br/>adaptation]
    F --> C

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
```

- **User input:** Did the user provide enough context?
- **AI output:** Does the output show evidence and limits?
- **User judgement:** Does the user inspect before trusting?
- **Correction:** Can the user mark errors easily?
- **Adaptation:** Does the system change in a visible and controllable way?
- **Long-term use:** Does trust improve, drift, or become misplaced?

Adaptation is useful only when it remains understandable and controllable.

## Uncertainty design

```mermaid
flowchart TB
    A((Uncertainty))

    A --> B[Confidence]
    A --> C[Source quality]
    A --> D[Missing data]
    A --> E[Model limit]
    A --> F[Alternative answer]
    A --> G[Verification step]

    B --> B1[How sure is<br/>the system?]
    C --> C1[Where did evidence<br/>come from?]
    D --> D1[What is unknown?]
    E --> E1[Where is the<br/>model weak?]
    F --> F1[Could another<br/>answer fit?]
    G --> G1[What should the<br/>user check?]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Confidence score:** useful when: The user understands probability; risk: Can create false precision
- **Alternative output:** useful when: Several answers are plausible; risk: Too many alternatives can overload the user
- **Clarifying question:** useful when: The input is ambiguous; risk: Too many questions slow the task
- **Verification checklist:** useful when: Stakes are academic or factual; risk: Users may skip it if it feels optional

## Generative AI

Generative AI produces text, code, images, summaries, translations, plans, and explanations. It is useful for drafting. It is not a source of truth by itself.

```mermaid
flowchart TB
    A((Generative AI Workflow))

    A --> B[Prompt]
    B --> C[Generation]
    C --> D[Human review]
    D --> E[Source verification]
    E --> F[Revision]
    F --> G[Use or reject]

    C --> H[Hallucination risk]
    C --> I[Bias risk]
    C --> J[Source risk]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef risk fill:#ffd6d6,stroke:#c96b6b,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class G final;
    class H,I,J risk;
```

## Prompting as interaction design

A prompt is not just text. It is an interface between the user and the model. The prompt frames the task, context, constraints, output format, and quality criteria.

Good prompt design supports good human judgement. It cannot replace checking.

## Human-centred AI

Human-centred AI is a broad approach. It places human needs, human agency, social impact, and responsible deployment at the centre of the system.

```mermaid
flowchart TB
    A((Human-Centred AI))

    A --> B[Augmentation]
    A --> C[Control]
    A --> D[Trust]
    A --> E[Safety]
    A --> F[Fairness]
    A --> G[Accountability]

    B --> B1[AI supports<br/>human capability]
    C --> C1[Human can direct<br/>and override]
    D --> D1[Trust matches<br/>evidence]
    E --> E1[Risks are<br/>reduced]
    F --> F1[Harms and bias<br/>are addressed]
    G --> G1[Responsibility<br/>is visible]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Augmentation:** AI helps the student structure, compare, and revise
- **Control:** Student can edit, reject, and verify
- **Trust:** AI output is treated as draft until checked
- **Fairness:** Missing groups and local contexts are checked
- **Accountability:** Sources, prompts, edits, and limits remain visible

The goal is not to make AI seem human. The goal is to make AI useful, honest, controllable, and accountable.

## AI in learning

```mermaid
flowchart TB
    A((AI for Learning))

    A --> B[Explain]
    A --> C[Question]
    A --> D[Critique]
    A --> E[Compare]
    A --> F[Verify]
    A --> G[Reflect]

    B --> B1[Clarify the concept]
    C --> C1[Make the student think]
    D --> D1[Find weak points]
    E --> E1[Show alternatives]
    F --> F1[Check evidence]
    G --> G1[Student explains<br/>in own words]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **AI gives the final answer:** AI asks questions and explains
- **Student pastes output:** Student verifies and rewrites
- **AI replaces reasoning:** AI supports reasoning
- **Sources are accepted blindly:** Sources are checked
- **Page looks impressive:** Student can explain it
- **AI hides process:** Prompts, edits, and sources remain visible

## AI and accessibility

AI can support access, but it can also create new barriers.

```mermaid
flowchart TB
    A((AI and Accessibility))

    A --> B[Support]
    A --> C[Risk]

    B --> B1[Captions, alt text,<br/>summaries]
    B --> B2[Communication<br/>support]
    B --> B3[Personalised<br/>learning]

    C --> C1[Wrong descriptions]
    C --> C2[Bias against<br/>disabled users]
    C --> C3[Privacy concerns]
    C --> C4[Inaccessible AI<br/>interface]

    B --> D[Evaluation required]
    C --> D

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef risk fill:#ffd6d6,stroke:#c96b6b,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B node;
    class C risk;
    class B1,B2,B3 node;
    class C1,C2,C3,C4 risk;
    class D final;
```

- **Generate alt text:** It may describe the image incorrectly
- **Summarise long text:** It may remove important nuance
- **Caption speech:** It may fail with accents, noise, or speech differences
- **Adapt content:** It may reduce user control
- **Personalise learning:** It may stereotype the user
- **Generate accessible code:** It may produce inaccessible interfaces
- **Help disabled users:** It may exclude disabled users from design and testing

## Risk management and accountability

The NIST AI RMF gives a useful risk-management vocabulary: **Govern**, **Map**, **Measure**, and **Manage**. These functions can be translated into Human-AI Interaction.

```mermaid
flowchart TB
    A((AI Risk Process))

    A --> B[Govern]
    A --> C[Map]
    A --> D[Measure]
    A --> E[Manage]

    B --> B1[Define roles and<br/>responsibility]
    C --> C1[Identify context,<br/>users, risks]
    D --> D1[Evaluate reliability,<br/>bias, understanding]
    E --> E1[Reduce risk and<br/>monitor repair]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

- **Govern:** Define who owns the system, output, review process, and repair path
- **Map:** Identify users, tasks, intended use, misuse, and affected groups
- **Measure:** Test correctness, bias, usability, trust, explanation, and accessibility
- **Manage:** Reduce risk through design changes, controls, monitoring, and updates

## Theory checklist

- **What is the AI role?:** Tutor, critic, drafting assistant, advisor, agent, or infrastructure
- **What can the AI do?:** Specific capability, not vague intelligence
- **What can it not guarantee?:** Truth, completeness, current facts, neutrality, or source support
- **Can the user intervene?:** Edit, reject, verify, undo, stop, or report
- **Can the student explain it?:** Yes, without copying the AI text
- **Is responsibility visible?:** Sources, review status, prompt context, and limits are recorded

## Academic anchors

| Route | Source |
|---|---|
| CS2023 HCI basis | [CS2023 HCI Version Gamma](https://csed.acm.org/wp-content/uploads/2023/09/HCI-Version-Gamma.pdf) |
| CS2023 Artificial Intelligence basis | [CS2023 AI SIGCSE 2022 version](https://csed.acm.org/knowledge-areas-intelligent-systems-ai-sigcse-2022-version/) |
| CS2023 Knowledge Areas | [CS2023 Knowledge Areas](https://csed.acm.org/knowledge-areas/) |
| Microsoft Human-AI guidelines | [Guidelines for Human-AI Interaction](https://www.microsoft.com/en-us/haxtoolkit/ai-guidelines/) |
| Microsoft Human-AI guidelines article | [Eighteen best practices for human-centered AI design](https://www.microsoft.com/en-us/research/group/customer-insights-research/articles/guidelines-for-human-ai-interaction-eighteen-best-practices-for-human-centered-ai-design/) |
| Google People + AI Research | [People + AI Research](https://design.google/library/people-ai-research) |
| Google People + AI Guidebook | [PAIR Guidebook](https://pair.withgoogle.com/guidebook/) |
| Stanford HAI human-centered AI definition | [Brief Definitions of Key Terms in AI](https://hai.stanford.edu/policy/brief-definitions-of-key-terms-in-ai) |
| Stanford HAI institute route | [Stanford HAI](https://hai.stanford.edu/) |
| NIST AI RMF | [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) |
| NIST AI RMF Core | [Govern, Map, Measure, Manage](https://airc.nist.gov/airmf-resources/airmf/5-sec-core/) |
| EU AI Act | [European Commission AI Act](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) |
| EU AI Act Article 14 | [Human oversight](https://artificialintelligenceact.eu/article/14/) |
| ACM IUI | [ACM Conference on Intelligent User Interfaces](https://iui.acm.org/) |
| ACM CHI | [ACM CHI](https://dl.acm.org/conference/chi) |
| ACM HAI | [Human-Agent Interaction](https://hai-conference.net/) |
| ACM TiiS | [ACM Transactions on Interactive Intelligent Systems](https://dl.acm.org/journal/TIIS) |
| ACM FAccT | [ACM FAccT](https://facctconference.org/) |
| ACM ASSETS | [ASSETS Conference](https://www.sigaccess.org/assets/) |
| UVT Faculty of Informatics | [Faculty of Informatics UVT](https://info.uvt.ro/en/) |
| UVT Faculty departments | [Faculty of Informatics Departments](https://info.uvt.ro/en/departamente/) |
| UVT CSAI Department | [Department of Computational Sciences and Artificial Intelligence](https://info.uvt.ro/en/departamente/csai/) |
| UVT DTSE Department | [Department of Digital Technologies and Software Engineering](https://info.uvt.ro/en/departamente/dtse/) |
| UVT AI and ML research route | [Artificial Intelligence and Machine Learning](https://research.info.uvt.ro/artificial-intelligence-and-machine-learning/) |
| RoCHI proceedings | [Romanian HCI proceedings](https://rochi.utcluj.ro/proceedings/en/) |
| Romanian HCI community route | [Romanian Special Interest Group in HCI](https://cgis.utcluj.ro/rochi_group/) |
| Radu-Daniel Vatavu | [Radu-Daniel Vatavu homepage](https://raduvatavu.usv.ro/) |
| Ovidiu-Andrei Schipor | [Ovidiu-Andrei Schipor homepage](https://www.eed.usv.ro/~schipor/) |
| A(I)BILITIES route | [A(I)BILITIES](https://aibilities.ro/en/about/) |
| ASSIST Software A(I)BILITIES | [A(I)BILITIES — Generative AI for Digital Accessibility](https://assist-software.net/project/aibilities) |
| MintViz A(I)BILITIES route | [MintViz A(I)BILITIES](https://mintviz.usv.ro/projects/A%28I%29BILITIES/index.php) |

^theory-human-ai-interaction-end
