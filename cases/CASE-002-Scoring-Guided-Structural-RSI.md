
# CASE-002 — Scoring-Guided Structural RSI

**Subtitle:** Rich Evaluators, Recursive Structural Improvement, Counter-Evidence, and Governed Evolution of Intelligence Systems

**Authors:** Sizhe Tan & GPT-Obot  
**Project:** Universal Control Planes and Scoring Tree/Forest/Folding for Structural Intelligence (UCPSF)  
**Document ID:** CASE-002  
**Version:** 1.0.0  
**Date:** October 15, 2026  
**Status:** Conceptual Case Study and Proposed Validation Design  
**License:** Apache-2.0

---

## Abstract

Recursive Self-Improvement (RSI) investigates whether an intelligence system can improve its own capabilities through repeated modification and evaluation.

Structural RSI extends the improvement space beyond model parameters and prompts to include Localization Engines, Per-Node Intelligence Engines, Calling Graphs, Scoring Trees, Common Concept Cores (CCCs), and Control Plane configurations.

This broader modification space introduces a fundamental challenge: the system must distinguish genuine improvement from changes that merely increase internal scores, shift evaluation criteria, exploit evaluator weaknesses, or introduce hidden structural regressions.

This case study proposes **Scoring-Guided Structural RSI**, an architecture in which a Universal Control Plane coordinates structural modification through Perspective-Aware Scoring Forests, Meta-Scoring Intelligence, independent validation, counter-evidence, and governed promotion.

The case examines a hypothetical software-engineering intelligence system that proposes improvements to its own task localization, execution, dispatch, and evaluation structures.

We distinguish two coupled but separately governed evolutionary processes: **Intelligence Architecture Evolution**, which modifies how tasks are performed, and **Evaluation Architecture Evolution**, which modifies how task outcomes and structural changes are judged.

A staged promotion protocol is introduced to prevent candidate changes from unilaterally controlling their own acceptance criteria.

The proposed process incorporates explicit contracts, immutable reference evaluations where appropriate, independent evidence, long-tail testing, rollback, and bounded recursive search.

We also examine how repeated improvement campaigns may generate reusable Scoring CCCs through Unaligned AND Folding and recursive distillation.

The study provides a conceptual execution algorithm, failure-mode analysis, baseline comparisons, and a falsifiable experimental research agenda.

No autonomous RSI capability or empirical performance improvement is claimed.

The central hypothesis is that **richer, independently governed scoring structures can improve the reliability and directionality of Structural RSI relative to optimization driven by a single fixed reward or self-assessed metric**, under specified conditions.

**Keywords:** Structural Recursive Self-Improvement, Structural RSI, Scoring Intelligence, Rich Evaluators, Universal Control Plane, Meta-Scoring, Scoring Forest, Common Concept Core, Counter-Evidence, Anti-Goodhart, Structural Folding, Independent Validation, Governed Promotion

---

## 1. Introduction

### 1.1 Recursive Self-Improvement

Recursive Self-Improvement refers to processes in which an intelligence system contributes to modifications intended to improve its own future performance.

Possible modifications include:

- Prompt and instruction refinement;
- Model selection;
- Tool-use strategies;
- Search policies;
- Memory structures;
- Evaluation methods;
- Computational workflows;
- Model parameters;
- System architecture.

The effectiveness of an RSI process depends not only on its ability to generate candidate improvements but also on its ability to evaluate them.

### 1.2 From Parameter RSI to Structural RSI

A parameter-focused improvement process modifies a relatively constrained set of numerical variables.

Structural RSI expands the candidate space.

For example, an intelligence system may propose:

- A different Localization Engine;
- A specialized Per-Node Intelligence Engine;
- A revised Calling Graph;
- A new Scoring Tree;
- A folded evaluation structure;
- A different context representation;
- A new CCC;
- A revised dispatch policy.

These modifications may interact.

Consequently, a local improvement may create unexpected system-level effects.

### 1.3 The Evaluator Bottleneck

An RSI system may generate many candidate changes.

However, candidate generation does not establish that a change is beneficial.

The system needs evaluation mechanisms capable of distinguishing:

- Genuine task improvement;
- Reduced computation without unacceptable quality loss;
- Better transfer;
- Increased robustness;
- Hidden regressions;
- Metric exploitation;
- Policy violations.

A single reward signal may be insufficient for this purpose.

### 1.4 Case Study Objective

This study investigates a proposed architecture for guiding Structural RSI through richer evaluation and explicit governance.

The objective is to make structural improvement:

1. Measurable;
2. Evidence-driven;
3. Perspective-aware;
4. Reversible where feasible;
5. Governed by explicit authority.

---

## 2. Hypothetical System Under Improvement

### 2.1 System Definition

Consider an AI software-engineering system responsible for:

- Interpreting requirements;
- Localizing relevant code;
- Generating modifications;
- Running tests;
- Reviewing results;
- Reporting outcomes.

The system contains several interchangeable components.

### 2.2 Localization Layer

Candidate Localization Engines include:

- Semantic retrieval;
- Transformer-based contextual localization;
- Metric Differential Tree (MDT) search;
- UTN-based structural localization;
- Calling Graph traversal.

### 2.3 Intelligence Execution Layer

Candidate Per-Node Intelligence Engines include:

- General-purpose LLMs;
- Specialized coding models;
- Symbolic analyzers;
- Test-generation engines;
- Optimization tools.

### 2.4 Evaluation Layer

The system contains:

- Functional correctness evaluators;
- Test coverage evaluators;
- Cost estimators;
- Reliability evaluators;
- Security checkers;
- Scoring Trees;
- Scoring Forests;
- Meta-Scoring mechanisms.

### 2.5 Control Layer

A Universal Control Plane manages:

- Perspective;
- Contracts;
- Engine selection;
- Evaluation;
- Resource budgets;
- Structural modification;
- Promotion;
- Monitoring;
- Rollback.

### 2.6 Improvement Target

The system seeks to improve its performance on a distribution of software-engineering tasks.

A candidate objective is:

$$
\max_{\theta} U(\theta\mid P)
$$

subject to:

$$
C_{\mathrm{mandatory}}(\theta)=\mathrm{true}
$$

and:

$$
Cost(\theta)\leq B
$$

where:

- \(\theta\): System configuration;
- \(P\): Perspective;
- \(U\): Evaluated utility;
- \(B\): Resource budget.

The objective is conceptual.

In practice, utility may require multiple non-commensurable dimensions rather than a single scalar.

---

## 3. Baseline — Single-Reward Structural Optimization

### 3.1 Baseline Workflow

A simple RSI process may follow:

```text
Current System
      |
      v
Generate Candidate Modification
      |
      v
Run Evaluation
      |
      v
Compute Reward
      |
      v
Accept if Reward Improves
      |
      v
Repeat
```

### 3.2 Strengths

This approach may be effective when:

- Objectives are stable;
- Evaluation is reliable;
- Candidate modifications are constrained;
- The task distribution is well represented;
- Reward exploitation is limited.

### 3.3 Limitations

Potential limitations include:

**Evaluator Exploitation**

The candidate improves the reward without improving the intended outcome.

**Hidden Regression**

An average score improves while rare but important tasks degrade.

**Evaluation Drift**

The scoring mechanism becomes less reliable over time.

**Structural Interaction**

A local improvement creates negative effects elsewhere.

**Cost Blindness**

A candidate improves quality while introducing excessive computational expense.

**Policy Blindness**

A candidate violates mandatory constraints despite favorable scores.

### 3.4 Research Motivation

The proposed architecture investigates whether a richer evaluation structure can address these limitations.

---

## 4. Proposed Scoring-Guided Structural RSI Architecture

### 4.1 Architectural Overview

```text
                    HUMAN / GOVERNANCE AUTHORITY
                               |
                               v
                      UNIVERSAL CONTROL PLANE
                               |
              +----------------+----------------+
              |                                 |
              v                                 v
       STRUCTURAL RSI ENGINE             SCORING INTELLIGENCE
              |                                 |
       Candidate Generation               Scoring Trees
       Architecture Search                Scoring Forests
       Structural Folding                 Meta-Scoring
       CCC Proposals                      Counter-Evidence
              |                                 |
              +----------------+----------------+
                               |
                               v
                     INDEPENDENT VALIDATION
                               |
                               v
                       PROMOTION DECISION
                               |
                   +-----------+-----------+
                   |                       |
                   v                       v
                PROMOTE                 REJECT
                   |
                   v
                 MONITOR
                   |
                   v
              EVIDENCE FEEDBACK
```

### 4.2 Separation of Responsibilities

The architecture distinguishes:

- Candidate generation;
- Candidate evaluation;
- Independent validation;
- Authorization;
- Deployment;
- Monitoring.

These responsibilities may share infrastructure but should not share unrestricted decision authority.

### 4.3 Control Plane Role

The Universal Control Plane coordinates the improvement process.

It does not automatically authorize every modification proposed by the RSI engine.

### 4.4 Scoring Intelligence Role

Scoring Intelligence evaluates the quality, applicability, cost, and risk of proposed structural changes.

### 4.5 Independent Validation Role

Independent validation assesses whether apparent improvements generalize beyond the candidate's internal optimization signals.

---

## 5. Structural Modification Space

### 5.1 Candidate Representation

Let:

$$
\Theta =
(\Theta_L,\Theta_I,\Theta_D,\Theta_S,\Theta_K,\Theta_C)
$$

where:

- \(\Theta_L\): Localization structures;
- \(\Theta_I\): Intelligence Engines;
- \(\Theta_D\): Dispatch and Calling Graphs;
- \(\Theta_S\): Scoring structures;
- \(\Theta_K\): CCC structures;
- \(\Theta_C\): Composition contracts.

### 5.2 Localization Modifications

Examples include:

- Replacing semantic retrieval with MDT-assisted localization;
- Adding UTN references;
- Improving Calling Graph traversal;
- Introducing specialized context selection.

### 5.3 Intelligence Engine Modifications

Examples include:

- Replacing a general model with a specialist for selected tasks;
- Introducing an ANN scorer;
- Adding a symbolic verification step;
- Combining multiple engines.

### 5.4 Dispatch Modifications

Examples include:

- Revising routing thresholds;
- Adding a specialist branch;
- Folding redundant branches;
- Changing escalation conditions.

### 5.5 Scoring Modifications

Examples include:

- Adding a risk dimension;
- Recalibrating an evaluator;
- Distilling a Scoring Tree;
- Revising Meta-Scoring selection rules.

### 5.6 CCC Modifications

Examples include:

- Extracting a reusable evaluation core;
- Splitting an overgeneralized CCC;
- Preserving specialized Delta;
- Retiring an invalid core.

### 5.7 Contract Modifications

Contract changes may affect interoperability and governance.

Such changes require compatibility analysis and explicit approval.

---

## 6. Rich Evaluators for Structural RSI

### 6.1 Why Rich Evaluators?

Structural changes may affect multiple dimensions simultaneously.

A single reward may obscure important tradeoffs.

### 6.2 Candidate Scoring Forest

$$
\mathcal{F}_S=
\{
T_Q,T_C,T_R,T_T,T_G,T_M
\}
$$

where:

- \(T_Q\): Quality;
- \(T_C\): Cost;
- \(T_R\): Risk;
- \(T_T\): Transferability;
- \(T_G\): Governance and constraints;
- \(T_M\): Maintainability.

### 6.3 Quality Evaluation

Measure task outcomes using independent reference tasks.

### 6.4 Cost Evaluation

Measure:

- Execution cost;
- Evaluation cost;
- Training or adaptation cost;
- Maintenance overhead.

### 6.5 Risk Evaluation

Assess:

- Failure severity;
- Regression likelihood;
- Uncertainty;
- Long-tail behavior;
- Recovery capability.

### 6.6 Transferability

Determine whether improvements apply beyond the original optimization tasks.

### 6.7 Governance

Evaluate policy-relevant properties while preserving independent authorization enforcement.

### 6.8 Maintainability

Assess whether the structural change increases complexity beyond its expected benefit.

### 6.9 Multi-Objective Evaluation

A candidate may improve quality but increase cost.

The Control Plane should use Perspective-aware tradeoffs rather than assuming one fixed weighting is always appropriate.

### 6.10 Hard Constraints

Mandatory constraints must be enforced independently of compensable scoring dimensions.

---

## 7. Perspective-Aware Structural Improvement

### 7.1 Perspective Definition

Following UCPSF-005:

$$
P=(G,C,B,T,R)
$$

where:

- \(G\): Goals;
- \(C\): Context and constraints;
- \(B\): Resource budget;
- \(T\): Time horizon;
- \(R\): Risk preferences.

### 7.2 Example Perspectives

**Low-Cost Deployment**

Prioritizes efficiency while maintaining minimum quality requirements.

**High-Reliability Engineering**

Prioritizes robustness and regression prevention.

**Exploratory Research**

Allows broader structural experimentation within controlled environments.

**Security-Sensitive Operation**

Requires stronger evidence and authorization.

### 7.3 Perspective-Conditioned Promotion

A structural change may be acceptable under one Perspective and unsuitable under another.

For example, a faster but less robust engine may be appropriate for low-risk prototyping but not for security-sensitive deployment.

### 7.4 Perspective Does Not Override Governance

A favorable Perspective-specific score cannot authorize a prohibited action.

---

## 8. Two-Level Structural Evolution

### 8.1 Intelligence Architecture Evolution

This process modifies how the system performs tasks.

Examples include:

- Better Localization Engines;
- Specialized Per-Node Engines;
- Improved Calling Graphs;
- More efficient context structures.

### 8.2 Evaluation Architecture Evolution

This process modifies how the system evaluates tasks and structural changes.

Examples include:

- Revised Scoring Trees;
- New risk dimensions;
- Improved ANN evaluators;
- Refined CCCs;
- Better Meta-Scoring.

### 8.3 The Co-Evolution Problem

If the system changes both its task architecture and its evaluator simultaneously, apparent improvement may be difficult to interpret.

### 8.4 Staged Evolution

We propose:

```text
Reference Evaluation Baseline
            |
            v
Intelligence Architecture Proposal
            |
            v
Independent Validation
            |
            v
Evidence Collection
            |
            v
Evaluator Improvement Proposal
            |
            v
Separate Evaluator Validation
            |
            v
Governed Promotion
```

### 8.5 Evaluator Versioning

Each structural experiment should record:

- Candidate version;
- Evaluator version;
- Reference benchmark version;
- Perspective;
- Evidence provenance.

### 8.6 Non-Monotonic Evolution

The system must allow:

- Failed modifications;
- Rejected candidates;
- Rollback;
- Specialization;
- Retirement.

Progress cannot be assumed from revision count alone.

---

## 9. Meta-Scoring Intelligence

### 9.1 Evaluating Evaluators

Meta-Scoring assesses the reliability and suitability of evaluation mechanisms.

### 9.2 Candidate Dimensions

Potential dimensions include:

- Calibration;
- Predictive validity;
- Robustness;
- Domain applicability;
- Cost;
- Independence;
- Constraint coverage.

### 9.3 Evaluator Selection

A low-risk modification may require a lightweight evaluator.

A high-risk structural change may require multiple independent validators.

### 9.4 Evaluator Drift

An evaluator may become less reliable as the system evolves.

Meta-Scoring should help detect discrepancies between internal scores and external outcomes.

### 9.5 Recursive Evaluation Boundaries

Meta-evaluators may themselves be evaluated.

However, recursive evaluation must be bounded by explicit stopping conditions and independent references.

### 9.6 Evaluator Promotion

A candidate evaluator should not determine its own promotion solely through its own outputs.

---

## 10. Counter-Evidence and Anti-Goodhart Control

### 10.1 The Goodhart Problem

When a measure becomes an optimization target, it may cease to reliably represent the intended objective.

Structural RSI can amplify this problem because the system may repeatedly search for changes that improve the same evaluation signals.

### 10.2 Counter-Evidence

Counter-evidence includes observations that challenge a proposed improvement.

Examples include:

- Regression on held-out tasks;
- Failure under distribution shift;
- Increased resource cost;
- Hidden security vulnerabilities;
- Reduced transferability;
- Unexpected interaction effects.

### 10.3 Counter-Evidence Search

The Control Plane should actively search for conditions under which a candidate performs worse than the reference system.

### 10.4 Long-Tail Validation

Rare cases may be especially important.

A candidate that improves average performance while introducing severe long-tail failures may be unsuitable.

### 10.5 Evaluator Independence

Multiple evaluators are not necessarily independent.

They may share:

- Training data;
- Model lineage;
- Reward assumptions;
- Benchmark leakage;
- Organizational incentives.

### 10.6 Independent References

Possible reference mechanisms include:

- Held-out benchmarks;
- External outcome measurements;
- Formal checks;
- Human review;
- Adversarial tests;
- Separate evaluation models.

### 10.7 Anti-Goodhart Principle

> Structural improvement should be judged against independently grounded objectives, not merely against the metrics used to generate the candidate.

---

## 11. Structural Folding and CCC Growth

### 11.1 Repeated Improvement Patterns

Across many RSI campaigns, the system may encounter recurring evaluation and modification structures.

### 11.2 Scoring Tree Samples

Each campaign may produce:

- A candidate modification;
- A Scoring Tree;
- A decision trace;
- Validation evidence;
- Counter-evidence.

### 11.3 Unaligned AND Folding

Different Scoring Trees may express similar evaluation principles through different structures.

Unaligned AND Folding may identify candidate commonality.

### 11.4 Structural CCC

A Structural CCC captures reusable evaluation organization.

### 11.5 Behavioral CCC

A Behavioral CCC captures recurring decision behavior under specified conditions.

### 11.6 Core Plus Delta

A candidate decomposition is:

$$
T_i \approx K \oplus \Delta_i
$$

where:

- \(K\): Common Concept Core;
- \(\Delta_i\): Specialized differences.

### 11.7 Recursive Distillation

As more evidence becomes available, CCCs may be:

- Refined;
- Specialized;
- Split;
- Merged;
- Retired;
- Promoted.

### 11.8 CCC Validation

A CCC should be evaluated for:

- Decision preservation;
- Transferability;
- Robustness;
- Cost;
- Applicability boundaries.

### 11.9 Structural Growth

Validated CCCs may improve future evaluation efficiency.

However, structural growth should not be inferred merely from increasing CCC count.

---

## 12. Governed Promotion Protocol

### 12.1 Candidate Lifecycle

```text
Structural Proposal
        |
        v
Contract Validation
        |
        v
Sandbox Evaluation
        |
        v
Independent Validation
        |
        v
Counter-Evidence Search
        |
        v
Governance Authorization
        |
        v
Canary Deployment
        |
        v
Monitoring
        |
        +----> Promote
        |
        +----> Revise
        |
        +----> Roll Back
        |
        +----> Retire
```

### 12.2 Contract Validation

Check:

- Input-output compatibility;
- Context identity;
- Capability declarations;
- Evaluation semantics;
- Version compatibility;
- Policy requirements.

### 12.3 Sandbox Evaluation

Test the candidate in an isolated environment.

### 12.4 Independent Validation

Evaluate against reference baselines and held-out tasks.

### 12.5 Counter-Evidence Search

Attempt to identify conditions under which the candidate fails.

### 12.6 Authorization

A designated governance authority determines whether deployment is permitted.

### 12.7 Canary Deployment

Where feasible, deploy the candidate to a limited scope.

### 12.8 Monitoring

Collect evidence about:

- Task outcomes;
- Resource consumption;
- Reliability;
- Distribution shift;
- Constraint compliance.

### 12.9 Rollback

Restore a previous validated configuration when necessary and technically feasible.

### 12.10 Promotion Principle

**A structural candidate must not gain deployment authority merely by improving its own internal evaluation score.**

---

## 13. Proposed Structural RSI Algorithm

```text
Algorithm: Scoring-Guided-Structural-RSI

Input:
    Current Architecture A
    Perspective P
    Scoring Forest S
    Meta-Scoring Registry M
    Contract Registry C
    Evidence Repository E
    Governance Rules G
    Resource Budget B

Output:
    Validated Architecture A'
    Evidence Trace T
    Structural Learning Record R

1. Resolve Perspective P.

2. Resolve mandatory governance constraints G.

3. Establish reference architecture A.

4. Freeze or version reference evaluators.

5. Identify candidate improvement opportunities.

6. Generate candidate structural modifications.

7. Reject contract-incompatible candidates.

8. Reject policy-ineligible candidates.

9. Select applicable Scoring Trees.

10. Evaluate candidate quality, cost, and risk.

11. Meta-score evaluator applicability.

12. Select independent validation mechanisms.

13. Test candidates against reference baselines.

14. Search for counter-evidence.

15. Evaluate long-tail and distribution-shift behavior.

16. Estimate net structural benefit.

17. Reject candidates with unacceptable regressions.

18. Submit eligible candidates for authorization.

19. Deploy authorized candidates in controlled scope.

20. Monitor external outcomes.

21. Promote, revise, or roll back as required.

22. Record all evidence and evaluator versions.

23. Identify reusable Scoring Tree patterns.

24. Propose CCC extraction or refinement.

25. Validate CCC changes separately.

26. Update structural registries through
    governed promotion procedures.

27. Repeat only within authorized budgets
    and recursion limits.

28. Return validated architecture, trace,
    and structural learning record.
```

The algorithm is conceptual.

A production implementation would require explicit concurrency, transaction, authorization, and failure-recovery semantics.

---

## 14. Illustrative Improvement Campaign

### 14.1 Initial Condition

Suppose the baseline system uses one general-purpose LLM for code localization and modification.

### 14.2 Candidate Modification

The RSI engine proposes:

**Candidate A:** Introduce MDT-assisted localization before code generation.

### 14.3 Expected Benefit

The candidate may reduce irrelevant context and improve localization accuracy.

This is a hypothesis, not an observed result.

### 14.4 Evaluation

The Scoring Forest examines:

- Task correctness;
- Context sufficiency;
- Latency;
- Compute cost;
- Regression risk;
- Transferability.

### 14.5 Independent Validation

The candidate is evaluated on held-out software tasks.

### 14.6 Possible Outcomes

**Outcome A — Validated Improvement**

The candidate improves relevant metrics without unacceptable regressions.

It may proceed to authorized deployment.

**Outcome B — Mixed Results**

The candidate improves large-project localization but degrades small-task latency.

It may be specialized to an appropriate Perspective.

**Outcome C — Regression**

The candidate introduces unacceptable failures.

It is rejected or revised.

### 14.7 Recursive Opportunity

Evidence from the campaign may suggest:

- Better localization selection rules;
- A specialized dispatch branch;
- A reusable CCC;
- A revised evaluator.

### 14.8 Evaluation Separation

Any proposed evaluator revision must undergo a separate validation process.

---

## 15. Failure Modes and Defensive Measures

### 15.1 Reward Hacking

A candidate exploits the scoring mechanism.

**Defense:** Independent outcome validation.

### 15.2 Evaluator Capture

A candidate modifies the evaluator that judges it.

**Defense:** Separate evaluator governance and reference baselines.

### 15.3 Structural Overfitting

A candidate performs well on development tasks but poorly elsewhere.

**Defense:** Held-out tasks and transfer testing.

### 15.4 Hidden Regression

A candidate degrades rare but important cases.

**Defense:** Long-tail testing and counter-evidence.

### 15.5 Excessive Complexity

A candidate adds more components than its benefits justify.

**Defense:** Lifecycle cost accounting.

### 15.6 Recursive Instability

Repeated modifications produce unpredictable interactions.

**Defense:** Bounded recursion and staged promotion.

### 15.7 Contract Drift

Components change behavior without updating declared interfaces.

**Defense:** Versioned conformance testing.

### 15.8 Policy Bypass

A candidate attempts an unauthorized action.

**Defense:** Independent authorization enforcement.

### 15.9 Correlated Evaluation

Multiple evaluators share the same weaknesses.

**Defense:** Evaluator lineage analysis.

### 15.10 Rollback Failure

A promoted change cannot be reliably reversed.

**Defense:** Predefined rollback plans and controlled deployment scope.

---

## 16. Experimental Validation Design

### 16.1 Research Questions

**RQ-001:** Can Rich Evaluators improve Structural RSI promotion decisions?

**RQ-002:** Does Meta-Scoring improve evaluator selection?

**RQ-003:** Can counter-evidence reduce harmful structural promotions?

**RQ-004:** Does separate evaluator governance reduce evaluation drift?

**RQ-005:** Can recursive CCC distillation improve evaluation reuse?

**RQ-006:** Can Scoring-Guided Structural RSI improve cost-adjusted task outcomes?

### 16.2 Baselines

Proposed baselines include:

1. No structural self-improvement;
2. Single-reward RSI;
3. Multi-metric RSI with fixed aggregation;
4. Scoring Forest RSI without Meta-Scoring;
5. Scoring Forest RSI without independent validation;
6. Full Scoring-Guided Structural RSI.

### 16.3 Experimental Campaigns

**Campaign A — Localization Improvement**

Compare alternative Localization Engines.

**Campaign B — Per-Node Engine Selection**

Evaluate specialist versus general-purpose engine configurations.

**Campaign C — Scoring Structure Improvement**

Test revised Scoring Trees and learned evaluators.

**Campaign D — Counter-Evidence**

Introduce hidden regression cases.

**Campaign E — Evaluator Drift**

Measure the ability to detect misleading evaluator updates.

**Campaign F — Recursive CCC Growth**

Evaluate reusable scoring structures across multiple campaigns.

### 16.4 Metrics

| Metric | Purpose |
|---|---|
| Task Success Rate | External task performance |
| Promotion Precision | Fraction of promoted changes that satisfy defined improvement criteria |
| Harmful Promotion Rate | Frequency of unacceptable promoted regressions |
| Cost-Adjusted Utility | Benefit relative to total computational cost |
| Evaluator Drift Detection | Detection of unreliable evaluation changes |
| Counter-Evidence Detection | Identification of hidden failures |
| Structural Reuse | Reuse of validated components |
| Rollback Reliability | Recovery from unsuccessful promotions |
| Constraint Compliance | Preservation of mandatory requirements |
| Longitudinal Improvement | Sustained benefits over repeated campaigns |

### 16.5 Controlled Variables

Experiments should control for:

- Candidate-generation budget;
- Model capabilities;
- Evaluation budget;
- Benchmark exposure;
- Task difficulty;
- Available tools;
- Human intervention;
- Promotion thresholds.

### 16.6 Validation Status

This case study defines a proposed experimental framework.

No experiments are reported.

No quantitative performance claims are made.

---

## 17. Expected Benefits and Tradeoffs

### 17.1 Potential Benefits

Scoring-Guided Structural RSI may provide:

- More reliable improvement selection;
- Better evaluation coverage;
- Reduced reward exploitation;
- More explicit structural evidence;
- Reusable CCCs;
- Improved governance;
- Better control of recursive modification.

### 17.2 Potential Costs

The architecture introduces:

- Additional evaluation expense;
- Control Plane complexity;
- Contract maintenance;
- Evidence storage;
- Independent validation overhead;
- Slower promotion cycles.

### 17.3 When It May Be Useful

The architecture may be particularly useful when:

- Structural changes have broad effects;
- Evaluation is multidimensional;
- Tasks are heterogeneous;
- Regressions are costly;
- Components evolve frequently;
- Independent validation is important.

### 17.4 When Simpler Methods May Be Preferable

Simpler optimization may remain preferable when:

- The modification space is narrow;
- The reward is reliable;
- Tasks are stable;
- Risks are low;
- Evaluation overhead outweighs expected gains.

---

## 18. Relationship to the UCPSF Research Series

### UCPSF-001

Generalized Scoring Intelligence motivates richer evaluation.

### UCPSF-002

The three Scoring Operator families support parameter, branch, and learned-evaluator modifications.

### UCPSF-003

Scoring Trees, Forests, and Unaligned AND Folding organize evaluation structures.

### UCPSF-004

Recursive CCC distillation supports reusable evaluator growth.

### UCPSF-005

Perspective-Aware Meta-Scoring guides evaluator selection and optimization.

### UCPSF-006

Hybrid Localization and Per-Node Intelligence define a broad structural modification space.

### UCPSF-007

The Universal Control Plane governs execution, evaluation, authorization, and structural promotion.

### UCPSF-008

Open-Ended Scoring Intelligence provides the long-term research direction.

### CASE-001

Scoring-Controlled AI Relay examines evaluation-guided workflow decisions.

### CASE-003

Hybrid Localization and Per-Node Selection examines adaptive composition of heterogeneous intelligence engines.

---

## 19. Conclusion

Structural RSI expands the scope of recursive improvement from model parameters and prompts to the architecture of intelligence systems.

This expansion creates a difficult evaluation problem.

A candidate structural modification may improve one metric while degrading another, exploit an evaluator, increase system complexity, or introduce hidden regressions.

This case study proposes Scoring-Guided Structural RSI as a controlled approach to such modifications.

The architecture combines:

1. Rich Scoring Trees and Forests;
2. Perspective-Aware Optimization;
3. Meta-Scoring Intelligence;
4. Independent validation;
5. Counter-evidence;
6. Contract-first structural composition;
7. Governed promotion and rollback;
8. Recursive CCC distillation.

Its central proposition is:

> **The direction and reliability of Structural RSI depend not only on the system's ability to generate better structures, but also on the quality, independence, and governance of the intelligence used to evaluate those structures.**

A second principle follows:

> **An intelligence system must not establish its own improvement merely by changing the evaluation criteria under which improvement is measured.**

The proposed framework does not guarantee beneficial recursive improvement.

It provides an architectural research direction for making structural modification more measurable, auditable, and governable.

Future work should test whether richer evaluation and controlled promotion improve the long-term reliability and cost-adjusted performance of Structural RSI systems.

---

## Suggested Figure Placement

### Fig-007 — Universal Control Plane and Structural RSI

**File:** `../figures/Fig-007-Universal-Control-Plane-and-Structural-RSI.png`

**Suggested insertion:** After Section 4.5.

**Purpose:** Illustrate the complete Scoring-Guided Structural RSI architecture, including candidate generation, evaluation, independent validation, governance, and promotion.

### Fig-005 — Perspective Optimization and Meta-Scoring

**File:** `../figures/Fig-005-Perspective-Optimization-and-Meta-Scoring.png`

**Suggested insertion:** After Section 9.6.

**Purpose:** Illustrate Perspective-dependent evaluator selection and Meta-Scoring.

### Fig-004 — Unaligned AND Folding and CCC Distillation

**File:** `../figures/Fig-004-Unaligned-AND-Folding-and-CCC-Distillation.png`

**Suggested insertion:** After Section 11.9.

**Purpose:** Illustrate recursive extraction and refinement of reusable Scoring CCCs from repeated RSI campaigns.

---

## Research Lineage

### Structural Recursive Self-Improvement

https://github.com/sizhet/Structural-Recursive-Self-Improvement

### Generalized Structural Trigger and Computational Growth Intelligence

https://github.com/sizhet/Generalized-Structural-Trigger-and-Computational-Growth-Intelligence

### Principle Intelligence and Open Structural Learning

https://github.com/sizhet/Principle-Intelligence-and-Open-Structural-Learning

### Portable Intelligence Runtime Pieces and Units

https://github.com/sizhet/Portable-Intelligence-Runtime-Pieces-and-Units

### Pre-AGI AI Action Governance

https://github.com/sizhet/Pre-AGI-AI-Action-Governance

These repositories establish conceptual continuity within the Structural Intelligence research program.

They are not presented as independent empirical validation of the proposed architecture.

---

## Citation

Suggested citation prior to DOI assignment:

Tan, S., & GPT-Obot. (2026). *CASE-002: Scoring-Guided Structural RSI*. Universal Control Planes and Scoring Tree/Forest/Folding for Structural Intelligence, Version 1.0.0.

Repository:

https://github.com/sizhet/Universal-Control-Planes-and-Scoring-Folding

DOI: 10.5281/zenodo.23486273

---

## License

Copyright © 2026 Sizhe Tan & GPT-Obot.

Licensed under the Apache License, Version 2.0.

---

**Document:** CASE-002  
**Research Series:** Universal Control Planes and Scoring Tree/Forest/Folding  
**Status:** Conceptual Case Study and Proposed Validation Design  
**Version:** 1.0.0
