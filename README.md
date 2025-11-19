# Hybrid INtelligence Thesaurus (HINT)

The **Hybrid INtelligence Thesaurus (HINT)** is a SKOS-based controlled vocabulary for describing **Hybrid Intelligence (HI)** systems, scenarios, and evaluations.  
It provides shared terms for use cases, domains, goals, contexts, roles, agents, capabilities, tasks, methods, task executions, interactions, phenomena, experiments, evaluations, and metrics.

HINT is designed to be used together with the [Hybrid Intelligence Ontology (HI)](https://w3id.org/hi-ontology#), and is aligned to it via `skos:exactMatch` relations and dedicated linking properties in the ontology (e.g. `hi:hasUseCaseConcept`, `hi:hasCapabilityConcept`, `hi:hasMetricConcept`, …).

---

## Features

HINT defines a single SKOS `ConceptScheme`:

- **Concept scheme**
  - `hint:HIScheme` – *Hybrid INtelligence Thesaurus (HINT)*

Within this scheme, concepts are organised in groups such as:

- **Core structural concepts**
  - `hint:UseCase`, `hint:Domain`, `hint:Goal`, `hint:Context`, `hint:Constraint`
  - `hint:Agent`, `hint:Role`, `hint:Capability`, `hint:Task`, `hint:TaskExecution`
  - `hint:Interaction`, `hint:Experiment`, `hint:Evaluation`, `hint:Metric`

- **Use case & domain taxonomies**
  - Use cases like *Personal Assistant*, *Collaborative Manipulation*, *Group Deliberation*, *Autonomous Tutoring*, *Medical Diagnosis*, *Energy Negotiation*, *Virtual Museum Guide*
  - Domains such as *Health and Lifestyle*, *Industrial and Service Robotics*, *Law and Policy*, *Education*, *Medical Diagnosis*, *Smart Campus*, *Digital Museum*

- **Goal and context concepts**
  - Goals such as *User Wellbeing*, *Safe Retrieval*, *Fair and Accurate Verdict*, *Effective Learning*, *Accurate and Trustworthy Diagnosis*, *Fair Efficient Heating*, *Enhanced Visitor Experience*
  - Contexts such as *Health Monitoring*, *Workspace Manipulation*, *Jury Deliberation*, *Online Learning*, *Clinical Consultation*, *Smart Campus*, *Virtual Exhibition*

- **Agents, roles, and capabilities**
  - `hint:Agent`, `hint:HumanAgent`, `hint:ArtificialAgent`
  - Roles such as *System Assistant*, *User*, *Risk Operator*, *Fine Manipulator*, *AI Advisor*, *Juror*, *Tutor*, *Learner*, *Clinician*, *Builder*, *Grid Operator*, *Virtual Guide*, *Visitor*
  - A structured hierarchy of capabilities:
    - Cognitive & reasoning capabilities
    - Learning & adaptation capabilities
    - Communication & explanation capabilities
    - Perception & sensing capabilities
    - Physical & manipulation capabilities
    - Domain-specific expert capabilities

- **Tasks, methods, and task executions**
  - Tasks such as *Data Collection*, *Conflict Resolution*, *Explanation*, *Unlock Cabinet*, *Fine Insertion*, *Policy Learning*, *Knowledge Graph Query*, *Question Answering*, etc.
  - Methods such as *Argumentation Reasoning*, *Reinforcement Learning*, *Knowledge Graph Querying*, *Post-hoc Explanation*, *Bayesian Logic*, *Meta-analysis Scoring*, *Semantic Linking*, *Semantic Embedding*, *Cooperative Learning*, *Protocol Negotiation*, *Virtual Reality Input Parsing*, *Data Collection*
  - Task execution concepts mirroring task types (e.g. *Data Collection Task Execution*, *Conflict Resolution Task Execution*, *Bayesian Modeling Task Execution*, …)

- **Interaction, phenomena, feedback, and ethics**
  - Interaction intents (e.g. *Explanation*, *Deliberation*, *Negotiation*, *Guidance*, *Answering*)
  - Interaction modalities (e.g. *Verbal Dialogue*, *Text Chat*, *Network Protocol*, *Dashboard*, *Virtual Reality*, *Voice Chat*)
  - Phenomena such as *Sensor Noise*, *Data Mismatch*, *Trust Shift*, *Risk Exposure*, *Skills Complementarity*, *Group Thinking*, *Knowledge Mismatch*, *Diagnosis Anchoring*, *Load Variability*, *Cooperative Learning Dynamics*, *Engagement Shift*
  - Bias (e.g. *Confirmation Bias*) and feedback concepts (e.g. *Trust Report Feedback*, *Explanation Message Feedback*, *Intervention Rationale Feedback*, *Recommendation Rationale Feedback*, *Allocation Rationale Feedback*)
  - Ethical constraints such as *Privacy*, *Autonomy*, *Transparency*, *Safety*, *Avoid Undue Influence*, *Fairness*, *Sustainability*, *User Comfort*, *Accessibility*

- **Experiments, evaluations, and metrics**
  - Experiments (e.g. *Transparency and Trust Experiment*, *Reinforcement Learning with Knowledge Graphs Experiment*, *Deliberation Support Experiment*, *Online Tutoring Experiment*, *Diagnosis Experiment*, *Campus Energy Allocation Experiment*, *Virtual Reality Effectiveness Experiment*, *Fine Manipulation Experiment*, *Safety Compliance Experiment*)
  - Evaluations (e.g. *Transparency Evaluation*, *AI Intervention Impact Evaluation*, *Tutor Impact Evaluation*, *Negotiation Impact Evaluation*, *Virtual Reality Impact Evaluation*, plus fine-grained ones for data collection, conflict resolution, manipulation, KG querying)
  - Metrics (e.g. *Trust Preservation*, *Task Success Rate*, *Safety Compliance*, *Explanation Clarity*, *Fair Outcome*, *Undue Influence*, *Recommendation Relevance*, *Learning Gain*, *Diagnosis Accuracy*, *Time*, *Energy Efficiency*, *User Comfort*, *CO₂ Reduction*, *Answer Accuracy*, *Engagement Time*)

---

## Namespaces

The thesaurus uses the following namespaces:

```text
Thesaurus namespace:  https://w3id.org/hi-thesaurus#
Preferred prefix:      hint

Ontology namespace:    https://w3id.org/hi-ontology#
Preferred prefix:      hi
```

---

## The Main Concept Scheme

The Hybrid INtelligence Thesaurus is defined as a single SKOS concept scheme:

```turtle
hint:HIScheme a skos:ConceptScheme ;
    dct:title "Hybrid INtelligence Thesaurus (HINT)"@en ;
    dct:description "A controlled thesaurus of terms to describe Hybrid Intelligence (HI)."@en ;
    skos:prefLabel "Hybrid INtelligence Thesaurus"@en ;
    vann:preferredNamespacePrefix "hint" ;
    vann:preferredNamespaceUri "https://w3id.org/hi-thesaurus#" .
```

---