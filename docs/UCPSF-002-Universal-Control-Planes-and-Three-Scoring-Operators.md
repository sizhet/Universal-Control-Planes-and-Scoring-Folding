
# UCPSF-002 — Universal Control Planes and Three Scoring Operators

**Subtitle:** Value-Based Folding, Branching-Based Folding, and ANN Scoring Nodes as Composable Foundations for Structural Intelligence

**Authors:** Sizhe Tan & GPT-Obot  
**Project:** Universal Control Planes and Scoring Tree/Forest/Folding for Structural Intelligence (UCPSF)  
**Document ID:** UCPSF-002  
**Version:** 1.0.0  
**Date:** October 19, 2026  
**Status:** Research Framework and Algorithmic Architecture  
**License:** Apache-2.0

---

## Abstract

Complex artificial intelligence systems increasingly rely on multiple evaluators, candidate branches, learned scoring models, and policy-controlled decisions.

AI Relay, multi-agent coordination, automated engineering, and Structural Recursive Self-Improvement (RSI) all require mechanisms for evaluating alternatives, allocating computation, selecting branches, and deciding whether to continue, stop, merge, or delegate.

Despite differences among these applications, many scoring and control mechanisms exhibit recurring computational patterns.

This paper proposes three candidate families of reusable scoring and folding operators:

1. **Value-Based Folding:** Optimization and consolidation of scoring values, parameters, thresholds, and weights.
2. **Branching-Based Folding:** Selection, pruning, merging, and composition of alternative scoring or decision branches.
3. **ANN Scoring Nodes:** Learned scoring functions that approximate complex evaluation relationships for efficient inference.

We introduce a common operator contract, distinguish scoring from action authorization, and develop an initial compositional algebra for constructing Scoring Trees, Scoring Forests, and Universal Control Planes.

The framework emphasizes perspective-aware evaluation, computational efficiency, explicit constraints, auditability, and evidence-driven structural evolution.

The central hypothesis is that a relatively small collection of reusable operator families can support a substantial portion of the evaluation and control requirements of early- and intermediate-stage AI Relay and Structural RSI systems.

The three families are proposed as a practical starting point, not as a proven exhaustive basis for all intelligent control mechanisms.

**Keywords:** Universal Control Plane, Scoring Operators, Value-Based Folding, Branching-Based Folding, ANN Scoring Node, Structural Intelligence, Scoring Tree, Scoring Forest, Perspective Optimization, Structural RSI, AI Relay, Compositional Intelligence

---

![Fig-002 — Three Universal Scoring Operators](../figures/Fig-002-Three-Universal-Scoring-Operators.png)

**Fig-002.** Three proposed Scoring Operator families and their roles in generalized evaluation.

---

## 1. Introduction

### 1.1 From Generalized Scoring Intelligence to Executable Operators

UCPSF-001 introduced Generalized Scoring Intelligence as a research direction.

Its central argument was that evaluation should not remain merely an auxiliary function attached to an intelligence engine.

Instead, scoring mechanisms should become explicit, composable, transferable, and structurally improvable.

This paper advances that argument from conceptual foundations toward algorithmic construction.

The immediate question is:

**What reusable computational primitives are sufficient to construct useful Scoring Trees and Control Planes?**

A universal architecture cannot begin by implementing every possible scoring mechanism independently.

It needs a manageable collection of operators with clear contracts and composition rules.

### 1.2 Recurrent Patterns in Complex AI Systems

Consider several examples.

An AI coding agent may adjust quality thresholds, compare candidate implementations, and invoke a learned evaluator.

A multi-agent relay may rank alternative agent outputs, merge compatible branches, and terminate low-value paths.

A Structural RSI system may compare proposed architectural modifications, estimate improvement confidence, and reject candidates that violate governance constraints.

Although these systems differ substantially, their control processes often include three recurring forms of computation:

- Adjustment of evaluation values;
- Structural selection or combination of branches;
- Learned approximation of evaluation functions.

These motivate the three operator families proposed here.

### 1.3 Research Scope

This paper focuses on the structural and algorithmic foundations of these operators.

It does not claim:

- That the three families form a mathematically complete operator basis;
- That every AI control problem can be reduced to scalar scoring;
- That Folding always improves decision quality;
- That learned scorers are universally preferable to explicit metrics;
- That the proposed architecture has already demonstrated superior performance.

These are matters for subsequent formalization and empirical validation.

---

## 2. Universal Control Plane: Functional Definition

### 2.1 Scoring and Control Are Distinct

A scoring mechanism estimates or measures the quality of a candidate.

A control mechanism uses evaluation results and applicable policies to determine subsequent operations.

We distinguish:

**Evaluation Plane**

Produces metrics, comparisons, predictions, confidence estimates, and evidence.

**Decision Plane**

Selects candidates, branches, resources, and execution strategies.

**Governance Plane**

Enforces authorization, safety constraints, resource limits, and audit requirements.

These functions may be implemented within one system, but they should remain conceptually distinct.

### 2.2 Universal Control Plane

We define a Universal Control Plane (UCP) as a proposed architectural framework for coordinating heterogeneous scoring, decision, and governance mechanisms across intelligence systems.

A UCP may support:

1. Candidate evaluation;
2. Perspective selection;
3. Scoring Tree dispatch;
4. Branch selection and merging;
5. Resource-budget allocation;
6. Learned scorer invocation;
7. Decision confidence assessment;
8. Evidence collection;
9. Structural improvement;
10. Policy-constrained action selection.

The term *universal* expresses an architectural research objective rather than a claim of demonstrated universal applicability.

### 2.3 Control Plane as a Structured Decision Process

A simplified control cycle is:

```text
Task / Candidate / Context
          |
          v
Perspective and Policy Selection
          |
          v
Scoring Operator Dispatch
          |
          v
Scoring Tree / Forest Evaluation
          |
          v
Evidence and Constraint Validation
          |
          v
Decision / Continue / Merge / Delegate / Stop
          |
          v
Execution Feedback
          |
          v
Structural Learning and Scoring Update
```

The control process may be recursive.

A decision may trigger additional scoring, invoke a different intelligence engine, or modify the candidate evaluation structure.

---

## 3. Three Candidate Operator Families

### 3.1 Overview

We propose three primary operator families.

| Family | Primary Object | Main Operations | Typical Application |
|---|---|---|---|
| Value-Based Folding | Values and parameters | Adjust, aggregate, calibrate, compress | Thresholds, weights, metric configuration |
| Branching-Based Folding | Candidate branches | Select, prune, merge, compose | Relay paths, candidate plans, structural search |
| ANN Scoring Node | Learned evaluation function | Train, infer, calibrate, distill | Fast candidate scoring, quality prediction |

These families operate at different structural levels.

Value-Based Folding primarily modifies numerical or symbolic evaluation parameters.

Branching-Based Folding modifies alternative paths or candidate structures.

ANN Scoring Nodes provide learned evaluation functions that can be embedded inside either family.

### 3.2 Complementarity Rather Than Exclusivity

The families are not mutually exclusive.

For example:

1. An ANN Scoring Node predicts the quality of candidate branches.
2. A Value-Based operator adjusts the decision threshold.
3. A Branching-Based operator selects the surviving candidates.
4. A governance mechanism checks whether the selected action is permitted.

The combined mechanism can form a reusable Scoring Tree.

### 3.3 Why Start with Three Families?

The proposed classification emphasizes practical engineering coverage.

Many early- and intermediate-stage Relay and RSI systems rely heavily on:

- Parameter optimization;
- Candidate comparison;
- Branch selection;
- Learned quality estimation.

These mechanisms provide a tractable starting point for structural research.

However, formal verification, constrained optimization, scheduling, symbolic inference, and other mechanisms may require additional operator families or independent control components.

---

## 4. Operator A — Value-Based Folding

### 4.1 Definition

Value-Based Folding operates on values, parameters, weights, thresholds, or configurations associated with an evaluation mechanism.

Let:

$$
\theta = (\theta_1,\theta_2,\ldots,\theta_n)
$$

represent a parameter vector.

A scoring function may be written as:

$$
S(x \mid \theta,P)
$$

where $P$ is the evaluation perspective.

The objective is to identify a parameter configuration that improves decision quality under applicable constraints.

### 4.2 Basic Optimization

A simple formulation is:

$$
\theta^*
=
\arg\max_{\theta \in \Theta}
J(\theta \mid P,E)
$$

where:

- $\Theta$: Admissible parameter space;
- $J$: Evaluation objective;
- $P$: Perspective;
- $E$: Validation evidence.

The objective may account for quality, calibration, cost, robustness, and other criteria.

### 4.3 Value Folding

Optimization and Folding are related but not identical.

Optimization changes values to improve an objective.

Value Folding additionally attempts to consolidate or simplify value configurations while preserving relevant decision behavior.

Examples include:

- Merging nearly equivalent weight configurations;
- Replacing redundant thresholds with a shared parameter;
- Compressing repeated scoring profiles;
- Extracting a common parameter pattern from multiple evaluators.

### 4.4 Example: Relay Confidence Threshold

Suppose an AI Relay system delegates a task when confidence falls below a threshold:

$$
operatorname{Delegate}(x) =
\mathbb{1}[c(x)<\tau]
$$

where:

- $c(x)$: Confidence estimate;
- $\tau$: Delegation threshold.

The threshold may be optimized according to:

- Error cost;
- Delegation cost;
- Latency;
- Task difficulty;
- Risk tolerance.

A Perspective-aware threshold becomes:

$$
\tau = \tau(P)
$$

Different task perspectives may require different delegation policies.

### 4.5 Value-Based Folding Operators

Candidate operators include:

**V-ADJUST**

Modify a parameter according to evaluation feedback.

**V-CALIBRATE**

Align score or confidence estimates with observed outcomes.

**V-AGGREGATE**

Combine compatible scoring values.

**V-NORMALIZE**

Transform scores into a specified comparable representation.

**V-FOLD**

Consolidate redundant value configurations.

**V-SPECIALIZE**

Create perspective-specific parameter variants.

### 4.6 Limitations

Value-Based Folding may fail when:

- The scoring structure is fundamentally incorrect;
- Important evaluation dimensions are missing;
- Parameters have incompatible semantics;
- The optimization objective is misspecified;
- Hard constraints are incorrectly converted into soft penalties.

Value optimization cannot compensate for every structural deficiency.

---

## 5. Operator B — Branching-Based Folding

### 5.1 Definition

Branching-Based Folding operates on sets of candidate branches or structural alternatives.

Let:

$$
B = \{b_1,b_2,\ldots,b_N\}
$$

represent a candidate branch set.

The system may evaluate, select, prune, merge, or compose branches.

### 5.2 Branch Selection

A basic selection mechanism is:

$$
b^*
=
\arg\max_{b_i \in B}
S(b_i\mid P)
$$

This represents winner selection under a given scoring function.

However, complex systems may require more than selecting one branch.

### 5.3 N-to-K Folding

A central candidate operator is:

$$
F_{N\rightarrow K}(B,P,E)
$$

where:

$$
1 \le K < N
$$

The operator transforms $N$ candidate branches into $K$ retained or consolidated branches.

The transformation may involve:

- Ranking;
- Pruning;
- Clustering;
- Merging;
- Structural composition;
- Consensus extraction;
- Diversity preservation.

The objective is not necessarily to preserve the top $K$ scalar scores.

It may instead preserve a useful collection of complementary alternatives.

### 5.4 Confidence Through Branch Combination

Multiple branches may provide independent or partially independent evidence.

For example, several candidate implementations may agree on a design principle while differing in implementation details.

A Folding operator may extract their common structure.

However, agreement does not automatically imply increased confidence.

If the branches share the same underlying error or training bias, their agreement may be misleading.

Branch correlation and evidence independence must therefore be considered.

### 5.5 Example: Multi-Agent Relay

Consider an AI Relay system with four candidate outputs:

```text
Agent A ----\
             \
Agent B ------> Branch Scoring ---> Folding ---> Selected Structure
             /
Agent C ----/
            \
Agent D -----/
```

Possible operations include:

1. Rejecting invalid branches;
2. Ranking valid candidates;
3. Extracting common structural elements;
4. Preserving complementary differences;
5. Delegating unresolved conflicts to another evaluator.

The output may be one branch, several branches, or a newly composed structure.

### 5.6 Branching Operators

Candidate operators include:

**B-SELECT**

Choose a branch according to evaluation criteria.

**B-PRUNE**

Remove branches that are dominated, invalid, or insufficiently promising.

**B-MERGE**

Combine compatible branch structures.

**B-FOLD**

Extract a consolidated representation from multiple branches.

**B-SPLIT**

Separate a branch into specialized alternatives.

**B-DELEGATE**

Route unresolved alternatives to another evaluator or intelligence engine.

**B-PRESERVE**

Retain structurally diverse branches when uncertainty remains significant.

### 5.7 Decision Preservation

A Folding operation should be evaluated against the decision information it preserves.

Possible measures include:

- Utility retention;
- Coverage of relevant alternatives;
- Constraint satisfaction;
- Diversity retention;
- Robustness;
- Counter-evidence sensitivity.

Aggressive pruning may reduce cost but eliminate valuable long-tail alternatives.

---

## 6. Operator C — ANN Scoring Node

### 6.1 Definition

An ANN Scoring Node uses a trained model to estimate an evaluation quantity.

Let:

$$
S_{\phi}(x,P)
$$

represent a learned scoring function parameterized by $\phi$.

The model may estimate:

- Candidate quality;
- Expected improvement;
- Failure probability;
- Semantic similarity;
- Confidence;
- Cost;
- Ranking preference.

### 6.2 Why ANN Scoring?

Some evaluation relationships are too complex for simple explicit formulas.

A learned scorer can approximate these relationships from examples.

Once trained, it may provide efficient inference relative to more expensive evaluation procedures.

This can be particularly useful when the same evaluation task is repeated many times.

### 6.3 Training and Inference Separation

ANN Scoring naturally supports two computational phases.

**Offline or Periodic Training**

Learn an approximation from collected evaluation evidence.

**Online Scoring**

Apply the learned model to new candidates.

The intended advantage is to shift some expensive evaluation work away from repeated online decision-making.

However, inference cost, training cost, calibration, and distribution shift must be included in any efficiency comparison.

### 6.4 ANN Scoring as Structural Distillation

Suppose an expensive Scoring Forest produces reference evaluations:

$$
S_{\mathcal{F}}(x,P)
$$

A learned scorer may be trained to approximate:

$$
S_{\phi}(x,P)
\approx
S_{\mathcal{F}}(x,P)
$$

This creates a possible distillation path:

```text
Rich Scoring Forest
        |
        v
Reference Evaluations
        |
        v
Training Dataset
        |
        v
ANN Scoring Node
        |
        v
Fast Online Evaluation
```

The learned scorer should retain a route back to richer evaluation when uncertainty, novelty, or risk is high.

### 6.5 JEV-Like Scoring Hypothesis

A relevant architectural hypothesis is that some scoring tasks may be decomposed into learned representations, weights, and reference-conditioned scoring operations.

A generic form is:

$$
S(x,r)
=
f_{\phi}(x)^\top W g_{\psi}(r)
+
b(x,r)
$$

where:

- $x$: Candidate representation;
- $r$: Reference or target representation;
- $f_{\phi}$: Candidate encoder;
- $g_{\psi}$: Reference encoder;
- $W$: Learned scoring matrix;
- $b$: Optional baseline or correction term.

This formulation illustrates how learned representations and matrix operations may support efficient scoring.

It is not a verified description of any particular external system.

### 6.6 ANN Scoring Operators

Candidate operations include:

**A-TRAIN**

Train a scoring model from evaluation evidence.

**A-INFER**

Produce learned evaluation estimates.

**A-CALIBRATE**

Calibrate predictions against observed outcomes.

**A-DISTILL**

Approximate a richer evaluation process.

**A-DETECT-SHIFT**

Identify possible changes in input or evaluation distributions.

**A-ESCALATE**

Invoke a richer evaluator when learned scoring is insufficiently reliable.

### 6.7 Limitations

ANN Scoring Nodes may suffer from:

- Distribution shift;
- Poor calibration;
- Hidden bias;
- Reward misspecification;
- Training-data contamination;
- Reduced interpretability;
- Overconfidence on unfamiliar inputs.

They should therefore operate within explicit applicability and governance boundaries.

---

## 7. A Unified Scoring Operator Contract

### 7.1 Motivation

To compose heterogeneous operators, UCPSF requires a shared structural interface.

The interface must preserve enough information for downstream evaluation and control.

### 7.2 Proposed Contract

We propose:

$$
O:(X,P,E,C)\rightarrow(Y,S,U,T)
$$

where:

**Inputs**

- $X$: Candidate values, branches, or structures;
- $P$: Evaluation perspective;
- $E$: Available evidence;
- $C$: Operator contract and constraints.

**Outputs**

- $Y$: Resulting values or structures;
- $S$: Scoring information;
- $U$: Uncertainty and applicability information;
- $T$: Execution trace and audit evidence.

Not every operator must produce a scalar score.

Some may return rankings, feasible sets, distributions, or structured evaluation records.

### 7.3 Minimum Contract Fields

A practical operator contract should specify:

```text
Operator Identity
Operator Family
Input Schema
Output Schema
Perspective Requirements
Score Semantics
Uncertainty Representation
Applicability Conditions
Resource Requirements
Policy Constraints
Evidence Requirements
Trace / Audit Format
Version
```

### 7.4 Compatibility

Two operators should be composable only when their interfaces and semantic requirements are compatible.

For example, an ANN-generated probability should not be treated as an arbitrary utility score without an explicit conversion or calibration contract.

Likewise, an operator expecting a normalized score should not silently consume an unbounded distance value.

### 7.5 Contract-First Principle

The UCPSF architecture adopts the following engineering principle:

**Specifications and contracts should be established before runtime composition.**

This supports reliable Relay, structural reuse, and auditability.

---

## 8. Toward a Compositional Scoring Operator Algebra

### 8.1 Operator Composition

Let $O_1$ and $O_2$ represent compatible scoring operators.

Their sequential composition is:

$$
O_2 \circ O_1
$$

provided that the output contract of $O_1$ satisfies the input requirements of $O_2$.

### 8.2 Sequential Composition

Example:

```text
ANN Scoring
     |
     v
Value Calibration
     |
     v
Branch Selection
```

The ANN produces candidate evaluations.

The Value operator calibrates the scores.

The Branching operator selects candidates.

### 8.3 Parallel Composition

Multiple operators may evaluate the same candidate under different perspectives.

```text
                +--> Technical Scorer --+
                |                      |
Candidate ------+--> Economic Scorer ---+--> Aggregation
                |                      |
                +--> Risk Scorer -------+
```

The aggregation mechanism must account for score semantics and applicable constraints.

### 8.4 Conditional Composition

An operator may be invoked only when a condition is satisfied.

For example:

```text
Cheap Local Scoring
        |
        v
Confidence Sufficient?
      /     \
    Yes      No
     |        |
  Decide   Rich Scoring Forest
```

This supports cost-aware evaluation.

### 8.5 Recursive Composition

A Scoring Tree may invoke another Scoring Tree.

A Control Plane may also evaluate whether to modify its own scoring structure.

Such recursion requires explicit termination conditions, resource budgets, and governance constraints.

### 8.6 Algebraic Research Questions

A formal operator algebra must investigate:

- Type compatibility;
- Associativity under specified conditions;
- Identity operators;
- Equivalence;
- Commutativity where applicable;
- Information preservation;
- Error propagation;
- Constraint preservation.

These properties cannot be assumed universally.

For example, branch pruning followed by merging may produce a different result from merging followed by pruning.

---

## 9. Constructing Scoring Trees from Operators

### 9.1 Scoring Node

A Scoring Node contains:

1. An operator;
2. Input and output contracts;
3. Perspective information;
4. Evaluation evidence;
5. Control metadata.

### 9.2 Scoring Tree

A Scoring Tree organizes scoring nodes through dependency relationships.

A simplified representation is:

$$
T_S = (V,E,O,P,C)
$$

where:

- $V$: Nodes;
- $E$: Edges;
- $O$: Assigned operators;
- $P$: Perspective metadata;
- $C$: Contracts and constraints.

### 9.3 Example Tree

```text
                  Final Decision
                        |
                 Branching Operator
                        |
          +-------------+-------------+
          |             |             |
     Technical       Economic       Risk
       Scoring        Scoring       Scoring
          |             |             |
      ANN Node      Value Node    Rule / ANN
          |             |             |
       Evidence      Evidence      Evidence
```

The example illustrates how learned and explicit scoring mechanisms can coexist.

### 9.4 From Trees to Forests

Multiple Scoring Trees may be organized into a forest.

The forest may contain different:

- Domain evaluators;
- Perspective-specific evaluators;
- Temporal evaluators;
- Risk evaluators;
- Structural improvement evaluators.

A forest-level controller determines which trees to invoke and how their results should influence decisions.

---

## 10. Scoring Folding at Three Levels

### 10.1 Value-Level Folding

Consolidates redundant or related scoring parameters.

Example:

Multiple task-specific thresholds may be represented by a shared function conditioned on perspective.

### 10.2 Branch-Level Folding

Consolidates candidate branches while preserving useful alternatives.

Example:

Several candidate plans may share a common execution structure with different specialized branches.

### 10.3 Model-Level Distillation

A learned scorer may approximate a more complex evaluation process.

Example:

A rich Scoring Forest may provide training labels for a lower-cost ANN Scoring Node.

### 10.4 Cross-Level Folding

The three mechanisms may be combined.

For example:

1. Branching-Based Folding extracts common candidate structures.
2. Value-Based Folding consolidates their scoring parameters.
3. ANN Distillation learns an efficient approximation of recurring evaluation patterns.

This creates a possible route from complex evaluation structures to compact reusable control mechanisms.

### 10.5 Folding Must Preserve Meaning

Structural compression alone is not sufficient.

A useful Folding process should preserve relevant:

- Decision behavior;
- Constraint satisfaction;
- Evaluation semantics;
- Applicability boundaries;
- Uncertainty;
- Counter-evidence.

The precise preservation requirements depend on the application perspective.

---

## 11. Perspective-Aware Operator Selection

### 11.1 Perspective as an Input

Operator selection should depend on the task perspective.

Let:

$$
P = (G,C,B,T,R)
$$

represent goals, context, budget, time horizon, and risk preferences.

### 11.2 Operator Selection

A Control Plane may choose an operator configuration:

$$
O^*
=
\arg\max_{O \in \mathcal{O}_{valid}}
J(O\mid P,E)
$$

where $\mathcal{O}_{valid}$ contains contract-compatible and policy-permitted operators.

### 11.3 Cost-Aware Evaluation

The objective may include:

$$
J(O\mid P,E)
=
\mathbb{E}[U(O\mid P,E)]
-
\lambda C(O)
$$

where $C(O)$ represents expected evaluation cost.

### 11.4 Adaptive Scoring Depth

A low-risk task may require only a cheap ANN scorer.

A high-risk task may require:

- Independent evaluators;
- Richer Scoring Trees;
- Constraint verification;
- Counter-evidence;
- Human authorization.

This produces an adaptive evaluation architecture rather than a fixed-depth scoring pipeline.

---

## 12. Universal Control Plane Runtime Skeleton

### 12.1 Functional Components

A candidate UCP runtime may contain:

```text
Universal Control Plane
│
├── Perspective Manager
│
├── Policy / Contract Manager
│
├── Scoring Operator Registry
│   ├── Value Operators
│   ├── Branching Operators
│   └── ANN Scoring Operators
│
├── Scoring Tree / Forest Manager
│
├── Operator Dispatch
│
├── Evidence and Calibration Manager
│
├── Folding / Distillation Manager
│
├── Decision and Resource Controller
│
└── Trace / Audit / Validation
```

### 12.2 Perspective Manager

Determines the active evaluation context and relevant objectives.

### 12.3 Operator Registry

Maintains operator identities, capabilities, contracts, and applicability information.

### 12.4 Scoring Tree / Forest Manager

Constructs and selects evaluation structures.

### 12.5 Folding / Distillation Manager

Supports structural consolidation and learned approximation.

### 12.6 Evidence Manager

Collects evaluation outcomes and counter-evidence.

### 12.7 Decision Controller

Selects subsequent operations under applicable policies.

### 12.8 Governance Boundary

The Control Plane must not treat scoring success as sufficient authorization for external action.

Action permission remains subject to independent policy constraints.

---

## 13. Application to AI Relay

### 13.1 Relay Control Requirements

AI Relay systems may contain multiple stages, specialized agents, and alternative execution paths.

They require decisions about:

- Task routing;
- Candidate selection;
- Delegation;
- Merge operations;
- Termination;
- Resource allocation.

### 13.2 Operator Mapping

**Value-Based Folding**

Adjusts thresholds, weights, and relay-specific evaluation parameters.

**Branching-Based Folding**

Selects and consolidates candidate relay paths.

**ANN Scoring Nodes**

Provide fast quality estimates for repeated decisions.

### 13.3 Example Relay Process

```text
Task Input
    |
    v
Localization
    |
    v
Candidate Agent / Engine Selection
    |
    v
ANN Scoring
    |
    v
Value-Based Calibration
    |
    v
Branching-Based Selection
    |
    v
Relay / Merge / Stop
    |
    v
Evidence Collection
```

The same operator families may be reused across different relay stages.

---

## 14. Application to Structural RSI

### 14.1 RSI Evaluation Requirements

Structural RSI evaluates proposed changes to an intelligence system.

Potential modifications include:

- New branches;
- New scoring nodes;
- New localization structures;
- Alternative intelligence engines;
- Updated control policies;
- Revised evaluation criteria.

### 14.2 Rich Evaluators

A structural modification should not be judged solely by a single performance metric.

Relevant criteria may include:

- Task performance;
- Computational cost;
- Robustness;
- Transferability;
- Structural complexity;
- Safety;
- Governance compliance.

### 14.3 Operator Roles

Value-Based Folding optimizes parameters of candidate structures.

Branching-Based Folding selects or merges candidate structural modifications.

ANN Scoring Nodes estimate improvement potential.

The UCP coordinates these evaluations under explicit constraints.

### 14.4 Independent Validation

A candidate RSI modification should not be promoted merely because its internal scorer predicts improvement.

Promotion should require independent validation against specified objectives and constraints.

### 14.5 Recursive Improvement of Scoring

The scoring structures themselves may become RSI targets.

This creates a meta-level improvement process.

However, modifications to evaluators require stricter validation to avoid self-referential reward manipulation.

---

## 15. Open-Ended Growth and Operator Extensibility

### 15.1 Three Families as a Starting Basis

The proposed operator families are intended to provide a compact initial architecture.

They should not prevent future extensions.

### 15.2 New Operator Families

Possible future additions include:

- Constraint-solving operators;
- Formal verification operators;
- Temporal planning operators;
- Causal evaluation operators;
- Multi-objective Pareto operators;
- Resource scheduling operators.

Some may be expressible as compositions of existing operators.

Others may justify independent operator families.

### 15.3 Plugin-Oriented Evolution

An extensible UCP may allow new operators to register through explicit contracts.

This supports:

- Local experimentation;
- Specialized domains;
- Replacement of obsolete operators;
- Collective learning;
- Portable scoring components.

### 15.4 Relationship to PIRP/PIRU

Portable Intelligence Runtime Pieces and Units provide a potential structural exchange mechanism.

A scoring operator or Scoring Tree may eventually be packaged as a portable intelligence component with explicit identity, interfaces, and validation metadata.

This remains a future integration direction.

---

## 16. Validation Framework

### 16.1 Core Research Hypothesis

A compositional scoring architecture may improve evaluation reuse, adaptability, and efficiency compared with independently engineered scoring mechanisms.

### 16.2 Baselines

Candidate baselines include:

1. Fixed scalar scoring;
2. Weighted multi-criteria scoring;
3. Standalone learned reward models;
4. Fixed branch-selection rules;
5. Non-compositional scoring pipelines.

### 16.3 Experiments

**Experiment A — Value Folding**

Compare fixed thresholds with perspective-conditioned parameter optimization.

**Experiment B — Branch Folding**

Compare winner-take-all selection with N-to-K structural Folding.

**Experiment C — ANN Distillation**

Compare direct rich evaluation with learned scoring approximation and selective escalation.

**Experiment D — Operator Composition**

Compare isolated scoring mechanisms with contract-compatible composed Scoring Trees.

**Experiment E — Cross-Task Reuse**

Evaluate whether reusable operator structures transfer across different AI Relay tasks.

### 16.4 Metrics

| Metric | Purpose |
|---|---|
| Decision Quality | Evaluate downstream task outcomes |
| Decision Preservation | Measure information retained after Folding |
| Calibration | Assess confidence reliability |
| Transferability | Evaluate reuse across tasks |
| Computational Cost | Measure scoring overhead |
| Latency | Measure decision time |
| Robustness | Evaluate sensitivity to distribution shift |
| Constraint Compliance | Verify governance requirements |

### 16.5 Validation Status

The operators and architecture presented here are research proposals.

No experimental superiority is claimed in this document.

---

## 17. Risks and Limitations

### 17.1 Incomplete Operator Coverage

Three operator families may not cover all relevant control mechanisms.

### 17.2 Composition Overhead

A modular architecture may introduce latency and interface complexity.

### 17.3 Score Semantics

Different operators may produce incompatible scores.

### 17.4 Folding Errors

Structural consolidation may remove valuable distinctions.

### 17.5 Learned Scorer Drift

ANN scorers may become unreliable under changing task distributions.

### 17.6 Meta-Evaluation Risks

Recursive modification of scoring mechanisms may produce Goodhart failures.

### 17.7 Governance Complexity

Scoring and policy mechanisms may conflict if their responsibilities are not explicitly separated.

These limitations should guide subsequent formalization and validation.

---

## 18. Research Roadmap

The next stages of UCPSF research are:

**UCPSF-003**

Formalize Scoring Trees, Scoring Forests, and Unaligned AND Folding.

**UCPSF-004**

Develop Common Concept Core extraction and recursive structural distillation.

**UCPSF-005**

Investigate Perspective-aware optimization and Meta-Scoring Intelligence.

**UCPSF-006**

Study Hybrid Localization and Per-Node Intelligence.

**UCPSF-007**

Integrate scoring operators into Universal Control Plane and Structural RSI architectures.

**UCPSF-008**

Explore open-ended scoring intelligence and long-term structural evolution.

---

## 19. Conclusion

This paper proposes three candidate operator families as reusable foundations for Generalized Scoring Intelligence:

1. **Value-Based Folding**, which modifies and consolidates evaluation parameters;
2. **Branching-Based Folding**, which selects and transforms candidate structures;
3. **ANN Scoring Nodes**, which learn approximations of complex evaluation functions.

Their combination provides a practical starting point for constructing Scoring Trees, Scoring Forests, and Universal Control Planes.

The central architectural principle is:

> **Scoring mechanisms should be composable intelligence structures rather than isolated evaluation functions.**

This perspective supports a progression from local scoring toward reusable structural evaluation and controlled evolution.

The proposed operators do not constitute a proven universal basis.

Their value must be established through formal contracts, decision-preservation analysis, cross-domain testing, and empirical comparison.

Nevertheless, they provide a concrete algorithmic foundation for investigating Universal Control Planes in AI Relay, Hybrid Structural Intelligence, and Structural Recursive Self-Improvement.

---

## Suggested Figure Placement

### Fig-002 — Three Universal Scoring Operators

**File:** `../figures/Fig-002-Three-Universal-Scoring-Operators.png`

**Suggested insertion:** After Section 3.3.

**Purpose:** Illustrate the three operator families and their complementary roles in constructing Scoring Trees.

### Fig-001 — Universal Control Plane Grand Map

**File:** `../figures/Fig-001-Universal-Control-Plane-Grand-Map.png`

**Suggested insertion:** After Section 12.8.

**Purpose:** Show how the operator registry, Scoring Forest, Perspective Manager, governance, and structural learning components interact.

---

## Citation

Suggested citation prior to DOI assignment:

Tan, S., & GPT-Obot. (2026). *UCPSF-002: Universal Control Planes and Three Scoring Operators*. Universal Control Planes and Scoring Tree/Forest/Folding for Structural Intelligence, Version 1.0.0.

Repository:

https://github.com/sizhet/Universal-Control-Planes-and-Scoring-Folding

DOI: To be assigned after the initial archived release.

---

## License

Copyright © 2026 Sizhe Tan & GPT-Obot.

Licensed under the Apache License, Version 2.0.

---

**Document:** UCPSF-002  
**Research Series:** Universal Control Planes and Scoring Tree/Forest/Folding  
**Status:** Research Framework and Algorithmic Architecture  
**Version:** 1.0.0
