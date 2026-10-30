
# OPEN QUESTIONS — Universal Control Planes and Scoring Tree/Forest/Folding

**Open Research Problems, Counterexamples, and Falsification Agenda**

**Project:** Universal Control Planes and Scoring Tree/Forest/Folding for Structural Intelligence (UCPSF)  
**Authors:** Sizhe Tan & GPT-Obot  
**Version:** 1.0.0  
**Date:** October 15, 2026  
**Status:** Open Research Questions  
**License:** Apache-2.0

---

## 1. Purpose

This document identifies unresolved theoretical, algorithmic, architectural, experimental, and governance questions within the UCPSF research framework.

UCPSF proposes that evaluation mechanisms can become structurally learnable, transferable, and recursively improvable intelligence structures.

The framework connects:

- Generalized Scoring Intelligence;
- Scoring Trees and Forests;
- Value-Based and Branching-Based Folding;
- ANN Scoring Nodes;
- Unaligned AND Folding;
- Common Concept Core extraction;
- Recursive CCC distillation;
- Perspective-Aware Meta-Scoring;
- Dual-Hybrid Localization and Per-Node Intelligence;
- Universal Control Planes;
- Governed Structural Recursive Self-Improvement.

These concepts form a proposed research architecture.

Their generality, effectiveness, limitations, and compatibility require further investigation.

This document treats unresolved questions and potential counterexamples as essential research assets rather than obstacles to be hidden.

---

## 2. Research Question Classification

Questions are grouped into three priority levels.

| Priority | Meaning |
|---|---|
| **P0 — Foundational** | Must be addressed to establish the validity or coherence of major architectural claims |
| **P1 — Architectural** | Important for practical algorithms, interoperability, and controlled implementation |
| **P2 — Exploratory** | Important for long-term generalization, collective learning, and open-ended evolution |

Each question may include:

- The research problem;
- Why it matters;
- A potential counterexample;
- A proposed validation approach.

A question is not considered resolved merely because a plausible architectural explanation exists.

---

# Part I — Foundations of Scoring Intelligence

## Q-001 — What Makes Scoring an Intelligence Capability?

**Priority:** P0  
**Related:** UCPSF-001, UCPSF-002

### Research Problem

A fixed scoring function evaluates an input according to predefined criteria.

Scoring Intelligence is proposed to include the ability to select, compose, adapt, and improve evaluators.

What minimal capabilities distinguish Scoring Intelligence from conventional evaluation software?

### Critical Questions

- Is evaluator selection sufficient?
- Must the system learn from evidence?
- Must it support structural modification?
- Is Meta-Scoring necessary?
- How should intelligence improvement be measured?

### Potential Counterexample

A conventional rule-based evaluation engine may already support metric selection and composition without requiring a new intelligence category.

### Proposed Validation

Develop operational criteria that distinguish Scoring Intelligence from fixed scoring systems, rule engines, and conventional model selection.

**Required outcome:** A falsifiable functional definition.

---

## Q-002 — Are the Three Scoring Operator Families Sufficient?

**Priority:** P0  
**Related:** UCPSF-002

### Research Problem

UCPSF proposes three Scoring Operator families:

1. Value-Based Folding;
2. Branching-Based Folding;
3. ANN Scoring Nodes.

Do these families provide sufficient expressive coverage for complex evaluation systems?

### Potential Missing Mechanisms

- Symbolic theorem proving;
- Constraint satisfaction;
- Simulation-based evaluation;
- Causal inference;
- Human judgment;
- Probabilistic graphical models;
- Adversarial testing.

### Potential Counterexample

An evaluator based on formal proof obligations may not fit naturally into any of the three proposed families without an overly broad interpretation.

### Proposed Validation

Construct a taxonomy of real evaluation mechanisms and test whether the proposed operator families provide useful, nontrivial coverage.

**Important distinction:** The three families need not be mutually exclusive or exhaustive to be useful.

---

## Q-003 — Can Scoring Operators Be Composed Without Losing Meaning?

**Priority:** P0  
**Related:** UCPSF-002, UCPSF-005

### Research Problem

Different evaluators may produce scores with incompatible semantics.

Examples include:

- Probabilities;
- Similarity measures;
- Ordinal rankings;
- Risk categories;
- Utility estimates;
- Binary constraints.

When is operator composition mathematically and semantically valid?

### Potential Counterexample

Combining a calibrated probability with an uncalibrated similarity score through a weighted sum may produce misleading rankings.

### Proposed Validation

Define typed scoring contracts and composition rules.

Test whether invalid combinations can be detected before execution.

---

## Q-004 — What Is the Correct Representation of Evaluation Uncertainty?

**Priority:** P1  
**Related:** UCPSF-001, UCPSF-002, UCPSF-005

### Research Problem

Evaluation uncertainty may arise from:

- Limited evidence;
- Model approximation;
- Distribution shift;
- Ambiguous goals;
- Measurement noise;
- Unknown failure modes.

Can these uncertainties be represented within a common Scoring Contract?

### Potential Counterexample

A single confidence score may conflate uncertainty about the candidate with uncertainty about the evaluator itself.

### Proposed Validation

Compare scalar uncertainty, interval estimates, probabilistic models, and structured uncertainty records.

---

## Q-005 — When Does Rich Evaluation Become Counterproductive?

**Priority:** P1  
**Related:** UCPSF-001, UCPSF-005, CASE-001

### Research Problem

Adding evaluation dimensions may improve coverage but also increase cost, latency, and complexity.

### Potential Counterexample

A simple deterministic test may outperform a large Scoring Forest for a narrowly specified task.

### Proposed Validation

Measure evaluation benefit relative to total cost across task complexity levels.

Determine conditions under which simpler evaluators should be preferred.

---

# Part II — Scoring Trees, Forests, and Structural Folding

## Q-006 — What Is the Appropriate Formal Model for a Scoring Tree?

**Priority:** P0  
**Related:** UCPSF-003

### Research Problem

Scoring structures may contain:

- Hierarchies;
- Shared substructures;
- Conditional branches;
- Feedback;
- Cross-node dependencies.

Is a tree sufficient, or is a general Scoring Graph required?

### Potential Counterexample

An evaluator with shared intermediate computations may be represented inefficiently as a strict tree.

### Proposed Validation

Compare tree, DAG, and general graph representations on expressiveness, execution cost, and analyzability.

---

## Q-007 — What Constitutes a Scoring Forest?

**Priority:** P1  
**Related:** UCPSF-003

### Research Problem

A Scoring Forest may be a collection of evaluators.

But what relationships distinguish a meaningful forest from an arbitrary set of scoring functions?

### Candidate Relationships

- Shared CCCs;
- Common task families;
- Perspective specialization;
- Structural lineage;
- Transferable evaluation semantics.

### Proposed Validation

Develop explicit membership, identity, and relationship contracts.

---

## Q-008 — Can Unaligned AND Folding Be Formally Defined?

**Priority:** P0  
**Related:** UCPSF-003, UCPSF-004

### Research Problem

Unaligned AND Folding seeks commonality across structures without direct node-to-node alignment.

What exactly is the AND operation?

Possible interpretations include:

- Structural intersection;
- Semantic commonality;
- Behavioral agreement;
- Constraint-preserving abstraction;
- Evidence-supported shared substructure.

### Potential Counterexample

Two structurally unrelated evaluators may agree on a limited dataset while diverging sharply outside that dataset.

### Proposed Validation

Define alternative formalizations and test them against controlled structural and behavioral examples.

**Required outcome:** An explicit matching relation and preservation contract.

---

## Q-009 — Can Folding Preserve Decision-Relevant Behavior?

**Priority:** P0  
**Related:** UCPSF-003, UCPSF-004

### Research Problem

Structural Folding may simplify an evaluator while removing rare but important distinctions.

### Potential Counterexample

A folded risk evaluator preserves average ranking accuracy but loses a low-frequency safety-critical branch.

### Proposed Validation

Measure:

- Exact decision agreement;
- Ranking preservation;
- Boundary-case behavior;
- Long-tail regression;
- Constraint preservation.

A successful Folding method must specify which properties it preserves and under what conditions.

---

## Q-010 — How Should Structural and Behavioral CCCs Be Reconciled?

**Priority:** P0  
**Related:** UCPSF-003, UCPSF-004

### Research Problem

Structural commonality does not necessarily imply behavioral commonality.

Conversely, behaviorally equivalent evaluators may have different structures.

### Potential Counterexample

Two evaluators implement the same decision function through entirely different internal organizations.

### Proposed Validation

Develop paired structural and behavioral equivalence tests.

Investigate whether a CCC should contain both representations or maintain separate linked abstractions.

---

## Q-011 — Is the Aspen Grove Core±Delta Model Computationally Useful?

**Priority:** P1  
**Related:** UCPSF-003, UCPSF-008

### Research Problem

The Aspen Grove analogy suggests shared roots and specialized branches.

Can this be translated into an efficient computational representation?

### Potential Counterexample

The cost of managing shared CCCs and Specialized Deltas may exceed the benefit of maintaining independent Scoring Trees.

### Proposed Validation

Compare shared-core and independent-tree representations on:

- Storage;
- Evaluation cost;
- Update complexity;
- Decision preservation;
- Transferability.

---

# Part III — CCC Extraction and Recursive Distillation

## Q-012 — What Is the Minimum Valid CCC?

**Priority:** P0  
**Related:** UCPSF-004

### Research Problem

A CCC should capture reusable commonality.

But how much commonality is sufficient?

### Potential Counterexample

An extracted CCC may be so generic that it provides no useful predictive or computational advantage.

### Proposed Validation

Define CCC usefulness through measurable reuse, transfer, compression, or evaluation benefits.

---

## Q-013 — How Can CCC Overgeneralization Be Detected?

**Priority:** P0  
**Related:** UCPSF-003, UCPSF-004

### Research Problem

Recursive distillation may progressively remove specialized distinctions.

### Potential Counterexample

A CCC that performs well across common cases fails on a domain-specific edge condition.

### Proposed Validation

Introduce:

- Applicability contracts;
- Counterexample tests;
- Specialized Delta preservation;
- Domain-shift evaluation;
- CCC splitting rules.

---

## Q-014 — Does Recursive CCC Distillation Converge?

**Priority:** P0  
**Related:** UCPSF-004, UCPSF-008

### Research Problem

Repeated CCC extraction may produce:

- Stable reusable cores;
- Cyclic structural revisions;
- Overgeneralization;
- Fragmentation;
- Unbounded complexity.

Under what conditions does recursive distillation stabilize?

### Potential Counterexample

Repeated merging and splitting of CCCs may never converge under changing task distributions.

### Proposed Validation

Study convergence, stability, and bounded-growth properties under controlled assumptions.

---

## Q-015 — Can Scoring CCCs Transfer Across Domains?

**Priority:** P0  
**Related:** UCPSF-004, UCPSF-008

### Research Problem

A CCC extracted from one task family may not remain valid in another.

### Potential Counterexample

A scoring structure optimized for software testing may transfer poorly to medical or financial decision support.

### Proposed Validation

Measure transfer performance under:

- Closely related tasks;
- Moderately different tasks;
- Strong distribution shifts;
- Incompatible evaluation semantics.

### Critical Research Principle

> A CCC should carry an explicit applicability boundary rather than an unrestricted claim of universality.

---

## Q-016 — How Should CCCs Be Promoted, Split, Merged, or Retired?

**Priority:** P1  
**Related:** UCPSF-004, UCPSF-007

### Research Problem

A CCC registry requires lifecycle management.

### Proposed Validation

Develop versioned lifecycle states and compare different promotion policies.

Evaluate the effects of:

- Premature promotion;
- Delayed promotion;
- Overaggressive merging;
- Excessive specialization;
- Retirement failures.

---

# Part IV — Perspective-Aware Meta-Scoring

## Q-017 — What Is a Complete Perspective Representation?

**Priority:** P0  
**Related:** UCPSF-005

### Research Problem

UCPSF proposes:

$$
P=(G,C,B,T,R)
$$

where the components represent goals, context and constraints, budget, time horizon, and risk preferences.

Is this representation sufficient?

### Potential Missing Dimensions

- Stakeholder authority;
- Legal obligations;
- Distributional fairness;
- Evidence quality;
- Irreversibility;
- Operational uncertainty.

### Proposed Validation

Test Perspective representations across diverse decision problems.

---

## Q-018 — How Can Meta-Scoring Avoid Circular Self-Validation?

**Priority:** P0  
**Related:** UCPSF-005, UCPSF-007

### Research Problem

If a system evaluates and modifies its own evaluators, it may create a self-reinforcing scoring loop.

### Potential Counterexample

A modified evaluator assigns higher scores to the modifications that produced it, while independent task quality declines.

### Proposed Validation

Require:

- Independent reference evaluators;
- Held-out benchmarks;
- Counter-evidence;
- Versioned evaluator lineage;
- Explicit authorization.

### Fundamental Boundary

> Evaluator evolution must not eliminate the independent evidence required to establish evaluator improvement.

---

## Q-019 — Can Meta-Scoring Improve Cost-Adjusted Decisions?

**Priority:** P0  
**Related:** UCPSF-005, CASE-001

### Research Problem

Meta-Scoring introduces additional computational overhead.

### Potential Counterexample

The cost of selecting an evaluator may exceed the cost of simply running the best fixed evaluator.

### Proposed Validation

Compare:

- Fixed evaluator;
- Simple heuristic selection;
- Learned evaluator selection;
- Full Meta-Scoring.

Measure quality, latency, cost, and selection regret.

---

## Q-020 — How Deep Should Meta-Evaluation Recurse?

**Priority:** P1  
**Related:** UCPSF-005

### Research Problem

If evaluators require evaluation, and Meta-Evaluators require evaluation, recursion may become unbounded.

### Proposed Validation

Investigate:

- Fixed recursion limits;
- Cost-based stopping;
- Value-of-Information thresholds;
- Independent terminal references.

---

## Q-021 — How Should Conflicting Perspectives Be Resolved?

**Priority:** P1  
**Related:** UCPSF-005, UCPSF-007

### Research Problem

Different stakeholders or components may assign incompatible priorities.

### Potential Counterexample

One Perspective optimizes speed while another requires additional verification.

### Proposed Validation

Compare:

- Lexicographic constraints;
- Multi-objective optimization;
- Explicit authority hierarchies;
- Negotiated policy resolution.

Mandatory governance constraints must not be silently converted into compensable score dimensions.

---

# Part V — Dual-Hybrid Intelligence

## Q-022 — Is Localization a Distinct Intelligence Capability?

**Priority:** P0  
**Related:** UCPSF-006

### Research Problem

UCPSF distinguishes Localization Intelligence from Per-Node Intelligence.

But Transformer models often perform these functions through tightly coupled operations.

### Potential Counterexample

Attempting to separate Localization from computation may destroy useful joint representations.

### Proposed Validation

Compare integrated and modular systems under controlled task conditions.

The decomposition should be evaluated as a functional abstraction, not assumed to imply physical independence.

---

## Q-023 — When Does Hybrid Composition Outperform Integrated Models?

**Priority:** P0  
**Related:** UCPSF-006, CASE-003

### Research Problem

Hybrid systems may improve specialization but introduce:

- Coordination overhead;
- Context translation;
- Interface failures;
- Additional latency;
- Error propagation.

### Proposed Validation

Compare:

- Integrated LLM;
- Retrieval-augmented LLM;
- Fixed structural-localization pipeline;
- Adaptive Dual-Hybrid system.

Measure end-to-end task outcomes and total resource cost.

---

## Q-024 — How Should Localization Quality Be Measured?

**Priority:** P1  
**Related:** UCPSF-006

### Research Problem

Retrieval accuracy alone may not capture whether localized context is sufficient for downstream reasoning.

### Proposed Validation

Measure:

- Context relevance;
- Context sufficiency;
- Identity preservation;
- Downstream task performance;
- Localization cost.

---

## Q-025 — What Contracts Are Required for Hybrid Engine Composition?

**Priority:** P0  
**Related:** UCPSF-006, UCPSF-007

### Research Problem

Heterogeneous engines may disagree on:

- Input representation;
- Context identity;
- Uncertainty semantics;
- Output guarantees;
- Authority;
- Resource limits.

### Proposed Validation

Develop explicit composition contracts and conformance tests.

Test whether incompatible combinations are rejected before runtime.

---

## Q-026 — Can Dual-Hybrid Selection Learn Reusable CCCs?

**Priority:** P1  
**Related:** UCPSF-006, CASE-003

### Research Problem

Repeated engine-selection decisions may reveal reusable structural patterns.

### Potential Counterexample

Selection rules learned on one workload may overfit and perform poorly on another.

### Proposed Validation

Compare learned selection CCCs against fixed rules and task-specific selectors.

---

# Part VI — Universal Control Plane

## Q-027 — What Does Universal Mean in Universal Control Plane?

**Priority:** P0  
**Related:** UCPSF-007, UCPSF-008

### Research Problem

The term **Universal** may refer to different levels of generality.

Possible interpretations include:

1. A common architectural interface;
2. A common contract system;
3. A common evaluation representation;
4. A common governance framework;
5. A universally effective control algorithm.

These claims are not equivalent.

### Potential Counterexample

A shared Control Plane interface may work across domains while the optimal scoring mechanisms remain highly domain-specific.

### Proposed Validation

Separate claims of interface generality from claims of algorithmic universality.

**Recommended research position:**

> Universal should initially refer to a proposed extensible control architecture and contract framework, not a claim that one evaluator or control algorithm is optimal for every task.

---

## Q-028 — Which Control Plane Functions Must Remain Independent?

**Priority:** P0  
**Related:** UCPSF-007

### Research Problem

Execution, evaluation, governance, and structural learning may interact.

Which responsibilities require separation?

### Potential Counterexample

A component generates a structural modification, evaluates it, and authorizes its own deployment.

### Proposed Validation

Define explicit authority and evidence boundaries.

Test whether the architecture prevents unauthorized promotion paths.

---

## Q-029 — Can a Universal Control Plane Scale Across Complex AI Systems?

**Priority:** P1  
**Related:** UCPSF-007

### Research Problem

Centralized coordination may introduce:

- Bottlenecks;
- Latency;
- Single points of failure;
- Governance complexity.

### Proposed Validation

Compare centralized, hierarchical, and federated Control Plane designs.

---

## Q-030 — How Should Federated Control Planes Resolve Conflicts?

**Priority:** P1  
**Related:** UCPSF-007, UCPSF-008

### Research Problem

Multiple bounded intelligence units may maintain different policies and priorities.

### Proposed Validation

Investigate:

- Local sovereignty;
- Delegated authority;
- Contract negotiation;
- Conflict escalation;
- Evidence exchange;
- Revocation and rollback.

---

## Q-031 — Can Control Plane Contracts Be Verified Before Runtime?

**Priority:** P0  
**Related:** UCPSF-006, UCPSF-007

### Research Problem

Specifications/Contracts First is a central engineering principle.

But some compatibility properties may depend on runtime behavior.

### Proposed Validation

Separate:

- Static contract validation;
- Sandbox conformance;
- Runtime monitoring;
- Post-deployment verification.

Determine which guarantees can be established at each stage.

---

# Part VII — Structural RSI and Recursive Evolution

## Q-032 — What Constitutes Genuine Structural Improvement?

**Priority:** P0  
**Related:** UCPSF-007, CASE-002

### Research Problem

Structural modification may improve one metric while degrading another.

### Potential Counterexample

A new dispatch architecture reduces latency but increases harmful error rates.

### Proposed Validation

Define improvement relative to:

- Task quality;
- Cost;
- Reliability;
- Risk;
- Transferability;
- Governance constraints.

Avoid treating a single scalar reward as sufficient evidence of improvement.

---

## Q-033 — Can Intelligence and Evaluation Architectures Co-Evolve Safely?

**Priority:** P0  
**Related:** UCPSF-007, UCPSF-008

### Research Problem

Structural RSI may modify both:

- The architecture performing tasks;
- The architecture evaluating tasks.

This creates a risk of self-referential optimization.

### Proposed Validation

Compare:

1. Fixed evaluator, evolving intelligence;
2. Evolving evaluator, fixed intelligence;
3. Joint evolution with independent references;
4. Joint evolution without independent references.

Measure improvement validity and harmful promotion rates.

---

## Q-034 — What Prevents Recursive Goodhart Effects?

**Priority:** P0  
**Related:** UCPSF-005, UCPSF-007

### Research Problem

Repeated optimization may progressively exploit weaknesses in the evaluation system.

### Potential Counterexample

Each generation improves benchmark scores while generalization declines.

### Proposed Validation

Use:

- Held-out tasks;
- Independent outcome measures;
- Adversarial counterexamples;
- Evaluator version tracking;
- Distribution-shift testing.

---

## Q-035 — How Should Structural Promotion Be Governed?

**Priority:** P0  
**Related:** UCPSF-007, CASE-002

### Research Problem

A candidate may pass local evaluation without being suitable for deployment.

### Proposed Validation

Develop a promotion state machine with:

- Contract validation;
- Sandbox evaluation;
- Independent validation;
- Authorization;
- Controlled deployment;
- Monitoring;
- Rollback.

Evaluate both false promotions and missed beneficial promotions.

---

## Q-036 — Can Structural RSI Produce Sustained Improvements?

**Priority:** P0  
**Related:** UCPSF-007, UCPSF-008

### Research Problem

One successful modification does not establish recursive improvement.

### Potential Counterexample

Early generations improve performance, followed by stagnation, regressions, or evaluator exploitation.

### Proposed Validation

Conduct longitudinal experiments over multiple bounded generations.

Measure:

- Net task improvement;
- Evaluation validity;
- Structural complexity;
- Cost;
- Regression rate;
- Recovery effectiveness.

---

# Part VIII — Collective and Open-Ended Scoring Intelligence

## Q-037 — Can Scoring CCCs Become Portable Intelligence Components?

**Priority:** P2  
**Related:** UCPSF-004, UCPSF-008

### Research Problem

Portable Scoring CCCs may support reuse across compatible systems.

### Proposed Validation

Develop portable formats containing:

- Structural representation;
- Contracts;
- Applicability boundaries;
- Evidence provenance;
- Version information;
- Known limitations.

Test transfer across independent runtimes.

---

## Q-038 — Can Collective Structural Learning Improve Evaluation Quality?

**Priority:** P2  
**Related:** UCPSF-008

### Research Problem

Multiple systems may contribute evaluation structures and counterexamples.

### Potential Counterexample

Shared structures may introduce correlated failures or propagate invalid assumptions.

### Proposed Validation

Compare isolated learning with controlled structural exchange.

Measure transfer benefit and failure propagation.

---

## Q-039 — How Can Collective Learning Preserve Local Sovereignty?

**Priority:** P2  
**Related:** UCPSF-007, UCPSF-008

### Research Problem

Structural exchange should not imply unrestricted control over receiving systems.

### Proposed Validation

Investigate:

- Local validation;
- Local authorization;
- Contract compatibility;
- Revocable component adoption;
- Evidence provenance;
- Federated governance.

---

## Q-040 — Is Open-Ended Scoring Intelligence Computationally Sustainable?

**Priority:** P2  
**Related:** UCPSF-008

### Research Problem

Continuous structural growth may increase complexity and maintenance costs.

### Potential Counterexample

A system accumulates increasingly elaborate Scoring Forests without measurable improvement.

### Proposed Validation

Measure capability growth relative to:

- Compute;
- Memory;
- Evaluation overhead;
- Maintenance cost;
- Governance complexity.

---

# Part IX — Decisive Counterexamples and Falsification Tests

The following tests are especially important because they challenge central UCPSF assumptions.

## F-001 — Scoring Forests Fail to Beat Simple Evaluators

**Challenge:** Rich evaluation structures provide no meaningful benefit after accounting for overhead.

**Implication:** Scoring Forests may be useful only for limited task classes.

**Required response:** Narrow the applicability claim rather than assuming additional complexity will solve the problem.

---

## F-002 — Unaligned AND Folding Destroys Critical Decisions

**Challenge:** Extracted commonality removes rare but important evaluation distinctions.

**Implication:** Folding requires stronger preservation contracts or more conservative specialization.

**Required response:** Reject or revise the Folding mechanism for the affected domain.

---

## F-003 — CCC Transfer Produces Negative Transfer

**Challenge:** A CCC improves source-domain evaluation but degrades target-domain outcomes.

**Implication:** CCC applicability boundaries are insufficient.

**Required response:** Improve domain contracts, splitting rules, or transfer validation.

---

## F-004 — Meta-Scoring Costs More Than It Saves

**Challenge:** Evaluator selection overhead exceeds the benefit of adaptive evaluation.

**Implication:** Meta-Scoring may require narrow activation conditions.

**Required response:** Develop bounded selection policies or prefer fixed evaluators.

---

## F-005 — Hybrid Architecture Underperforms Integrated Models

**Challenge:** Modular composition introduces more errors or cost than specialization benefits justify.

**Implication:** Dual-Hybrid systems should retain integrated models as first-class candidates.

**Required response:** Revise the selection policy rather than assuming modularity is inherently superior.

---

## F-006 — Evaluator Evolution Produces False Improvement

**Challenge:** Evolving evaluators increasingly reward the modifications that created them.

**Implication:** Joint evolution without independent references is unreliable.

**Required response:** Strengthen evaluator independence, evidence requirements, and promotion governance.

---

## F-007 — Universal Control Plane Becomes a Bottleneck

**Challenge:** Centralized control reduces system performance or resilience.

**Implication:** Universal architectural coordination may require hierarchical or federated implementations.

**Required response:** Separate logical universality from centralized physical deployment.

---

## F-008 — Structural RSI Fails to Sustain Progress

**Challenge:** Repeated structural modification leads to stagnation, regression, or escalating complexity.

**Implication:** Open-ended structural improvement is not established.

**Required response:** Investigate bounded improvement regimes, structural retirement, and stronger validation.

---

# Part X — Proposed Research Experiments

## E-001 — Scoring Tree Baseline Experiment

**Objective:** Compare a structured Scoring Tree with fixed scoring baselines.

**Primary metrics:** Quality, cost, calibration, latency.

**Related questions:** Q-001, Q-003, Q-005.

---

## E-002 — Unaligned Folding Preservation Experiment

**Objective:** Test whether heterogeneous Scoring Trees can be folded while preserving specified decisions.

**Primary metrics:** Decision agreement, long-tail regression, compression, cost.

**Related questions:** Q-008, Q-009, Q-010.

---

## E-003 — Recursive CCC Transfer Experiment

**Objective:** Evaluate CCC extraction, reuse, and cross-domain transfer.

**Primary metrics:** Transfer gain, applicability accuracy, negative-transfer rate.

**Related questions:** Q-012 through Q-016.

---

## E-004 — Perspective-Aware Meta-Scoring Experiment

**Objective:** Compare adaptive evaluator selection against fixed strategies.

**Primary metrics:** Cost-adjusted utility, selection regret, robustness.

**Related questions:** Q-017 through Q-021.

---

## E-005 — Dual-Hybrid Engine Selection Experiment

**Objective:** Compare integrated and adaptive hybrid architectures.

**Primary metrics:** Task quality, total cost, localization quality, composition failures.

**Related questions:** Q-022 through Q-026.

---

## E-006 — Control Plane Conformance Experiment

**Objective:** Test explicit contracts, authorization boundaries, and workflow auditability.

**Primary metrics:** Contract violations, unauthorized promotions, trace completeness, overhead.

**Related questions:** Q-027 through Q-031.

---

## E-007 — Governed Structural RSI Experiment

**Objective:** Compare structural evolution with and without independent validation and governed promotion.

**Primary metrics:** Genuine improvement, harmful promotion rate, regression, rollback success.

**Related questions:** Q-032 through Q-036.

---

## E-008 — Collective Scoring CCC Transfer Experiment

**Objective:** Test portable evaluation structures across independent systems.

**Primary metrics:** Transfer benefit, conformance, failure propagation, governance compliance.

**Related questions:** Q-037 through Q-040.

---

## 11. Priority Research Matrix

| Research Area | Foundational Question | Suggested First Experiment |
|---|---|---|
| Scoring Intelligence | Q-001 | E-001 |
| Operator Composition | Q-003 | E-001 |
| Unaligned AND Folding | Q-008 | E-002 |
| Decision Preservation | Q-009 | E-002 |
| CCC Transfer | Q-015 | E-003 |
| Meta-Scoring Independence | Q-018 | E-004 and E-007 |
| Hybrid Architecture | Q-023 | E-005 |
| Universal Control Plane | Q-027 | E-006 |
| Control Contracts | Q-031 | E-006 |
| Structural Improvement | Q-032 | E-007 |
| Evaluator Co-Evolution | Q-033 | E-007 |
| Collective Learning | Q-038 | E-008 |

---

## 12. Recommended Near-Term Priorities

The following five questions are recommended as the first research priorities.

### Priority 1 — Q-003: Scoring Contract and Composition Semantics

Without valid score semantics, Scoring Trees and Forests may combine incompatible evaluators.

### Priority 2 — Q-008 and Q-009: Unaligned AND Folding and Decision Preservation

These questions determine whether structural Scoring CCC extraction can be made rigorous.

### Priority 3 — Q-018: Meta-Scoring Independence

This question determines whether evaluator evolution can avoid circular self-validation.

### Priority 4 — Q-023: Hybrid Composition Benefit

This question tests whether Dual-Hybrid Intelligence provides practical value beyond fixed architectures.

### Priority 5 — Q-033: Intelligence and Evaluation Co-Evolution

This question determines whether Structural RSI can evolve both execution and evaluation architectures while retaining credible evidence of improvement.

---

## 13. Research Question Lifecycle

Each open question should eventually receive one of the following statuses:

- **OPEN:** Not yet resolved.
- **FORMALIZED:** A precise problem definition exists.
- **UNDER TEST:** Experimental or analytical investigation is underway.
- **PARTIALLY SUPPORTED:** Evidence supports a limited claim.
- **REFUTED:** Evidence contradicts the stated hypothesis under defined conditions.
- **REVISED:** The original question or claim has been narrowed or modified.
- **RESOLVED:** A sufficiently supported answer exists within explicitly stated boundaries.

A question should not be marked resolved merely because an implementation works on a small demonstration.

### Suggested Future Tracking Record

```text id="v9fryo"
Question ID:
Status:
Formal Definition:
Hypothesis:
Baseline:
Experimental Protocol:
Evidence:
Counter-Evidence:
Known Limitations:
Decision:
Version:
```

This structure may support future issue tracking and research documentation.

---

## 14. Relationship to the UCPSF Research Papers

| Research Paper | Principal Open Questions |
|---|---|
| [UCPSF-001](docs/UCPSF-001-From-Primitive-Scoring-to-Generalized-Scoring-Intelligence.md) | Q-001 to Q-005 |
| [UCPSF-002](docs/UCPSF-002-Universal-Control-Planes-and-Three-Scoring-Operators.md) | Q-002 to Q-004 |
| [UCPSF-003](docs/UCPSF-003-Scoring-Trees-Forests-and-Unaligned-AND-Folding.md) | Q-006 to Q-011 |
| [UCPSF-004](docs/UCPSF-004-Common-Concept-Core-Extraction-and-Recursive-Distillation.md) | Q-008 to Q-016 |
| [UCPSF-005](docs/UCPSF-005-Perspective-Aware-Optimization-and-Meta-Scoring-Intelligence.md) | Q-017 to Q-021 |
| [UCPSF-006](docs/UCPSF-006-Hybrid-Localization-and-Per-Node-Intelligence.md) | Q-022 to Q-026 |
| [UCPSF-007](docs/UCPSF-007-Universal-Control-Plane-Architecture-and-Structural-RSI.md) | Q-027 to Q-036 |
| [UCPSF-008](docs/UCPSF-008-Open-Ended-Scoring-Intelligence-and-the-Future-of-AI.md) | Q-037 to Q-040 |

### Related Case Studies

- [CASE-001 — Scoring Control in AI Relay](cases/CASE-001-Scoring-Control-in-AI-Relay.md)
- [CASE-002 — Scoring-Guided Structural RSI](cases/CASE-002-Scoring-Guided-Structural-RSI.md)
- [CASE-003 — Hybrid Localization and Per-Node Selection](cases/CASE-003-Hybrid-Localization-and-Per-Node-Selection.md)

---

## 15. Research Integrity Principles

The UCPSF research program should maintain the following principles.

### 15.1 Separate Hypotheses from Results

Proposed mechanisms should not be described as empirically established without supporting evidence.

### 15.2 Preserve Counter-Evidence

Failed experiments and counterexamples are important research outputs.

### 15.3 Compare Against Simpler Baselines

Additional structural complexity must justify its cost.

### 15.4 Record Applicability Boundaries

A validated result should specify the conditions under which it holds.

### 15.5 Maintain Independent Evaluation

Candidate-generating systems should not control all criteria used to validate their own improvements.

### 15.6 Treat Governance as a Separate Responsibility

Scoring results may inform decisions but do not themselves confer authorization.

### 15.7 Revise Claims When Evidence Requires It

A failed general hypothesis may still yield a useful specialized mechanism.

---

## 16. Final Perspective

The central uncertainty of UCPSF is not whether complex AI systems can be equipped with more scoring mechanisms.

They clearly can.

The deeper question is whether evaluation structures can become:

- More reusable;
- More transferable;
- More adaptive;
- More reliable;
- More computationally efficient;
- More governable;
- More capable of supporting validated structural evolution.

The most consequential open question is:

> **Can intelligence systems improve the structures by which they evaluate intelligence without losing the independent evidence needed to distinguish genuine progress from self-reinforcing optimization?**

Answering this question requires progress in Scoring Contracts, Structural Folding, CCC learning, Meta-Scoring, Hybrid Intelligence, and governance.

The UCPSF framework is intended to organize these investigations.

Its success must ultimately be judged by reproducible evidence rather than architectural ambition alone.

---

## Citation

Suggested citation before DOI assignment:

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

**OPEN QUESTIONS — UCPSF Research Problems and Falsification Agenda**  
**Sizhe Tan & GPT-Obot | October 2026 | Version 1.0.0**
