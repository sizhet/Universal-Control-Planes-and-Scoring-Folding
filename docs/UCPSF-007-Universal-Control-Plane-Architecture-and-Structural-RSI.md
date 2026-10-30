
# UCPSF-007 — Universal Control Plane Architecture and Structural RSI

**Subtitle:** Governing Hybrid Intelligence, Scoring Forests, Recursive Evaluator Evolution, and Structural Self-Improvement

**Authors:** Sizhe Tan & GPT-Obot  
**Project:** Universal Control Planes and Scoring Tree/Forest/Folding for Structural Intelligence (UCPSF)  
**Document ID:** UCPSF-007  
**Version:** 1.0.0  
**Date:** October 19, 2026  
**Status:** Proposed System Architecture and Research Framework  
**License:** Apache-2.0

---

## Abstract

Complex artificial intelligence systems increasingly combine heterogeneous models, tools, evaluators, context-localization mechanisms, and multi-stage computational workflows.

AI Relay and Structural Recursive Self-Improvement (RSI) extend this complexity by introducing repeated candidate generation, evaluation, selection, delegation, and structural modification.

These systems require more than powerful execution engines. They require explicit mechanisms for selecting computational structures, evaluating alternatives, managing resources, preserving evidence, enforcing policy, and governing structural evolution.

This paper proposes a **Universal Control Plane (UCP)** architecture for Structural Intelligence.

The proposed architecture integrates Generalized Scoring Intelligence, Scoring Trees and Forests, Unaligned AND Folding, recursive Common Concept Core (CCC) distillation, Perspective-Aware Optimization, Meta-Scoring Intelligence, and Hybrid Localization with Hybrid Per-Node Intelligence.

We distinguish the **Intelligence Execution Plane**, responsible for task computation, from the **Evaluation and Scoring Plane**, responsible for assessing candidates and evaluators, and the **Governance and Control Plane**, responsible for dispatch, resource allocation, authorization, lifecycle decisions, and structural evolution.

These are logical responsibilities rather than necessarily separate physical services.

The architecture supports hierarchical, distributed, and federated control arrangements, including local control at individual structural nodes and higher-level coordination across AI Relay systems.

We introduce a contract-first execution model, an evidence-based structural promotion protocol, and a bounded RSI lifecycle that separates candidate generation from independent evaluation and action authorization.

Particular attention is given to evaluator drift, reward hacking, correlated evidence, policy violations, uncontrolled recursion, and the risks of modifying both an intelligence system and its evaluators.

The central hypothesis is that a contract-governed Universal Control Plane can provide a reusable architectural foundation for composing heterogeneous intelligence resources and managing their structural evolution.

The term *Universal* describes the intended generality of the control abstractions, not a claim of demonstrated applicability to every intelligence system.

**Keywords:** Universal Control Plane, Structural RSI, Scoring Forest, Meta-Scoring Intelligence, Hybrid Structural Intelligence, AI Relay, Common Concept Core, Structural Folding, Policy Governance, Contract-First Architecture, Evidence-Driven Evolution, Distributed Control, Counter-Evidence

---

![Fig-007 — Universal Control Plane and Structural RSI](../figures/Fig-007-Universal-Control-Plane-and-Structural-RSI.png)

**Fig-007.** Evidence-driven and governed structural evolution under a Universal Control Plane.

---

## 1. Introduction

### 1.1 From Powerful Models to Governed Intelligence Systems

Modern AI systems increasingly operate through composite workflows rather than isolated model calls.

A complex workflow may include:

- Context localization;
- Task decomposition;
- Model selection;
- Specialized computation;
- Candidate generation;
- Scoring and ranking;
- Independent validation;
- Tool execution;
- Evidence collection;
- Structural learning.

These components may be implemented through different models, algorithms, services, or organizations.

The resulting architecture creates an important control problem.

Who determines which components should execute, how they should interact, what evidence is sufficient, and which structural changes should be accepted?

### 1.2 The Structural RSI Challenge

Recursive Self-Improvement is often discussed as the ability of an intelligence system to improve its own performance.

Structural RSI expands the potential modification space.

Instead of changing only model parameters or prompts, a system may propose changes to:

- Localization structures;
- Per-Node Intelligence Engines;
- Dispatch and Calling Graphs;
- Scoring Trees;
- Evaluation criteria;
- CCC structures;
- Context representations;
- Control policies;
- Computational resource allocation.

This creates a composite evolutionary system.

Such a system requires mechanisms for controlling not only computation, but also the evolution of its computational and evaluative structures.

### 1.3 The Control Plane Hypothesis

We propose:

> Complex Structural Intelligence systems require an explicit, governable control architecture that coordinates computation, evaluation, evidence, policy, and structural evolution.

The Universal Control Plane is intended to provide that architecture.

### 1.4 Research Scope

This paper develops a proposed system architecture and associated algorithms.

It does not demonstrate that a Universal Control Plane necessarily improves every AI system.

It does not establish a complete formal safety guarantee for Structural RSI.

The proposed architecture requires implementation, empirical validation, security analysis, and further formalization.

---

## 2. Foundations from the UCPSF Research Series

The preceding UCPSF papers establish complementary components.

### 2.1 UCPSF-001 — Generalized Scoring Intelligence

Scoring is treated as a potentially learnable and structurally organized intelligence capability rather than a fixed scalar reward.

### 2.2 UCPSF-002 — Three Scoring Operator Families

Three candidate operator families are introduced:

1. Value-Based Folding;
2. Branching-Based Folding;
3. ANN Scoring Nodes.

These operators support different forms of evaluation and structural transformation.

### 2.3 UCPSF-003 — Scoring Trees, Forests, and Unaligned AND Folding

Heterogeneous scoring mechanisms are represented as structured evaluation objects.

Unaligned AND Folding investigates reusable commonality across different scoring topologies and representations.

### 2.4 UCPSF-004 — Recursive CCC Distillation

Repeated structural comparison and independent validation may produce reusable Common Concept Cores.

These cores remain revisable and retain Specialized Delta, applicability boundaries, and counter-evidence.

### 2.5 UCPSF-005 — Perspective-Aware Meta-Scoring

Evaluators themselves become objects of evaluation.

The system can select evaluation mechanisms according to Perspective, cost, risk, applicability, and validation evidence.

### 2.6 UCPSF-006 — Dual-Hybrid Structural Intelligence

Localization Intelligence and Per-Node Intelligence become separately selectable architectural functions.

Multiple Localization Engines and Intelligence Engines may be composed under explicit contracts.

### 2.7 Architectural Integration

Together, these components motivate a higher-level architecture:

**Hybrid Intelligence + Scoring Intelligence + Structural Learning + Governance → Universal Control Plane.**

The Control Plane provides coordination across these functions.

---

## 3. What Is a Universal Control Plane?

### 3.1 Definition

A Universal Control Plane is a logical system responsible for selecting, coordinating, evaluating, authorizing, and evolving structural intelligence operations under explicit constraints.

A conceptual representation is:

$$
UCP = (P,C,L,I,S,M,E,G,A)
$$

where:

- $P$: Perspective management;
- $C$: Contracts and compatibility;
- $L$: Localization Engine management;
- $I$: Intelligence Engine management;
- $S$: Scoring Trees and Forests;
- $M$: Meta-Scoring;
- $E$: Evidence and structural learning;
- $G$: Governance and policy;
- $A$: Audit and lifecycle control.

This representation describes functional responsibilities rather than a required implementation topology.

### 3.2 Control Plane Versus Execution Plane

The Execution Plane performs task computation.

The Control Plane determines:

- What should execute;
- Which resources should be used;
- Which constraints apply;
- How results should be evaluated;
- Whether further computation is justified;
- Whether a proposed structural change may be promoted.

### 3.3 Control Plane Versus Scoring Function

A scoring function evaluates a candidate according to defined semantics.

A Control Plane may use many scoring functions.

However, it also manages:

- Authorization;
- Contracts;
- Resource budgets;
- Execution scheduling;
- Evidence;
- Structural lifecycle;
- Rollback.

Therefore, the Universal Control Plane is not reducible to a single scoring function.

### 3.4 Universal as an Architectural Aspiration

The architecture seeks reusable control abstractions across multiple domains.

However, some domains may require specialized control mechanisms or regulatory constraints.

Universal does not mean unrestricted authority or guaranteed cross-domain compatibility.

---

## 4. Three Logical Planes

### 4.1 Intelligence Execution Plane

The Execution Plane contains the computational mechanisms that perform tasks.

Potential components include:

- General-purpose LLMs;
- Specialized Transformers;
- ANN scorers;
- Principle Engines;
- Symbolic reasoning systems;
- Optimizers;
- Simulators;
- External tools;
- AI Relay workflows.

### 4.2 Evaluation and Scoring Plane

The Evaluation Plane contains mechanisms for assessing:

- Candidate quality;
- Structural changes;
- Localization quality;
- Engine performance;
- Risk;
- Computational cost;
- Transferability.

It may include:

- Scoring Trees;
- Scoring Forests;
- CCC evaluators;
- ANN evaluation models;
- Independent validators;
- Meta-Scoring mechanisms.

### 4.3 Governance and Control Plane

The Governance and Control Plane manages:

- Perspective;
- Policy;
- Contracts;
- Dispatch;
- Resource budgets;
- Authorization;
- Structural promotion;
- Evidence requirements;
- Rollback.

### 4.4 Logical Separation

The three planes may be implemented within one process or distributed across multiple systems.

Their separation is primarily conceptual and contractual.

For example, one model may participate in execution and evaluation, but independent validation must still be maintained where required.

### 4.5 Architectural Diagram

```text id="yfpq1s"
                    GOVERNANCE AND CONTROL
              +--------------------------------+
              | Perspective / Policy / Contracts|
              | Dispatch / Budget / Lifecycle   |
              | Authorization / Audit / Rollback|
              +---------------+----------------+
                              |
                              v
                    EVALUATION AND SCORING
              +--------------------------------+
              | Scoring Trees / Forests         |
              | CCC / Meta-Scoring              |
              | Independent Validation          |
              | Counter-Evidence                |
              +---------------+----------------+
                              |
                              v
                    INTELLIGENCE EXECUTION
              +--------------------------------+
              | Hybrid Localization            |
              | Hybrid Per-Node Intelligence    |
              | AI Relay / Tools / Simulation   |
              +---------------+----------------+
                              |
                              v
                         External Outcomes
                              |
                              v
                        Evidence Feedback
```

Control and feedback may operate bidirectionally.

The diagram is a logical overview rather than a complete runtime data-flow specification.

---

## 5. Perspective Management

### 5.1 Perspective as a Control Object

Following UCPSF-005, we represent Perspective as:

$$
P=(G,C,B,T,R)
$$

where:

- $G$: Goals;
- $C$: Context and constraints;
- $B$: Resource budget;
- $T$: Time horizon;
- $R$: Risk preferences.

### 5.2 Perspective-Conditioned Control

The same task may require different computational strategies under different perspectives.

For example:

**Exploratory Research**

May favor broad search, novelty, and uncertainty tolerance.

**Production Engineering**

May favor reliability, reproducibility, and cost control.

**Safety-Critical Operation**

May require stronger validation, explicit constraints, and escalation.

### 5.3 Perspective Is Not Policy Authority

Perspective describes objectives and operational preferences.

Policy determines which actions and structural modifications are permitted.

A user-selected Perspective should not automatically override higher-priority governance constraints.

### 5.4 Perspective Switching

The Control Plane may revise active evaluation and execution configurations when Perspective changes.

However, switching should preserve:

- Relevant state;
- Evidence provenance;
- Policy constraints;
- Audit history;
- Structural identity.

---

## 6. Contract-First Architecture

### 6.1 The Composition Problem

A Universal Control Plane may coordinate heterogeneous components.

These components may use different:

- Input schemas;
- Output semantics;
- Context representations;
- Identity systems;
- Confidence conventions;
- Policy assumptions.

Without explicit contracts, composition can produce silent semantic errors.

### 6.2 Specifications Before Runtime

We propose:

**Specifications / Contracts First → Conformance Validation → Runtime Composition.**

This establishes a disciplined sequence for introducing new components.

### 6.3 Capability Contract

Each intelligence component should declare:

- Component identity;
- Supported task types;
- Input and output schemas;
- Required context;
- Computational cost profile;
- Failure conditions;
- Evidence semantics;
- Policy requirements;
- Version.

### 6.4 Localization Contract

Localization Engines should specify:

- Structural references;
- Context identity;
- Relevance semantics;
- Coverage requirements;
- Provenance;
- Uncertainty;
- Applicability.

### 6.5 Scoring Contract

Scoring mechanisms should specify:

- Score type;
- Score direction;
- Calibration;
- Aggregation rules;
- Constraint semantics;
- Applicability;
- Validation evidence.

A probability should not be silently treated as a utility or ranking score.

### 6.6 Evolution Contract

A proposed structural modification should declare:

- Target component;
- Proposed change;
- Expected benefit;
- Compatibility impact;
- Evaluation plan;
- Rollback mechanism;
- Authorization requirements.

### 6.7 Conformance Testing

A component should not be promoted merely because its interface is syntactically compatible.

Semantic and behavioral conformance may also be required.

---

## 7. Hybrid Localization and Per-Node Intelligence Control

### 7.1 Engine Registries

The Control Plane may maintain:

$$
\mathcal{L}=\{L_1,\ldots,L_m\}
$$

for Localization Engines, and:

$$
\mathcal{I}=\{I_1,\ldots,I_n\}
$$

for Per-Node Intelligence Engines.

### 7.2 Candidate Composition

A candidate configuration may be represented as:

$$
a=(L_i,I_j,C_{ij})
$$

where $C_{ij}$ is the composition contract.

More complex configurations may form computational graphs.

### 7.3 Selection

The Control Plane may evaluate candidate configurations using:

- Expected task quality;
- Cost;
- Latency;
- Reliability;
- Context sufficiency;
- Risk;
- Policy compliance.

### 7.4 Adaptive Coupling

The Control Plane may choose between:

- A single integrated Transformer;
- A Transformer with external context;
- Modular localization and computation;
- Multi-engine hybrid composition.

The choice should be evidence-driven.

### 7.5 Engine Replacement

A component may be replaced if a candidate alternative satisfies:

- Contract compatibility;
- Required validation;
- Policy constraints;
- Acceptable cost;
- Promotion criteria.

### 7.6 Controlled Diversity

Architectural diversity is useful only when the system can evaluate and govern it.

The Control Plane should avoid uncontrolled proliferation of poorly validated components.

---

## 8. Scoring Forest Control

### 8.1 Evaluation Registry

The Control Plane may maintain a registry of:

- Scoring Trees;
- Scoring Forests;
- ANN scorers;
- CCC evaluators;
- Independent validators;
- Meta-Scoring mechanisms.

### 8.2 Perspective-Aware Selection

Evaluator selection depends on:

- Task type;
- Perspective;
- Available evidence;
- Risk;
- Resource budget;
- Applicability boundaries.

### 8.3 Scoring Composition

Multiple evaluators may be composed sequentially or in parallel.

For example:

```text id="jgv6e2"
Candidate Architecture
        |
        +--> Quality Scoring
        |
        +--> Cost Scoring
        |
        +--> Risk Evaluation
        |
        +--> Policy Constraints
        |
        v
Multi-Perspective Assessment
        |
        v
Decision Recommendation
```

### 8.4 Hard Constraints

Mandatory constraints should not be treated as compensable score dimensions.

A candidate that violates a required constraint may be ineligible regardless of its expected utility.

### 8.5 Meta-Scoring

Meta-Scoring evaluates the suitability and reliability of the scoring structures themselves.

### 8.6 Scoring Forest Evolution

Repeated evaluation may generate evidence for:

- New scoring branches;
- Operator refinement;
- CCC extraction;
- Specialized Delta;
- Evaluator retirement.

Such changes require independent validation.

---

## 9. Structural RSI as a Controlled Evolution Process

### 9.1 Structural Modification Space

Structural RSI may propose modifications to:

$$
\Theta =
(\Theta_L,\Theta_I,\Theta_S,\Theta_C,\Theta_D,\Theta_P)
$$

where:

- $\Theta_L$: Localization architecture;
- $\Theta_I$: Intelligence Engines;
- $\Theta_S$: Scoring structures;
- $\Theta_C$: Composition contracts;
- $\Theta_D$: Dispatch and Calling Graphs;
- $\Theta_P$: Policy-adjacent configuration.

The inclusion of policy-adjacent configuration does not imply that the system may autonomously rewrite its governing authority.

### 9.2 Candidate Generation

A candidate structural change may originate from:

- Human design;
- Automated search;
- Counter-evidence;
- Performance analysis;
- CCC extraction;
- AI Relay feedback;
- Specialized optimization.

### 9.3 Candidate Evaluation

Each candidate should be evaluated against:

- A reference baseline;
- Task-specific objectives;
- Robustness requirements;
- Cost;
- Transferability;
- Governance constraints.

### 9.4 Independent Validation

The evaluator used to justify a structural change should not be solely controlled by that change.

### 9.5 Promotion

A validated candidate may be promoted within an explicitly authorized scope.

### 9.6 Monitoring

Promoted changes should be monitored for:

- Performance degradation;
- Distribution shift;
- Unexpected interactions;
- Constraint violations;
- Resource anomalies.

### 9.7 Rollback

A promotion should be reversible when technically feasible.

Rollback plans should be defined before deployment.

---

## 10. Two-Level Structural Evolution

### 10.1 Intelligence Architecture Evolution

The first level modifies how tasks are computed.

Examples include:

- New Localization Engines;
- Specialized Per-Node Engines;
- Improved dispatch structures;
- Better context representations;
- Reusable hybrid workflows.

### 10.2 Evaluation Architecture Evolution

The second level modifies how candidate solutions and structural changes are evaluated.

Examples include:

- New scoring dimensions;
- Revised Scoring Trees;
- ANN scorer distillation;
- CCC refinement;
- Meta-Scoring improvements.

### 10.3 Coupled Evolution Risk

If the intelligence architecture and its evaluators change simultaneously, it may become difficult to determine whether apparent improvement is genuine.

### 10.4 Controlled Co-Evolution

We propose a staged approach:

1. Establish a reference evaluation baseline.
2. Generate a candidate intelligence modification.
3. Validate the modification independently.
4. Collect evidence about evaluator limitations.
5. Propose evaluator changes separately.
6. Validate evaluator changes against external references.
7. Promote changes through authorized lifecycle controls.

### 10.5 Non-Monotonic Progress

Structural evolution may include regressions, failed experiments, and rejected candidates.

A valid research process must preserve these outcomes as evidence.

---

## 11. Evidence, Counter-Evidence, and Anti-Goodhart Governance

### 11.1 Evidence as a First-Class Object

Evidence should include:

- Source identity;
- Collection conditions;
- Task and Perspective;
- Evaluator version;
- Candidate version;
- Observed outcomes;
- Uncertainty;
- Provenance.

### 11.2 Counter-Evidence

Counter-evidence may reveal:

- Missing scoring dimensions;
- Invalid CCC generalization;
- Unreliable engine selection;
- Distribution shift;
- Hidden policy conflicts;
- Long-tail failures.

### 11.3 Independent Evaluation

Independent validation may involve:

- Held-out benchmarks;
- External outcome measurements;
- Separate evaluation models;
- Formal checks;
- Human review;
- Adversarial testing.

Independence should be assessed in terms of shared data, model lineage, incentives, and control authority.

### 11.4 Anti-Goodhart Mechanisms

Candidate mechanisms include:

- Multiple evaluation perspectives;
- Independent reference tests;
- Counter-evidence search;
- Constraint preservation;
- Score calibration;
- Evaluator drift monitoring;
- Promotion thresholds.

### 11.5 Evaluator Drift

A system may improve internal scores while degrading external outcomes.

The Control Plane should detect disagreement between internal evaluation and independent evidence.

### 11.6 Evidence Before Promotion

The proposed principle is:

**No structural promotion without sufficient independent evidence for the intended scope.**

---

## 12. Distributed and Hierarchical Control Planes

### 12.1 Why Centralized Control May Be Insufficient

Large AI systems may contain many structural nodes, specialized engines, and independent execution environments.

A single centralized controller may create:

- Bottlenecks;
- High coordination cost;
- Single points of failure;
- Excessive global state requirements.

### 12.2 Hierarchical Control

A possible hierarchy is:

```text id="38j1af"
Global Governance Authority
            |
            v
System-Level Control Plane
            |
     +------+------+ 
     |             |
     v             v
Domain Control   Domain Control
     |             |
     v             v
Local Node       Local Node
Control          Control
```

### 12.3 Local Control Responsibilities

A local controller may manage:

- Task-specific dispatch;
- Local scoring;
- Resource use;
- Retry and escalation;
- Evidence collection.

### 12.4 System-Level Responsibilities

A system-level controller may manage:

- Cross-domain resource allocation;
- Shared evaluator registries;
- CCC promotion;
- Cross-component contracts;
- System-wide monitoring.

### 12.5 Governance Authority

Higher-level governance may define non-delegable constraints.

Local controllers should not be able to override those constraints through favorable scores.

### 12.6 Federated Control

Independent organizations or BrainUnits may retain local ownership while exchanging portable intelligence structures.

Federated control requires explicit trust, identity, and authorization mechanisms.

### 12.7 Control Plane Consistency

Distributed control introduces additional challenges:

- Conflicting policies;
- Stale evaluator versions;
- Inconsistent evidence;
- Partial failures;
- Cross-node authorization;
- Rollback coordination.

These problems require dedicated engineering mechanisms.

---

## 13. PIRP/PIRU and Portable Intelligence

### 13.1 Structural Exchange

Portable Intelligence Runtime Pieces and Units provide a candidate framework for exchanging reusable intelligence components.

### 13.2 Portable Components

Potential portable objects include:

- Scoring CCCs;
- Localization components;
- Evaluation operators;
- Hybrid workflow structures;
- Principle Engines;
- Contract definitions.

### 13.3 Portability Requirements

A portable intelligence component should preserve:

- Identity;
- Version;
- Capability declaration;
- Input-output contracts;
- Applicability;
- Evidence;
- Policy requirements.

### 13.4 Local Adaptation

A portable component may require localization to the receiving environment.

This may involve:

- Context mapping;
- UTN resolution;
- Contract adaptation;
- Perspective alignment;
- Validation.

### 13.5 Collective Structural Learning

Multiple systems may contribute reusable components and evidence.

However, collective learning should not imply unrestricted trust or automatic promotion.

---

## 14. Universal Control Plane Runtime Cycle

### 14.1 Proposed Execution Lifecycle

A candidate runtime cycle is:

```text id="e4o70a"
Task / Goal
    |
    v
Perspective and Policy Resolution
    |
    v
Contract and Capability Localization
    |
    v
Hybrid Architecture Selection
    |
    v
Execution
    |
    v
Scoring Forest Evaluation
    |
    v
Independent Validation
    |
    v
Decision / Escalation / Stop
    |
    v
Evidence Recording
    |
    v
Structural Learning Proposal
    |
    v
Governed Promotion / Rejection
```

### 14.2 Separation of Execution and Learning

Not every task execution should trigger structural modification.

Learning may occur:

- Online;
- Periodically;
- In isolated experiments;
- Through offline validation;
- Under human supervision.

### 14.3 Resource-Aware Control

The Control Plane should account for:

- Evaluation cost;
- Execution cost;
- Latency;
- Energy or infrastructure cost;
- Expected future reuse;
- Risk.

### 14.4 Stopping Conditions

The Control Plane should stop or escalate when:

- Resource budgets are exhausted;
- Expected improvement is insufficient;
- Required evidence is unavailable;
- Policy constraints are violated;
- Uncertainty exceeds acceptable limits;
- Repeated attempts fail to make progress.

---

## 15. Proposed Control Algorithm

```text id="1fapd3"
Algorithm: Universal-Control-Plane-Structural-RSI

Input:
    Task X
    Perspective P
    Localization Registry L
    Intelligence Registry I
    Scoring Forest S
    CCC Registry K
    Contract Registry C
    Evidence Repository E
    Policy Rules G
    Resource Budget B

Output:
    Task Result Y
    Decision Trace T
    Optional Structural Change Proposal R

1. Resolve Perspective P.

2. Resolve applicable governance constraints G.

3. Identify mandatory contracts.

4. Localize candidate Localization Engines.

5. Localize candidate Intelligence Engines.

6. Generate valid hybrid configurations.

7. Reject contract-incompatible configurations.

8. Reject policy-ineligible configurations.

9. Meta-score remaining configurations.

10. Select configuration under budget B.

11. Execute task through selected configuration.

12. Evaluate output using applicable Scoring Trees.

13. Check constraints and uncertainty.

14. If additional evaluation is justified:
        Escalate within authorized limits.

15. Produce task result and evidence trace.

16. Apply independent authorization
    before external actions.

17. Record outcomes and evaluator versions.

18. Detect potential structural improvement.

19. If improvement is plausible:
        Generate a structural change proposal.

20. Validate proposal against reference baselines.

21. Search for counter-evidence.

22. Check promotion contracts and authority.

23. Promote, reject, revise, or quarantine proposal.

24. Monitor promoted changes.

25. Roll back when required and feasible.

26. Update CCC and evaluator registries
    through separately governed procedures.

27. Return Y, T, and optional proposal R.
```

The algorithm is conceptual.

A production implementation would require explicit transaction semantics, concurrency controls, authorization enforcement, and failure recovery.

---

## 16. Structural RSI Promotion Protocol

### 16.1 Candidate States

We propose:

```text id="03r7if"
Proposed
    |
    v
Contract-Checked
    |
    v
Sandboxed
    |
    v
Independently Validated
    |
    v
Authorized
    |
    v
Canary Deployment
    |
    v
Promoted
    |
    +--> Monitored
    |
    +--> Rolled Back
    |
    +--> Retired
```

### 16.2 Contract-Checked

The candidate must satisfy required interface and capability contracts.

### 16.3 Sandboxed

The candidate is evaluated in a controlled environment.

### 16.4 Independently Validated

Reference tests and external evidence assess its performance.

### 16.5 Authorized

A governance authority determines whether promotion is permitted.

### 16.6 Canary Deployment

Where applicable, the candidate may be introduced to a limited scope before broader promotion.

### 16.7 Promoted

The candidate becomes available for authorized use.

### 16.8 Monitored

Post-promotion evidence is collected.

### 16.9 Rolled Back

The system restores a previous validated configuration when necessary and feasible.

### 16.10 Promotion Principle

**A favorable internal score is necessary in some workflows, but never sufficient by itself for structural promotion.**

---

## 17. Failure Modes and Defensive Architecture

### 17.1 Reward Hacking

A candidate may exploit weaknesses in the evaluator.

**Mitigation:** Independent outcome testing and counter-evidence.

### 17.2 Evaluator Capture

A modified system may influence the criteria used to assess itself.

**Mitigation:** Separation of evaluator authority and immutable reference controls where appropriate.

### 17.3 Contract Drift

Components may change behavior without updating declared contracts.

**Mitigation:** Versioned conformance testing.

### 17.4 Policy Bypass

A local controller may attempt an action outside its authority.

**Mitigation:** Independent authorization enforcement.

### 17.5 Structural Overgrowth

The system may accumulate excessive components and CCC variants.

**Mitigation:** Lifecycle management, cost accounting, and retirement.

### 17.6 Recursive Instability

Repeated changes may create unforeseen interactions.

**Mitigation:** Bounded modification depth, staged promotion, and rollback.

### 17.7 Correlated Validation

Multiple evaluators may share the same underlying bias.

**Mitigation:** Evidence lineage and evaluator independence analysis.

### 17.8 Distributed Inconsistency

Different controllers may operate with conflicting versions or policies.

**Mitigation:** Explicit consistency, synchronization, and authority protocols.

### 17.9 Long-Tail Failures

Rare conditions may escape standard validation.

**Mitigation:** Counter-evidence search, stress testing, and risk-sensitive escalation.

---

## 18. Validation Framework

### 18.1 Research Hypotheses

**H1 — Architectural Coordination**

An explicit Control Plane can improve coordination of heterogeneous intelligence components under specified workloads.

**H2 — Perspective-Aware Dispatch**

Scoring-guided selection can improve task quality or resource efficiency relative to fixed configurations.

**H3 — Governed Structural RSI**

Independent validation and promotion controls can reduce unsafe or ineffective structural changes.

**H4 — Evaluator Evolution**

Separately governed evaluator updates can improve evaluation quality without relying solely on self-assessment.

**H5 — Distributed Control**

Hierarchical or federated control can support larger systems while preserving defined authority boundaries.

### 18.2 Baselines

Candidate baselines include:

1. Single integrated model;
2. Fixed multi-agent workflow;
3. Dynamic routing without a unified Control Plane;
4. Scoring-guided dispatch without independent validation;
5. Structural RSI without separate evaluator governance;
6. Full Universal Control Plane architecture.

### 18.3 Experimental Campaigns

**Campaign A — Hybrid Dispatch**

Compare fixed and dynamic engine configurations.

**Campaign B — Scoring Forest Selection**

Measure the quality and cost of perspective-aware evaluator selection.

**Campaign C — Structural Promotion**

Evaluate promotion decisions under controlled structural changes.

**Campaign D — Evaluator Drift**

Introduce misleading evaluator updates and measure detection rates.

**Campaign E — Counter-Evidence**

Test whether rare failure cases trigger appropriate rejection or specialization.

**Campaign F — Distributed Control**

Evaluate coordination overhead and consistency under hierarchical control.

### 18.4 Metrics

| Metric | Purpose |
|---|---|
| Task Utility | Downstream outcome quality |
| Total Cost | Execution, evaluation, and control overhead |
| Latency | End-to-end response time |
| Contract Conformance | Interface and semantic compatibility |
| Policy Violation Rate | Governance effectiveness |
| Promotion Precision | Quality of accepted structural changes |
| Rollback Reliability | Recovery from failed promotions |
| Evaluator Drift Detection | Detection of evaluation degradation |
| Structural Reuse | Reuse of validated components and CCCs |
| System Robustness | Stability under faults and distribution shift |

### 18.5 Validation Status

This paper proposes a research architecture.

No universal performance improvement or complete governance guarantee is claimed.

---

## 19. Open Research Questions

**RQ-001:** What is the minimal useful Universal Control Plane interface?

**RQ-002:** Which control responsibilities should be centralized, distributed, or delegated?

**RQ-003:** How can contract semantics remain consistent across heterogeneous intelligence engines?

**RQ-004:** How should Scoring Forests be selected and composed under changing Perspectives?

**RQ-005:** What independent validation requirements are sufficient for bounded Structural RSI?

**RQ-006:** How should evaluator changes be governed separately from intelligence architecture changes?

**RQ-007:** What formal authorization boundaries are required for distributed control?

**RQ-008:** How can CCC promotion, specialization, and rollback be implemented reliably?

**RQ-009:** How should a Control Plane detect and manage evaluator drift?

**RQ-010:** Can portable intelligence components support federated structural learning without compromising local sovereignty?

**RQ-011:** What cost models justify recursive structural improvement?

**RQ-012:** How can long-tail failures be preserved during aggressive Scoring Folding?

**RQ-013:** How should distributed Control Planes resolve conflicting policy and evaluation results?

**RQ-014:** What measurable advantages distinguish a Universal Control Plane from conventional orchestration frameworks?

---

## 20. Relationship to the UCPSF Research Series

### UCPSF-001

Introduces Generalized Scoring Intelligence.

### UCPSF-002

Defines three candidate Scoring Operator families.

### UCPSF-003

Develops Scoring Trees, Scoring Forests, and Unaligned AND Folding.

### UCPSF-004

Introduces recursive CCC extraction and evidence-driven structural growth.

### UCPSF-005

Develops Perspective-Aware Optimization and Meta-Scoring Intelligence.

### UCPSF-006

Proposes Dual-Hybrid Localization and Per-Node Intelligence.

### UCPSF-008

Explores open-ended Scoring Intelligence and the long-term evolution of governed hybrid AI systems.

---

## 21. Conclusion

Complex AI Relay and Structural RSI systems require coordination across heterogeneous intelligence engines, evaluation structures, computational resources, and governance constraints.

This paper proposes a Universal Control Plane architecture that integrates:

1. Perspective management;
2. Contract-first Hybrid Intelligence composition;
3. Scoring Trees and Forests;
4. Meta-Scoring Intelligence;
5. Recursive CCC distillation;
6. Independent validation;
7. Policy and authorization controls;
8. Evidence-driven Structural RSI.

The architecture distinguishes execution, evaluation, and governance as separate logical responsibilities.

It supports centralized, hierarchical, and federated implementations, while requiring explicit authority boundaries and traceable structural evolution.

Its central principle is:

> **Intelligence may generate and evaluate structural improvements, but structural promotion and external action must remain governed by explicit contracts, independent evidence, and authorized control.**

The Universal Control Plane is therefore not simply an orchestration layer or a scoring aggregator.

It is proposed as a reusable architecture for coordinating the execution, evaluation, and controlled evolution of heterogeneous intelligence systems.

The next paper, UCPSF-008, explores the broader implications of this framework for open-ended Scoring Intelligence, Collective Structural Learning, and future AI architectures.

---

## Suggested Figure Placement

### Fig-007 — Universal Control Plane and Structural RSI

**File:** `../figures/Fig-007-Universal-Control-Plane-and-Structural-RSI.png`

**Suggested insertion:** After Section 9.

**Purpose:** Illustrate the interaction between Hybrid Intelligence execution, Scoring Forest evaluation, Meta-Scoring, governance, and controlled Structural RSI.

### Fig-001 — Universal Control Plane Grand Map

**File:** `../figures/Fig-001-Universal-Control-Plane-Grand-Map.png`

**Suggested insertion:** After Section 4.

**Purpose:** Present the integrated architecture of Perspective management, Hybrid Localization, Per-Node Intelligence, Scoring Forests, CCC growth, policy, and audit.

---

## Citation

Suggested citation prior to DOI assignment:

Tan, S., & GPT-Obot. (2026). *UCPSF-007: Universal Control Plane Architecture and Structural RSI*. Universal Control Planes and Scoring Tree/Forest/Folding for Structural Intelligence, Version 1.0.0.

Repository:

https://github.com/sizhet/Universal-Control-Planes-and-Scoring-Folding

DOI: To be assigned after the initial archived release.

---

## License

Copyright © 2026 Sizhe Tan & GPT-Obot.

Licensed under the Apache License, Version 2.0.

---

**Document:** UCPSF-007  
**Research Series:** Universal Control Planes and Scoring Tree/Forest/Folding  
**Status:** Proposed System Architecture and Research Framework  
**Version:** 1.0.0
