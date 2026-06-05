![[problemo1.webp|1000]]
# Open Problems

Open problems are not empty spaces. They are questions that remain difficult because people, technology, institutions, and social norms change together. In HCI, a problem often stays open when a design affects users in ways that are hard to measure, explain, or repair.

> [!quote] Frontier rule
> An open problem in HCI appears when a system changes what users can understand, trust, access, control, or contest faster than existing design knowledge can explain.

## Frontier compass

The main frontiers in this section are cognitive overload, mental model mismatch, calibrated trust, dynamic accessibility, evidence quality, user representation, and local-global fit.

```mermaid
flowchart TB
    A((Frontier Map))

    A --> B[Cognitive<br/>overload]
    A --> C[Mental model<br/>mismatch]
    A --> D[Human-AI<br/>trust]
    A --> E[Dynamic<br/>accessibility]
    A --> F[Evidence<br/>quality]
    A --> G[Local-global<br/>fit]

    B --> B1[Attention<br/>pressure]
    C --> C1[Hidden system<br/>logic]
    D --> D1[Uncertain<br/>output]
    E --> E1[Changing<br/>barriers]
    F --> F1[Incomplete<br/>metrics]
    G --> G1[Context<br/>mismatch]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F,G node;
    class B1,C1,D1,E1,F1,G1 detail;
```

- **Cognitive overload:** why it remains difficult: Interfaces place many choices, alerts, and interpretations inside limited attention.; connected section: [[Activities/Theory]]
- **Mental model mismatch:** why it remains difficult: Systems hide complex behaviour behind simple interface surfaces.; connected section: [[Activities/Design]]
- **Human-AI trust:** why it remains difficult: Users may overtrust fluent output or reject useful automation.; connected section: [[01_Core_Area_HCI/001_Subareas/05_Human_AI_Interaction/Open Problems]]
- **Dynamic accessibility:** why it remains difficult: Personalised, animated, and AI-generated interfaces can create changing barriers.; connected section: [[Local and Global]]
- **Evidence quality:** why it remains difficult: Task success and time do not fully show understanding, dignity, or effort.; connected section: [[Activities/Experiment]]
- **User representation:** why it remains difficult: Personas, analytics, and AI profiles can flatten diverse users into averages.; connected section: [[Connections]]
- **Local-global fit:** why it remains difficult: Global systems may ignore language, infrastructure, law, culture, and social risk.; connected section: [[Local and Global]]

## Frontier one: cognitive overload and attention scarcity

Modern interfaces often promise convenience while increasing hidden cognitive work. Users must compare options, manage notifications, interpret dashboards, understand privacy choices, evaluate automated suggestions, and recover from errors across devices.

The problem is larger than busy screens. The deeper issue is responsibility. A system may transfer too much judgement to the user while giving too little structure for making that judgement well.

```mermaid
flowchart TB
    A((Attention Scarcity))

    A --> B[More alerts]
    A --> C[More choices]
    A --> D[More data]
    A --> E[More recovery<br/>work]

    B --> B1[Interruption]
    C --> C1[Decision<br/>fatigue]
    D --> D1[Interpretation<br/>burden]
    E --> E1[Error stress]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

This frontier links to [[Activities/Design]]. Good design does not only remove visible clutter. It reduces unnecessary memory burden, interruption, uncertainty, and interpretation work. It also links to [[Activities/Experiment]], because a design that looks simpler is not always easier to understand.

| Overload source | HCI risk | Research question |
|---|---|---|
| Notification density | Users lose task focus. | Which notification patterns preserve attention without hiding urgency? |
| Privacy decisions | Users consent without understanding. | How can privacy choices be understandable without becoming exhausting? |
| Dashboard complexity | Users see data but cannot judge meaning. | What visual structures support correct interpretation? |
| Multi-step forms | Users forget progress and dependencies. | Which progress cues reduce memory burden? |
| AI suggestions | Users must evaluate uncertain output. | Which uncertainty cues improve judgement? |

The open problem is not whether cognitive load exists. The open problem is how to design systems that respect attention when digital environments constantly compete for it.

## Frontier two: mental models of invisible systems

Many systems hide complex technical behaviour behind simple surfaces. Search engines rank information. Recommenders personalise feeds. AI assistants generate answers. Platforms moderate content. Smart devices sense environments. Users often see the result, not the system logic that produced it.

```mermaid
flowchart LR
    A[Hidden system<br/>logic] --> B[Interface<br/>surface]
    B --> C[User sees<br/>output]
    C --> D[User builds<br/>mental model]
    D --> E[User acts on<br/>partial understanding]

    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A,B,C,D node;
    class E final;
```

The design challenge is not to expose every technical detail. That would create overload. The challenge is to show the right amount of system logic for the task, the risk, and the user’s decision.

A user booking a train ticket may need clear availability, price, time, and cancellation rules. A user receiving an automated medical, financial, academic, or legal recommendation needs stronger explanation, uncertainty, and control.

- **Search:** hidden behaviour: Ranking and filtering; mental model risk: User mistakes rank for truth.
- **Recommendation:** hidden behaviour: Personalisation criteria; mental model risk: User cannot tell why content appears.
- **AI assistant:** hidden behaviour: Probabilistic generation; mental model risk: User mistakes fluency for certainty.
- **Smart device:** hidden behaviour: Sensing and inference; mental model risk: User does not know what is being captured.
- **Platform moderation:** hidden behaviour: Rule enforcement; mental model risk: User cannot predict or contest outcomes.

This frontier connects to human-AI design guidance from Microsoft and Google PAIR, because AI systems often require users to judge output that is uncertain or incomplete. It also connects to broader HCI research communities such as ACM SIGCHI and ACM CHI.

## Frontier three: calibrated trust in human-AI interaction

AI systems create a special frontier because their outputs can be useful, fluent, uncertain, wrong, persuasive, personalised, and difficult to inspect. Users may overtrust them, undertrust them, or use them without understanding their limits.

The open question is not whether users should trust AI. A stronger HCI question is how systems can support calibrated trust. Users need help deciding when to rely, when to question, when to verify, when to override, and how to recover.

```mermaid
flowchart TB
    A((AI Output))

    A --> B[User judgement]
    B --> C[Overtrust]
    B --> D[Undertrust]
    B --> E[Calibrated trust]

    C --> F[Risk]
    D --> G[Disuse]
    E --> H[Appropriate use]

    F --> I[Redesign need]
    G --> I
    H --> J[Supported action]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;
    classDef final fill:#d9efd7,stroke:#7cab72,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class F,G,I detail;
    class H,J final;
```

- **Overtrust:** User accepts output without enough evidence. (response: Show uncertainty, sources, and verification steps.)
- **Undertrust:** User rejects useful automation. (response: Explain capability, reliability, and boundaries.)
- **Misplaced trust:** User trusts the system in the wrong context. (response: Match confidence cues to risk level.)
- **Automation dependence:** User stops checking the system. (response: Preserve meaningful human review.)
- **Contestability failure:** User cannot challenge a system decision. (response: Provide appeal, correction, and escalation paths.)

This frontier links to [[01_Core_Area_HCI/001_Subareas/05_Human_AI_Interaction/Open Problems]] because it combines cognition, design, data, power, explanation, accountability, and social consequence.

## Frontier four: accessibility in dynamic systems

Accessibility remains open because interfaces are no longer static pages. They are dynamic, personalised, animated, voice-enabled, AI-assisted, collaborative, embedded, and constantly updated.

WCAG gives essential criteria for accessible web content. WAI-ARIA helps with dynamic content and advanced interface controls. These standards matter, but teams still need user testing, assistive technology testing, and maintenance as the system changes.

```mermaid
flowchart TB
    A((Dynamic Accessibility))

    A --> B[Changing<br/>content]
    A --> C[Personalised<br/>interface]
    A --> D[AI-generated<br/>output]
    A --> E[Rich<br/>interaction]

    B --> B1[Structure<br/>may break]
    C --> C1[User path<br/>may vary]
    D --> D1[Text quality<br/>may shift]
    E --> E1[Keyboard and<br/>focus risk]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

> [!important] Frontier rule
> Accessibility is not solved when a system passes a checklist once. It must be maintained as content changes, components evolve, and user contexts shift.

- **Live updates:** accessibility risk: Screen reader users may miss changes.; evaluation need: Test announcements and focus behaviour.
- **Personalisation:** accessibility risk: Users may receive different interface paths.; evaluation need: Test multiple user states and profiles.
- **Animation:** accessibility risk: Motion may distract or harm users.; evaluation need: Provide reduced-motion options.
- **AI-generated content:** accessibility risk: Text may be unclear, biased, or unstructured.; evaluation need: Test readability, structure, and alternatives.
- **Custom controls:** accessibility risk: Native semantics may be lost.; evaluation need: Test keyboard and assistive technology support.

The strongest anchors for this frontier are the W3C Web Accessibility Initiative, WCAG 2.2, WAI-ARIA, the ARIA Authoring Practices Guide, and WebAIM.

## Frontier five: evidence beyond easy metrics

Another open problem is evidence itself. HCI often measures what is easy to count: time, clicks, task success, and error rate. These measures matter, but they do not fully capture understanding, dignity, anxiety, confidence, fatigue, exclusion, learning, or long-term adaptation.

A user may complete a task while feeling uncertain and unsupported. Another user may fail because the system assumes abilities, language, infrastructure, or prior knowledge they were never given. A third user may succeed in the short term but become dependent, distracted, or mistrustful over time.

```mermaid
flowchart TB
    A((Evidence Quality))

    A --> B[Easy to count]
    A --> C[Hard to interpret]
    A --> D[Often missed]
    A --> E[Long-term effects]

    B --> B1[Time<br/>clicks<br/>errors]
    C --> C1[Confidence<br/>stress<br/>effort]
    D --> D1[Dignity<br/>exclusion<br/>access]
    E --> E1[Learning<br/>dependency<br/>trust]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

- **Completion time:** Shows efficiency. (difficulty: Can hide confusion and stress.)
- **Error rate:** Shows breakdowns. (difficulty: May not explain cause.)
- **Confidence:** Shows perceived understanding. (difficulty: Hard to compare across users.)
- **Dignity:** Shows whether the experience respects the user. (difficulty: Often missing from metrics.)
- **Accessibility:** Shows inclusion or exclusion. (difficulty: Requires diverse testing and tools.)
- **Long-term adaptation:** Shows habits and dependency. (difficulty: Requires time and repeated observation.)

## Frontier six: representing users without flattening them

HCI often uses personas, analytics, user groups, behavioural clusters, and demographic categories. These tools can help designers reason about users. They can also flatten people into stereotypes or averages.

A persona can become a cartoon if it is not grounded in research. Analytics can hide minority experiences if the average looks acceptable. A user model can become harmful if it treats culture, disability, gender, age, language, or technical expertise as fixed assumptions instead of situated realities.

```mermaid
flowchart TB
    A((User Representation))

    A --> B[Persona]
    A --> C[Analytics]
    A --> D[User group]
    A --> E[Model profile]

    B --> B1[Stereotype<br/>risk]
    C --> C1[Average hides<br/>edge cases]
    D --> D1[Group labels<br/>simplify]
    E --> E1[Prediction may<br/>misclassify]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E node;
    class B1,C1,D1,E1 detail;
```

- **Persona:** useful when: Grounded in real research.; dangerous when: Invented from assumptions.
- **Analytics:** useful when: Combined with qualitative evidence.; dangerous when: Treated as complete truth.
- **User segment:** useful when: Used to detect different needs.; dangerous when: Used to stereotype behaviour.
- **AI profile:** useful when: Transparent and correctable.; dangerous when: Hidden, inaccurate, or hard to challenge.

The open problem is how to represent users without reducing them to convenient myths. This frontier connects strongly to [[Connections]], [[Local and Global]], and [[Important People]] because representation has intellectual, social, and ethical history.

## Frontier seven: local-global fit

Many systems are built globally but used locally. A design may work in one language, institution, legal setting, device ecosystem, or cultural context and fail in another. Local-global fit is therefore more than translation. It includes infrastructure, norms, trust in institutions, disability support, education systems, payment systems, privacy expectations, and risk perception.

```mermaid
flowchart TB
    A((Local-Global Fit))

    A --> B[Language]
    A --> C[Infrastructure]
    A --> D[Institutions]
    A --> E[Privacy norms]
    A --> F[Device context]

    B --> B1[Meaning changes]
    C --> C1[Access may fail]
    D --> D1[Rules differ]
    E --> E1[Consent expectations<br/>differ]
    F --> F1[Performance limits]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;
    classDef detail fill:#f6d6ee,stroke:#c27aa2,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
    class B1,C1,D1,E1,F1 detail;
```

- **Everyone has stable internet:** local complication: Rural or low-resource contexts may not.; hci response: Design offline, low-bandwidth, or resilient flows.
- **English labels are enough:** local complication: Meaning changes across languages.; hci response: Test terminology locally.
- **One privacy model fits all:** local complication: Laws and norms differ.; hci response: Adapt consent and data explanations.
- **Users trust institutions similarly:** local complication: Trust varies by history and context.; hci response: Study local trust conditions.
- **Devices are modern and powerful:** local complication: Hardware differs widely.; hci response: Design for performance and compatibility.

This frontier is one reason [[Local and Global]] must exist as a separate route. HCI cannot study the user outside place.

## Frontier map: unresolved tensions

Some open problems remain difficult because they involve real tensions. Improving one side can damage another.

```mermaid
flowchart TB
    A((Unresolved Tensions))

    A --> B[Personalisation<br/>vs privacy]
    A --> C[Automation<br/>vs control]
    A --> D[Efficiency<br/>vs understanding]
    A --> E[Engagement<br/>vs attention]
    A --> F[Global scale<br/>vs local fit]

    classDef center fill:#ddd2ff,stroke:#a875ff,color:#2b160b,stroke-width:3px;
    classDef node fill:#eee9ff,stroke:#a875ff,color:#2b160b,stroke-width:2px;

    class A center;
    class B,C,D,E,F node;
```

These tensions show why open problems cannot always be solved by a single design rule. They require judgement, evidence, ethics, and repeated evaluation.

## Academic anchors

| Frontier route | Trusted source |
|---|---|
| HCI research community | [ACM SIGCHI](https://sigchi.org/) |
| HCI academic venue | [ACM CHI Conference](https://dl.acm.org/conference/chi) |
| HCI research library | [ACM Digital Library](https://dl.acm.org/) |
| Human-centred design | [ISO 9241-210](https://www.iso.org/standard/77520.html) |
| Human-AI interaction | [Microsoft Human-AI Interaction Guidelines](https://www.microsoft.com/en-us/research/project/guidelines-for-human-ai-interaction/) |
| Human-AI design toolkit | [Microsoft HAX Toolkit](https://www.microsoft.com/en-us/haxtoolkit/) |
| AI design practice | [Google People + AI Guidebook](https://pair.withgoogle.com/guidebook/) |
| Fairness and accountability | [ACM FAccT](https://facctconference.org/) |
| Accessibility practice | [W3C Web Accessibility Initiative](https://www.w3.org/WAI/) |
| Accessibility standards | [WCAG 2.2](https://www.w3.org/TR/WCAG22/) |
| Dynamic web accessibility | [WAI-ARIA Overview](https://www.w3.org/WAI/standards-guidelines/aria/) |
| Accessible widget patterns | [ARIA Authoring Practices Guide](https://www.w3.org/WAI/ARIA/apg/) |
| Web accessibility reference | [WebAIM](https://webaim.org/) |
| Human factors and HCD | [NIST Human-Centered Design](https://www.nist.gov/itl/iad/human-centered-technologies/human-factors-human-centered-design) |
| Usability testing | [Nielsen Norman Group: Usability Testing 101](https://www.nngroup.com/articles/usability-testing-101/) |
| Computing ethics | [ACM Code of Ethics](https://www.acm.org/code-of-ethics) |

