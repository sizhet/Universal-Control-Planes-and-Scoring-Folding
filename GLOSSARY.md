
# GLOSSARY — Universal Control Planes and Scoring Tree/Forest/Folding

**Canonical Terminology, Conceptual Definitions, and Semantic Boundaries**

**Project:** Universal Control Planes and Scoring Tree/Forest/Folding for Structural Intelligence (UCPSF)  
**Authors:** Sizhe Tan & GPT-Obot  
**Version:** 1.0.0  
**Date:** October 15, 2026  
**Status:** Canonical Research Glossary  
**License:** Apache-2.0

---

## 1. Purpose and Scope

This glossary establishes consistent terminology for the UCPSF research framework.

UCPSF investigates the structural representation, composition, evaluation, governance, and recursive improvement of intelligence systems.

Its central research proposition is:

> **Scoring Intelligence itself can become a structurally learnable, transferable, and recursively improvable form of intelligence.**

The glossary serves four purposes:

1. Define the principal concepts used throughout the repository.
2. Distinguish related concepts that should not be treated as equivalent.
3. Establish semantic foundations for future specifications and contracts.
4. Identify proposed terminology that remains subject to formalization and empirical validation.

Definitions are organized by conceptual domain rather than strictly alphabetically.

The terms **Universal**, **Generalized**, and **Open-Ended** express research ambitions or architectural scope. They should not be interpreted as demonstrated guarantees.

---

## 2. Foundational Intelligence Concepts

### 2.1 Structural Intelligence (SI)

**Definition:** An approach to intelligence that emphasizes explicit or recoverable structures for representing, organizing, composing, evaluating, and evolving knowledge and computational behavior.

Structural Intelligence may involve:

- Differential structures;
- Trees and graphs;
- Calling Graphs;
- Common Concept Cores;
- Structural localization;
- Specialized intelligence components;
- Evidence-driven structural growth.

**Distinction:** Structural Intelligence is not synonymous with symbolic AI. Its proposed structures may include learned, probabilistic, neural, and hybrid mechanisms.

### 2.2 Generalized Scoring Intelligence (GSI)

**Definition:** A proposed intelligence capability for selecting, composing, adapting, evaluating, and improving scoring mechanisms across tasks, contexts, and Perspectives.

GSI extends beyond computing a numerical score.

It may involve:

- Metric selection;
- Evaluation decomposition;
- Scoring Tree construction;
- Scoring Forest selection;
- Uncertainty assessment;
- Meta-Scoring;
- Structural learning.

**Research status:** Proposed architectural concept.

### 2.3 Scoring Function

**Definition:** A mapping that assigns an evaluative value or structured evaluation result to an input under specified conditions.

A simple representation is:

$$
s:X\rightarrow\mathbb{R}
$$

More general scoring mechanisms may return vectors, rankings, categorical decisions, uncertainty estimates, or evidence records.

**Distinction:** A Scoring Function computes an evaluation. Scoring Intelligence may decide which function to use, how to interpret it, and whether it should be revised.

### 2.4 Scoring Intelligence

**Definition:** The capability to reason about, select, organize, compose, and improve evaluation mechanisms.

A Scoring Intelligence system may evaluate:

- Candidate outputs;
- Computational paths;
- Intelligence Engines;
- Structural modifications;
- Other evaluators.

**Key distinction:**

> A Scoring Function produces an evaluation; Scoring Intelligence manages and improves the process of evaluation.

### 2.5 Primitive Scoring

**Definition:** Evaluation performed through a relatively simple or fixed mechanism, such as a scalar metric, threshold, or predefined ranking rule.

Examples include:

- Pass/fail checks;
- Weighted sums;
- Similarity scores;
- Fixed confidence thresholds.

Primitive Scoring remains useful and may be preferable when additional structural complexity is unnecessary.

### 2.6 Rich Evaluator

**Definition:** An evaluation mechanism that considers multiple relevant dimensions, potentially including quality, risk, cost, uncertainty, evidence, and task-specific constraints.

A Rich Evaluator may be implemented through a Scoring Tree, Scoring Forest, or another structured evaluation architecture.

**Distinction:** Richness refers to relevant evaluative coverage, not simply the number of metrics.

### 2.7 Evaluation Intelligence

**Definition:** A general term for capabilities involved in assessing outcomes, processes, models, or structural changes.

Within UCPSF, Generalized Scoring Intelligence is a proposed structural approach to Evaluation Intelligence.

---

## 3. Metrics, Scores, and Evaluation Semantics

### 3.1 Metric

**Definition:** A defined measure used to assess an attribute of a system, object, process, or outcome.

Examples include:

- Accuracy;
- Latency;
- Cost;
- Reliability;
- Regression rate.

Not every evaluation criterion is necessarily a mathematical metric in the strict sense.

### 3.2 Metric Distance

**Definition:** A measure of separation or difference between objects or states.

In a strict mathematical metric space, a distance function satisfies non-negativity, identity of indiscernibles, symmetry, and the triangle inequality.

UCPSF may also investigate generalized distances or dissimilarity measures that do not satisfy every metric axiom.

Such cases should be explicitly identified.

### 3.3 Score

**Definition:** An evaluative result produced by a scoring mechanism.

A score may be:

- Scalar;
- Vector-valued;
- Ordinal;
- Probabilistic;
- Categorical;
- Structured.

### 3.4 Score Normalization

**Definition:** A transformation intended to place scores on a comparable scale or reduce unwanted dependence on factors such as input length or magnitude.

Normalization does not automatically establish calibration or semantic comparability.

### 3.5 Score Calibration

**Definition:** The process of aligning score interpretations with observed reference outcomes.

For probabilistic scores, calibration concerns the relationship between predicted probabilities and observed frequencies.

### 3.6 Evaluation Criterion

**Definition:** A specified property or condition against which a candidate is assessed.

Criteria may be quantitative or qualitative.

### 3.7 Evaluation Evidence

**Definition:** Information supporting or challenging an evaluative conclusion.

Examples include:

- Test outcomes;
- External measurements;
- Independent reviews;
- Failure traces;
- Benchmark results.

### 3.8 Evaluation Trace

**Definition:** A record of evaluation steps, selected mechanisms, intermediate results, and decisions.

Traces support reproducibility, auditing, and structural learning.

### 3.9 Evaluation Uncertainty

**Definition:** Uncertainty associated with an evaluation result or the applicability of an evaluator.

Sources may include:

- Limited evidence;
- Model uncertainty;
- Distribution shift;
- Measurement error;
- Missing context.

### 3.10 Evaluation Budget

**Definition:** Resources allocated to evaluation.

Budgets may include:

- Compute;
- Time;
- Monetary cost;
- Model calls;
- Human review capacity.

---

## 4. Scoring Structures

### 4.1 Scoring Node

**Definition:** An individual evaluation component within a larger scoring structure.

A node may perform:

- Metric computation;
- Rule checking;
- Learned scoring;
- Aggregation;
- Branch selection;
- Evidence collection.

### 4.2 Scoring Tree

**Definition:** A structured evaluation system organized through hierarchical relationships among Scoring Nodes.

A conceptual representation is:

$$
T_S=(V,E,O,\Sigma,P,C)
$$

where:

- $V$: Evaluation nodes;
- $E$: Structural relationships;
- $O$: Evaluation operators;
- $\Sigma$: Scoring semantics;
- $P$: Perspective information;
- $C$: Constraints and contracts.

This representation is a research abstraction rather than a finalized implementation schema.

### 4.3 Scoring Forest

**Definition:** A collection of Scoring Trees that may represent multiple tasks, domains, Perspectives, or evaluation strategies.

A Scoring Forest may support:

- Specialized evaluation;
- Multi-Perspective comparison;
- Adaptive evaluator selection;
- Structural reuse;
- Recursive distillation.

### 4.4 Scoring Graph

**Definition:** A scoring structure containing general graph relationships rather than strictly hierarchical tree relationships.

Scoring Graphs may support shared substructures, feedback, or cross-branch dependencies.

### 4.5 Local Scoring

**Definition:** Evaluation of an individual component, intermediate result, or localized decision.

### 4.6 Global Scoring

**Definition:** Evaluation of a complete workflow, system outcome, or composite structural configuration.

**Distinction:** Strong local scores do not necessarily imply strong global outcomes.

### 4.7 Hierarchical Scoring

**Definition:** Evaluation organized across multiple levels of abstraction or composition.

### 4.8 Multi-Perspective Scoring

**Definition:** Evaluation performed under multiple explicitly defined Perspectives.

Different Perspectives may produce different rankings without implying evaluator malfunction.

### 4.9 Scoring Aggregation

**Definition:** Combining multiple evaluative results into a higher-level representation or decision.

Aggregation may use:

- Weighted combinations;
- Lexicographic rules;
- Pareto comparisons;
- Constraints;
- Learned composition.

### 4.10 Scoring Semantics

**Definition:** The meaning, scale, applicability, uncertainty, and interpretation of a score or scoring operation.

Two numerical scores should not be assumed comparable without compatible semantics.

---

## 5. Three Scoring Operator Families

UCPSF proposes three broad families of scoring-related structural operations.

These are candidate architectural abstractions, not an exhaustive taxonomy.

### 5.1 Value-Based Folding

**Definition:** A proposed family of operations that adjusts, combines, calibrates, normalizes, or compresses evaluative values and parameters.

Examples include:

- Weight adjustment;
- Score normalization;
- Metric aggregation;
- Parameter compression;
- Calibration.

**Research question:** Under what conditions can value-level transformations preserve decision-relevant evaluation behavior?

### 5.2 Branching-Based Folding

**Definition:** A proposed family of operations that reorganizes, merges, specializes, or reduces branches within a scoring or decision structure.

Examples include:

- Branch pruning;
- Conditional routing;
- Subtree reuse;
- Decision-path compression;
- Specialized branch creation.

**Research question:** How can branching transformations preserve important decision boundaries?

### 5.3 ANN Scoring Node

**Definition:** A learned scoring component implemented through an artificial neural network or related learned approximation mechanism.

Potential uses include:

- Ranking;
- Quality estimation;
- Routing;
- Distillation;
- Fast approximate evaluation.

**Distinction:** ANN Scoring Nodes are implementation mechanisms, whereas Value-Based and Branching-Based Folding describe broader structural operations.

The three families therefore should not be assumed to form a mutually exclusive mathematical partition.

### 5.4 Operator Composition

**Definition:** The combination of multiple scoring operators into a larger evaluation structure.

Composition may be:

- Sequential;
- Parallel;
- Conditional;
- Hierarchical;
- Iterative.

### 5.5 Operator Contract

**Definition:** A specification of an operator's input requirements, output semantics, constraints, uncertainty representation, and compatibility conditions.

A conceptual operator interface is:

$$
O:(X,P,E,C)\rightarrow(Y,S,U,T)
$$

where:

- $X$: Input;
- $P$: Perspective;
- $E$: Evidence;
- $C$: Constraints;
- $Y$: Output;
- $S$: Score;
- $U$: Uncertainty;
- $T$: Trace.

---

## 6. Structural Folding and Common Concept Cores

### 6.1 Structural Folding

**Definition:** A proposed process for transforming complex structures into more compact, reusable, or generalized representations while preserving specified essential properties.

Possible objectives include:

- Reduced redundancy;
- Improved reuse;
- Lower evaluation cost;
- Better transferability;
- Simpler composition.

Folding is not automatically lossless.

### 6.2 Structural Unfolding

**Definition:** A process that expands a compact or generalized representation into a more detailed, specialized, or executable structure.

Unfolding may depend on:

- Perspective;
- Context;
- Contracts;
- Specialized Delta;
- External evidence.

### 6.3 Aligned Folding

**Definition:** Folding across structures with sufficiently corresponding components or topologies to support direct alignment.

### 6.4 Unaligned Folding

**Definition:** Folding across structures that do not share a directly aligned representation or topology.

### 6.5 Unaligned AND Folding

**Definition:** A proposed structural operation that seeks common structural, semantic, or behavioral content across heterogeneous structures without requiring direct node-by-node alignment.

The term **AND** denotes a search for shared or jointly supported content.

It does not imply literal set intersection in every implementation.

**Research challenge:** Defining valid matching, preservation, and generalization criteria.

### 6.6 Common Concept Core (CCC)

**Definition:** A reusable representation of common structural, semantic, or behavioral content extracted from related objects or processes.

A CCC may support:

- Transfer;
- Reuse;
- Specialization;
- Structural learning;
- Evaluation composition.

A CCC is a candidate abstraction whose applicability must be validated.

### 6.7 Structural CCC

**Definition:** A CCC emphasizing common structural organization, relationships, or composition patterns.

### 6.8 Behavioral CCC

**Definition:** A CCC emphasizing common input-output behavior, decision patterns, or transition properties.

### 6.9 Semantic CCC

**Definition:** A CCC emphasizing shared meaning or functional interpretation across different representations.

### 6.10 Core±Delta

**Definition:** A representation in which a reusable core is combined with preserved specialized differences.

A conceptual decomposition is:

$$
T_i\approx K\oplus\Delta_i
$$

where:

- $T_i$: Original structure;
- $K$: Common Concept Core;
- $\Delta_i$: Specialized Delta.

The approximation symbol acknowledges that preservation may be incomplete or conditional.

### 6.11 Specialized Delta

**Definition:** Information or behavior that distinguishes a specific structure from its shared core.

A Specialized Delta may preserve:

- Domain-specific rules;
- Risk-sensitive branches;
- Context-specific parameters;
- Rare decision conditions.

### 6.12 Aspen Grove Model

**Definition:** A conceptual analogy in which individual Scoring Trees share reusable structural roots while retaining distinct branches and behaviors.

The analogy emphasizes:

- Shared intelligence foundations;
- Specialized adaptation;
- Collective learning;
- Open-ended growth.

It is not a literal biological or computational equivalence.

### 6.13 Recursive CCC Distillation

**Definition:** A proposed process in which candidate CCCs are repeatedly extracted, compared, refined, specialized, and validated across multiple structural levels.

### 6.14 CCC Promotion

**Definition:** The governed acceptance of a validated CCC into a reusable structural registry.

### 6.15 CCC Splitting

**Definition:** Dividing an overgeneralized CCC into more specialized representations when evidence reveals incompatible behaviors.

### 6.16 CCC Retirement

**Definition:** Removing a CCC from active use when it becomes invalid, redundant, or unsuitable.

---

## 7. Perspective and Meta-Scoring

### 7.1 Perspective

**Definition:** An explicit representation of task objectives, operating context, constraints, resources, time horizon, and risk preferences.

UCPSF proposes:

$$
P=(G,C,B,T,R)
$$

where:

- $G$: Goals;
- $C$: Context and constraints;
- $B$: Budget;
- $T$: Time horizon;
- $R$: Risk preferences.

### 7.2 Perspective-Aware Optimization

**Definition:** Optimization that conditions evaluation and selection on a defined Perspective.

A solution may be preferred under one Perspective but not another.

### 7.3 Perspective Drift

**Definition:** A change in the intended or applied evaluation Perspective over time.

Uncontrolled Perspective Drift may invalidate comparisons across experiments.

### 7.4 Meta-Scoring Intelligence

**Definition:** The capability to evaluate, compare, select, and improve scoring mechanisms.

Meta-Scoring may consider:

- Calibration;
- Predictive validity;
- Robustness;
- Applicability;
- Cost;
- Independence;
- Transferability.

### 7.5 Meta-Evaluator

**Definition:** A mechanism that evaluates another evaluator.

### 7.6 Evaluator Selection

**Definition:** Choosing an evaluation mechanism appropriate to a task, Perspective, and available evidence.

### 7.7 Evaluator Drift

**Definition:** A change in evaluator behavior or reliability over time.

Evaluator Drift may result from:

- Model updates;
- Distribution shift;
- Revised scoring criteria;
- Changed task composition;
- Feedback contamination.

### 7.8 Evaluator Independence

**Definition:** The degree to which an evaluator's judgments are not compromised by dependence on the candidate or optimization process it evaluates.

Independence may be partial rather than absolute.

### 7.9 Value of Information (VOI)

**Definition:** The expected benefit of acquiring additional information or performing further evaluation, accounting for its cost.

VOI may guide:

- Additional tests;
- Rich evaluation;
- Specialist review;
- Escalation;
- Stopping decisions.

### 7.10 Bounded Meta-Scoring

**Definition:** Meta-evaluation constrained by explicit recursion depth, cost, time, or stopping criteria.

---

## 8. Hybrid Localization and Per-Node Intelligence

### 8.1 Localization Intelligence

**Definition:** The capability to identify, retrieve, organize, or select context relevant to a task.

Localization may involve:

- Semantic retrieval;
- Attention-based contextual processing;
- Structural search;
- Graph traversal;
- CCC matching;
- Identity resolution.

### 8.2 Per-Node Intelligence

**Definition:** Task-specific computation performed using localized information or structural context.

Per-Node Intelligence may involve:

- Reasoning;
- Generation;
- Scoring;
- Verification;
- Optimization;
- Simulation.

### 8.3 Localization Engine

**Definition:** A computational mechanism implementing Localization Intelligence.

### 8.4 Per-Node Intelligence Engine

**Definition:** A computational mechanism implementing task-specific reasoning, generation, evaluation, or other processing.

### 8.5 Dual-Hybrid Intelligence

**Definition:** A proposed architecture in which multiple Localization Engines and multiple Per-Node Intelligence Engines can be selected and composed adaptively.

### 8.6 Hybrid Configuration

**Definition:** A compatible combination of Localization and Per-Node Intelligence mechanisms.

A conceptual representation is:

$$
a=(L_i,I_j,C_{ij})
$$

where $C_{ij}$ is the applicable composition contract.

### 8.7 Adaptive Coupling

**Definition:** Selecting how tightly Localization and Per-Node Intelligence should be integrated for a task.

### 8.8 Adaptive Decoupling

**Definition:** Separating Localization and Per-Node functions when modular composition offers validated benefits.

### 8.9 Integrated Intelligence Architecture

**Definition:** An architecture in which context processing and task computation are tightly coupled within one computational system.

Transformer-based models provide an important example.

### 8.10 Contract-Aware Composition

**Definition:** Combining components only when their interfaces, semantics, capabilities, and constraints are compatible.

### 8.11 Context Identity

**Definition:** The ability to distinguish and consistently reference a context object across processing stages.

### 8.12 Context Sufficiency

**Definition:** The extent to which localized context contains the information necessary for a specified task.

Context Sufficiency should be evaluated relative to task requirements rather than raw context size.

---

## 9. Related Structural Intelligence Mechanisms

### 9.1 Metric Differential Tree (MDT)

**Definition:** A structural representation organizing objects or information through hierarchical metric or differential relationships.

Within UCPSF, MDT is a candidate Localization mechanism.

### 9.2 UTN

**Definition:** A structural identity and reference mechanism used within the broader Structural Intelligence research program.

UTN-based representations may support context-aware identity, localization, and structural interoperability.

The exact semantics depend on the relevant UTN specification.

### 9.3 Context-Bound Token (CBT)

**Definition:** A token or structural reference whose interpretation is explicitly associated with context.

### 9.4 Calling Graph

**Definition:** A graph representing computational calls, dependencies, transitions, or related execution relationships.

Calling Graphs may support:

- Localization;
- Workflow analysis;
- Dispatch;
- Structural learning.

### 9.5 Principle Engine

**Definition:** A proposed computational mechanism that applies reusable principles or structural rules to a task.

### 9.6 PIRP — Portable Intelligence Runtime Piece

**Definition:** A portable intelligence component or representation intended for flexible reuse and exchange.

### 9.7 PIRU — Portable Intelligence Runtime Unit

**Definition:** A more formally specified portable intelligence unit with defined interfaces or contracts.

### 9.8 Collective Structural Learning (CSL)

**Definition:** A proposed learning process in which reusable structural intelligence components, evidence, and improvements can be exchanged or accumulated across multiple systems or participants.

### 9.9 BrainUnit

**Definition:** A conceptually bounded intelligence unit with identifiable responsibilities, resources, context, and governance boundaries.

---

## 10. Universal Control Plane

### 10.1 Universal Control Plane (UCP)

**Definition:** A proposed logical architecture coordinating task Perspective, intelligence composition, evaluation, resources, governance, evidence, and structural evolution.

The term **Universal** denotes an architectural research ambition.

It does not establish universal applicability.

### 10.2 Execution Plane

**Definition:** The functional layer responsible for performing task computation and tool operations.

### 10.3 Scoring and Evaluation Plane

**Definition:** The functional layer responsible for evaluating candidates, outcomes, computational paths, and structural modifications.

### 10.4 Governance and Control Plane

**Definition:** The functional layer responsible for policies, authorization, resource limits, contracts, and promotion decisions.

### 10.5 Control Policy

**Definition:** A rule or mechanism governing permissible decisions and actions.

### 10.6 Dispatch

**Definition:** Selection of a computational component, workflow branch, or execution path.

### 10.7 Resource Allocation

**Definition:** Assignment of computational, temporal, monetary, or other resources to tasks and evaluations.

### 10.8 Authorization

**Definition:** A decision by an appropriate authority or enforcement mechanism that an action is permitted.

**Critical distinction:**

> A high score does not constitute authorization.

### 10.9 Policy Enforcement

**Definition:** Application of mandatory constraints to prevent unauthorized or prohibited operations.

### 10.10 Governance Boundary

**Definition:** A defined limit on the authority of a component, system, or participant.

### 10.11 Control Plane Federation

**Definition:** A proposed arrangement in which multiple Control Planes coordinate across bounded systems without necessarily surrendering local authority.

### 10.12 Sovereign Intelligence

**Definition:** An intelligence architecture in which a bounded unit retains defined control over its context, resources, policies, or actions.

---

## 11. AI Relay and Workflow Control

### 11.1 AI Relay

**Definition:** A workflow in which multiple intelligence components contribute sequentially or collaboratively to a task.

### 11.2 Relay Stage

**Definition:** An individual computational or evaluative step within an AI Relay.

### 11.3 Relay Decision

**Definition:** A decision determining how a Relay proceeds.

Candidate decisions include:

- ACCEPT;
- CONTINUE;
- RETRY;
- DELEGATE;
- ESCALATE;
- STOP.

### 11.4 Adaptive Relay

**Definition:** An AI Relay that changes its computational path according to task conditions, evaluation results, or resource constraints.

### 11.5 Scoring-Controlled Relay

**Definition:** A proposed AI Relay architecture in which structured scoring and a Control Plane guide workflow decisions.

### 11.6 Evaluation Escalation

**Definition:** Invocation of richer, more specialized, or more independent evaluation when existing evidence is insufficient.

### 11.7 Relay Trace

**Definition:** A record of stages, decisions, evaluators, costs, and outcomes associated with a Relay execution.

### 11.8 Relay Structural Learning

**Definition:** Learning reusable workflow or evaluation structures from repeated Relay evidence.

---

## 12. Structural Recursive Self-Improvement

### 12.1 Recursive Self-Improvement (RSI)

**Definition:** A process in which an intelligence system contributes to modifications intended to improve its own future capabilities or performance.

### 12.2 Structural RSI

**Definition:** RSI that modifies the architecture or organization of an intelligence system rather than being limited to model parameters or prompts.

Candidate targets include:

- Localization;
- Intelligence Engines;
- Dispatch structures;
- Scoring Trees;
- CCCs;
- Contracts;
- Control Plane configurations.

### 12.3 Intelligence Architecture Evolution

**Definition:** Modification of the structures used to perform tasks.

### 12.4 Evaluation Architecture Evolution

**Definition:** Modification of the structures used to evaluate tasks and candidate improvements.

### 12.5 Scoring-Guided Structural RSI

**Definition:** A proposed Structural RSI process in which Rich Evaluators, Scoring Forests, Meta-Scoring, independent validation, and governance guide architectural modifications.

### 12.6 Structural Candidate

**Definition:** A proposed modification to an intelligence system's architecture.

### 12.7 Structural Promotion

**Definition:** Acceptance of a validated structural candidate into an active configuration or registry.

### 12.8 Governed Promotion

**Definition:** Structural Promotion requiring explicit validation, authorization, and lifecycle controls.

### 12.9 Sandbox Evaluation

**Definition:** Testing a candidate within an isolated or constrained environment.

### 12.10 Canary Deployment

**Definition:** Limited deployment of a candidate to collect operational evidence before broader promotion.

### 12.11 Rollback

**Definition:** Reverting to a previous validated configuration when a modification proves unsuitable.

### 12.12 Structural Regression

**Definition:** A deterioration in relevant performance, reliability, safety, cost, or other required properties following a structural modification.

### 12.13 Open-Ended Structural Growth

**Definition:** A proposed process in which new structural capabilities, representations, or reusable components can continue to emerge beyond a fixed initial design.

Open-ended growth does not imply unbounded resources, guaranteed progress, or unrestricted action.

---

## 13. Evidence, Counter-Evidence, and Validation

### 13.1 Evidence Repository

**Definition:** A collection of evaluation records, outcomes, traces, versions, and supporting observations.

### 13.2 Counter-Evidence

**Definition:** Evidence that challenges a proposed conclusion, evaluation, or structural improvement.

### 13.3 Independent Validation

**Definition:** Evaluation conducted using references or mechanisms sufficiently separated from the candidate-generation process to provide meaningful external evidence.

### 13.4 Reference Baseline

**Definition:** A stable comparison point against which candidate changes are assessed.

### 13.5 Held-Out Evaluation

**Definition:** Evaluation using data or tasks excluded from the candidate's development or optimization process.

### 13.6 Distribution Shift

**Definition:** A change between the conditions under which a mechanism was developed or evaluated and those under which it is subsequently used.

### 13.7 Long-Tail Evaluation

**Definition:** Evaluation of rare, difficult, or high-impact cases that may be obscured by aggregate performance metrics.

### 13.8 Goodhart's Law

**Definition:** The general problem that optimization pressure can weaken the relationship between a proxy metric and the objective it is intended to represent.

### 13.9 Anti-Goodhart Mechanism

**Definition:** A mechanism intended to reduce metric exploitation or misleading optimization.

Examples include:

- Independent validation;
- Counter-evidence;
- Multiple evaluation dimensions;
- Held-out tasks;
- External outcome measurements.

No single mechanism guarantees elimination of Goodhart-related failures.

### 13.10 Decision Preservation

**Definition:** Preservation of specified decision behavior when a scoring or control structure is transformed.

Decision Preservation may be evaluated:

- Exactly;
- Approximately;
- Within a defined domain;
- Under specified risk constraints.

### 13.11 Behavioral Equivalence

**Definition:** Two systems produce equivalent behavior under a defined set of conditions.

Behavioral Equivalence must be defined relative to a specified observation model and domain.

### 13.12 Structural Similarity

**Definition:** Similarity in organization, relationships, or representations.

Structural Similarity does not automatically imply Behavioral Equivalence.

---

## 14. Specifications, Contracts, and Lifecycle

### 14.1 Specification

**Definition:** An explicit description of intended behavior, interfaces, constraints, or evaluation requirements.

### 14.2 Contract

**Definition:** A formal or structured declaration of obligations, assumptions, interfaces, and compatibility requirements.

### 14.3 Specifications/Contracts First

**Definition:** An engineering principle requiring essential interfaces, semantics, constraints, and conformance criteria to be established before unrestricted runtime composition.

### 14.4 Conformance

**Definition:** Satisfaction of specified interface, behavioral, or governance requirements.

### 14.5 Contract Registry

**Definition:** A managed collection of component contracts and version information.

### 14.6 Capability Registry

**Definition:** A collection of declared or validated component capabilities.

### 14.7 Versioned Evaluation

**Definition:** Evaluation that records the versions of candidates, evaluators, benchmarks, contracts, and relevant policies.

### 14.8 Lifecycle Management

**Definition:** Processes for introducing, validating, promoting, monitoring, specializing, retiring, and rolling back components.

---

## 15. Open-Ended and Collective Intelligence

### 15.1 Open-Ended Scoring Intelligence

**Definition:** A proposed process in which evaluation structures can continue to generate, learn, refine, and reuse new scoring capabilities.

### 15.2 Collective Scoring Intelligence

**Definition:** A proposed arrangement in which scoring structures, evaluation evidence, and validated improvements can be exchanged or learned across multiple participants or systems.

### 15.3 Portable Intelligence

**Definition:** Intelligence representations or components designed for transfer and reuse across compatible environments.

### 15.4 Structural Knowledge Transfer

**Definition:** Transfer of reusable structural patterns, contracts, or validated behaviors between systems.

### 15.5 Structural Learning Loop

**Definition:** A recurring process involving execution, evidence collection, evaluation, structural revision, validation, and governed promotion.

### 15.6 Open-Ended Growth Versus Uncontrolled Growth

**Definition:** Open-ended growth concerns the potential to discover new structures; uncontrolled growth concerns modification without adequate constraints or governance.

These concepts should not be conflated.

---

## 16. Critical Conceptual Distinctions

The following distinctions are especially important for interpreting UCPSF.

| Concept A | Concept B | Essential Difference |
|---|---|---|
| Scoring Function | Scoring Intelligence | Computing a score versus managing and improving evaluation |
| Primitive Scoring | Rich Evaluation | Fixed limited criteria versus broader relevant evaluation |
| Scoring Tree | Scoring Forest | One structured evaluator versus multiple evaluation structures |
| Structural Similarity | Behavioral Equivalence | Similar organization versus equivalent defined behavior |
| Folding | Lossless Compression | Folding may preserve only specified properties |
| CCC | Universal Truth | Reusable abstraction versus unrestricted applicability |
| Meta-Scoring | Self-Certification | Evaluating evaluators versus allowing circular proof of superiority |
| Perspective | Authorization | Evaluation priorities versus permission to act |
| Localization | Per-Node Intelligence | Context selection versus computation using context |
| Integrated Model | Modular Hybrid | Tight coupling versus selectable component composition |
| Intelligence Evolution | Evaluator Evolution | Improving task execution versus improving evaluation |
| Candidate Improvement | Validated Improvement | Proposed benefit versus independently supported benefit |
| Structural Growth | Structural Complexity | Useful new capability versus more components |
| Open-Ended Growth | Unrestricted Action | Expandable structures versus unconstrained authority |

---

## 17. Canonical Research Principles

The UCPSF framework adopts the following proposed principles.

### Principle 1 — Evaluation Is an Intelligence Problem

Evaluation may require structured reasoning, adaptation, and learning rather than only fixed metrics.

### Principle 2 — Structure Should Preserve Meaningful Differences

Structural Folding should not remove decision-relevant or risk-sensitive distinctions merely to achieve compression.

### Principle 3 — Perspective Must Be Explicit

Evaluation and optimization should identify the goals, constraints, budget, time horizon, and risk assumptions under which decisions are made.

### Principle 4 — Evaluators Require Independent Evidence

An evaluator should not establish its own validity solely through internal scoring.

### Principle 5 — Hybridization Must Be Justified

More complex compositions should be adopted only when validated benefits justify their costs.

### Principle 6 — Contracts Precede Unrestricted Composition

Component compatibility, identity, and constraints should be explicit before deployment.

### Principle 7 — Governance Is Distinct from Scoring

Evaluation may recommend an action, but authorization must remain an independent control responsibility.

### Principle 8 — Structural Promotion Requires Validation

Proposed improvements should be tested against appropriate references, including counter-evidence and long-tail cases.

### Principle 9 — Recursive Evolution Must Be Bounded and Reversible Where Feasible

Structural RSI should operate within explicit resource, authority, and lifecycle constraints.

### Principle 10 — Open-Ended Intelligence Requires Governed Growth

The ability to generate new structures should be accompanied by mechanisms for evaluation, compatibility, evidence, and control.

---

## 18. Notation Reference

| Symbol | Meaning |
|---|---|
| $X$ | Input or task |
| $Y$ | Output or result |
| $P$ | Perspective |
| $G$ | Goals or governance rules, depending on context |
| $C$ | Context, constraints, or contracts, depending on context |
| $B$ | Resource budget |
| $T$ | Time horizon or trace, depending on context |
| $R$ | Risk preferences or structural revision |
| $E$ | Evidence |
| $S$ | Score or scoring mechanism |
| $U$ | Utility or uncertainty, depending on context |
| $L_i$ | Localization Engine |
| $I_j$ | Per-Node Intelligence Engine |
| $T_S$ | Scoring Tree |
| $\mathcal{F}_S$ | Scoring Forest |
| $K$ | Common Concept Core |
| $\Delta$ | Specialized Delta |
| $\Theta$ | Structural configuration parameters |
| $A$ | Candidate action or architecture |
| $M$ | Meta-Scoring mechanism |

**Notation caution:** Some symbols are overloaded across conceptual documents. Formal specifications should introduce context-specific namespaces or explicit type declarations to avoid ambiguity.

---

## 19. Research Status and Terminology Policy

UCPSF introduces several proposed architectural concepts.

These terms should be interpreted as research constructs unless supported by formal definitions and empirical evidence.

### Established or Broadly Used Concepts

Examples include:

- Evaluation metrics;
- Calibration;
- Transformer architectures;
- Retrieval;
- Multi-objective optimization;
- Distribution shift;
- Independent validation;
- Recursive Self-Improvement.

### Proposed UCPSF Concepts or Specialized Uses

Examples include:

- Generalized Scoring Intelligence;
- Three Universal Scoring Operator families;
- Scoring Forest Folding;
- Unaligned AND Folding;
- Recursive Scoring CCC Distillation;
- Dual-Hybrid Intelligence;
- Universal Control Plane for Structural Intelligence;
- Scoring-Guided Structural RSI.

### Terminology Evolution

Future versions may refine definitions as:

- Formal models are developed;
- Implementations are tested;
- Counterexamples are discovered;
- Evaluation results become available;
- Interoperability requirements are clarified.

Such revisions should be documented through versioned specifications and the repository changelog.

---

## 20. Related Documents

For the full architecture:

[README.md](README.md)

For guided reading:

[START-HERE.md](START-HERE.md)

For the complete research index:

[CONTENTS.md](CONTENTS.md)

For figure navigation:

[FIGURE-INDEX.md](FIGURE-INDEX.md)

For unresolved questions:

[OPEN-QUESTIONS.md](OPEN-QUESTIONS.md)

For future research directions:

[FUTURE-DIRECTIONS.md](FUTURE-DIRECTIONS.md)

For the core research papers:

[UCPSF-001 through UCPSF-008](CONTENTS.md#3-core-research-papers)

For conceptual case studies:

[CASE-001 through CASE-003](CONTENTS.md#4-case-studies)

---

## 21. Final Perspective

UCPSF proposes that future intelligence systems may benefit from treating evaluation, computation, and governance as interacting but distinguishable structural capabilities.

The long-term research progression is:

**Scoring Functions → Scoring Intelligence → Scoring Trees and Forests → CCC Distillation → Meta-Scoring → Hybrid Intelligence → Universal Control Plane → Governed Structural RSI → Open-Ended Structural Learning**

The defining research challenge is to determine whether these mechanisms can produce measurable, transferable, and governable improvements.

> **The ability to evaluate intelligence may itself become an important object of intelligence research and structural evolution.**

---

## Citation

Tan, S., & GPT-Obot. (2026). *Universal Control Planes and Scoring Tree/Forest/Folding for Structural Intelligence (UCPSF)* (Version 1.0.0).

Repository:

https://github.com/sizhet/Universal-Control-Planes-and-Scoring-Folding

DOI: 10.5281/zenodo.23486273

---

## License

Copyright © 2026 Sizhe Tan & GPT-Obot.

Licensed under the Apache License, Version 2.0.

See [LICENSE.txt](LICENSE.txt).

---

**GLOSSARY — UCPSF Canonical Terminology**  
**Sizhe Tan & GPT-Obot | October 2026 | Version 1.0.0**
