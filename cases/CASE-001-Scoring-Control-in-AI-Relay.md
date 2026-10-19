
# CASE-001 — Scoring Control in AI Relay

**Subtitle:** Perspective-Aware Evaluation, Adaptive Relay Decisions, and Scoring Forest Governance in Multi-Stage AI Workflows

**Authors:** Sizhe Tan & GPT-Obot  
**Project:** Universal Control Planes and Scoring Tree/Forest/Folding for Structural Intelligence (UCPSF)  
**Document ID:** CASE-001  
**Version:** 1.0.0  
**Date:** October 15, 2026  
**Status:** Conceptual Case Study and Proposed Validation Design  
**License:** Apache-2.0

---

## Abstract

AI Relay systems distribute complex tasks across multiple intelligence engines, agents, tools, and evaluation stages.

A typical Relay workflow must repeatedly decide whether to accept an intermediate result, continue computation, retry a failed operation, invoke a specialist, delegate to another engine, or terminate.

These decisions are often implemented through fixed thresholds, static routing rules, confidence estimates, or a single learned evaluator.

Such mechanisms can be effective in well-defined environments, but may become insufficient when tasks vary in complexity, computational cost, uncertainty, risk, and required expertise.

This case study proposes **Scoring-Controlled AI Relay**, a conceptual architecture in which a Universal Control Plane coordinates multi-stage execution through Perspective-Aware Scoring Trees, Scoring Forests, Meta-Scoring Intelligence, and explicit governance constraints.

The architecture treats Relay decisions as first-class structural decision objects rather than incidental workflow conditions.

It introduces a layered evaluation process in which low-cost scoring handles routine cases, richer evaluation is invoked when justified, and independent validation is required for designated high-risk outcomes.

Repeated Relay execution may also provide evidence for extracting reusable Common Concept Cores (CCCs), improving dispatch structures, and learning more effective evaluation policies.

The study develops an illustrative software-engineering Relay scenario, a proposed execution algorithm, failure-mode analysis, and an experimental validation framework.

No empirical performance improvement is claimed.

The central research hypothesis is that Scoring-Controlled AI Relay may improve the quality, cost efficiency, and governability of heterogeneous AI workflows compared with fixed evaluation and routing strategies under appropriately selected workloads.

**Keywords:** AI Relay, Universal Control Plane, Scoring Tree, Scoring Forest, Perspective-Aware Optimization, Meta-Scoring, Hybrid Intelligence, Structural Folding, Common Concept Core, Adaptive Evaluation, Multi-Agent Systems, Structural Intelligence

---

## 1. Introduction

### 1.1 AI Relay as a Composite Intelligence System

AI Relay describes a class of workflows in which multiple intelligence components contribute sequentially or collaboratively to a task.

A Relay may involve:

- General-purpose LLMs;
- Specialized language models;
- Retrieval systems;
- Code-generation engines;
- ANN scoring models;
- Principle Engines;
- Symbolic validators;
- External tools;
- Human review.

The system must coordinate both computation and evaluation.

### 1.2 The Relay Control Problem

At each stage, a Relay system may need to decide:

1. Is the current result sufficient?
2. Should computation continue?
3. Should the task be delegated?
4. Which engine should be invoked next?
5. Is a retry worthwhile?
6. Is additional evaluation justified?
7. Should the workflow stop?
8. Is external action authorized?

These decisions directly affect task quality, cost, latency, and reliability.

### 1.3 Limitations of Fixed Relay Control

A fixed Relay policy may use rules such as:

```text
If confidence > threshold:
    Accept result
Else:
    Invoke another model
```

This may be useful for routine tasks.

However, confidence alone may not adequately represent:

- Task-specific risk;
- Missing evidence;
- Evaluation uncertainty;
- Domain complexity;
- Cost of additional computation;
- Policy constraints;
- Long-tail failure modes.

### 1.4 Proposed Research Direction

We propose replacing a single fixed decision criterion with a structured, Perspective-aware evaluation process.

The objective is not to eliminate simple rules.

It is to determine when simple rules are sufficient and when richer control is justified.

---

## 2. Case Scenario — Multi-Stage Software Engineering Relay

### 2.1 Task Definition

Consider a hypothetical AI Relay system responsible for modifying an existing software project.

A task may require:

- Understanding a change request;
- Locating relevant source files;
- Planning modifications;
- Generating code;
- Running tests;
- Evaluating results;
- Producing an implementation report.

### 2.2 Candidate Engines

The system contains the following conceptual components.

**Engine A — Task Interpreter**

Converts the user request into structured requirements.

**Engine B — Structural Localizer**

Identifies relevant files, dependencies, and Calling Graph relationships.

**Engine C — Code Generator**

Produces candidate modifications.

**Engine D — Test and Verification Engine**

Runs available tests and static checks.

**Engine E — Risk Evaluator**

Assesses possible regressions, policy violations, and unresolved uncertainty.

**Engine F — Review or Escalation Engine**

Performs additional analysis when ordinary evaluation is insufficient.

### 2.3 Baseline Relay

A conventional fixed pipeline might execute:

```text
User Request
     |
     v
Task Interpretation
     |
     v
File Retrieval
     |
     v
Code Generation
     |
     v
Run Tests
     |
     v
Pass / Fail
     |
     v
Accept / Retry
```

This workflow is simple and may be effective.

However, it does not explicitly evaluate whether:

- The retrieved context is sufficient;
- The selected engine is appropriate;
- The tests cover the relevant failure modes;
- Additional verification is worth its cost;
- The task requires a different Relay path.

### 2.4 Proposed Scoring-Controlled Relay

The proposed architecture adds structured evaluation and adaptive control.

```text
User Request
     |
     v
Perspective / Policy Resolution
     |
     v
Hybrid Localization
     |
     v
Task and Context Scoring
     |
     v
Engine Selection
     |
     v
Candidate Generation
     |
     v
Scoring Forest Evaluation
     |
     +----> Accept
     |
     +----> Retry
     |
     +----> Delegate
     |
     +----> Rich Validation
     |
     +----> Stop / Escalate
     |
     v
Evidence and Outcome Recording
```

The branches represent alternative control decisions rather than mandatory execution stages.

---

## 3. Perspective-Aware Relay Control

### 3.1 Perspective Definition

Following UCPSF-005, define:

\[
P=(G,C,B,T,R)
\]

where:

- \(G\): Task goals;
- \(C\): Context and constraints;
- \(B\): Resource budget;
- \(T\): Time horizon;
- \(R\): Risk preferences.

### 3.2 Example Perspectives

The same software task may be evaluated differently under different Perspectives.

| Perspective | Primary Concerns |
|---|---|
| Rapid Prototype | Speed, low cost, basic correctness |
| Production Engineering | Reliability, maintainability, test coverage |
| Security-Sensitive Change | Security constraints, independent validation |
| Exploratory Refactoring | Structural improvement, long-term maintainability |
| Emergency Repair | Time sensitivity, bounded risk, rollback readiness |

### 3.3 Perspective-Dependent Evaluation

A rapid prototype may use a lightweight evaluation path.

A security-sensitive modification may require:

- Additional static analysis;
- Dependency review;
- Independent security checks;
- Explicit authorization.

### 3.4 Perspective Is Not Permission

Perspective changes evaluation priorities.

It does not automatically override mandatory security, privacy, or deployment policies.

---

## 4. Scoring Tree for Relay Decisions

### 4.1 Object-Level Evaluation

A candidate software modification may be evaluated through multiple dimensions.

```text
Candidate Modification
        |
        v
     Scoring Tree
        |
        +--> Functional Correctness
        |
        +--> Test Evidence
        |
        +--> Context Sufficiency
        |
        +--> Maintainability
        |
        +--> Security Risk
        |
        +--> Resource Cost
        |
        v
Relay Decision Recommendation
```

### 4.2 Functional Correctness

Evaluate whether the modification satisfies the stated requirements.

### 4.3 Test Evidence

Evaluate:

- Test pass/fail outcomes;
- Test coverage relevance;
- Missing test scenarios;
- Regression evidence.

### 4.4 Context Sufficiency

Determine whether the system has identified enough relevant source context to support the modification.

### 4.5 Maintainability

Consider:

- Code complexity;
- Interface compatibility;
- Duplication;
- Readability;
- Architectural consistency.

### 4.6 Security Risk

Assess potential vulnerabilities and policy-sensitive changes.

### 4.7 Resource Cost

Estimate:

- Additional model calls;
- Test execution cost;
- Expected retry cost;
- Review overhead;
- Latency.

### 4.8 Constraint Semantics

Mandatory constraints should not be treated as compensable score dimensions.

For example, a candidate that violates a required security policy should not be accepted merely because it scores highly on performance.

---

## 5. Relay Decision Operators

### 5.1 Decision Set

At each Relay stage, the Control Plane may choose from:

\[
A=
\{
\text{ACCEPT},
\text{CONTINUE},
\text{RETRY},
\text{DELEGATE},
\text{ESCALATE},
\text{STOP}
\}
\]

### 5.2 ACCEPT

Accept the current result when evidence satisfies the required criteria.

Acceptance of a computational result does not necessarily authorize deployment.

### 5.3 CONTINUE

Proceed to the next planned stage.

### 5.4 RETRY

Repeat an operation when another attempt has plausible expected value.

Retries should be bounded.

### 5.5 DELEGATE

Transfer the task to a more appropriate engine.

### 5.6 ESCALATE

Invoke richer evaluation, specialized review, or human intervention.

### 5.7 STOP

Terminate the workflow when:

- The task is complete;
- Further computation is not justified;
- Resources are exhausted;
- Mandatory constraints cannot be satisfied;
- Required authorization is unavailable.

### 5.8 Decision Preservation

Structural Folding should preserve the conditions under which different Relay decisions are appropriate.

A compressed Relay policy that incorrectly merges ACCEPT and ESCALATE behavior may be unsafe.

---

## 6. Scoring Forest for Multi-Perspective Relay Evaluation

### 6.1 Why a Forest?

A single Scoring Tree may not capture every relevant Perspective.

A Scoring Forest allows multiple specialized evaluation structures.

### 6.2 Candidate Forest

\[
\mathcal{F}_S=
\{
T_{\mathrm{quality}},
T_{\mathrm{risk}},
T_{\mathrm{cost}},
T_{\mathrm{context}},
T_{\mathrm{policy}}
\}
\]

### 6.3 Quality Tree

Evaluates functional correctness and maintainability.

### 6.4 Risk Tree

Evaluates potential failures and their consequences.

### 6.5 Cost Tree

Estimates additional computational investment.

### 6.6 Context Tree

Evaluates localization quality and missing evidence.

### 6.7 Policy Tree

Identifies applicable governance constraints.

Policy enforcement should remain an independent authorization function, even when policy-related evaluation information is represented within a Scoring Tree.

### 6.8 Dynamic Forest Selection

The Control Plane need not invoke every tree for every task.

It may select a subset based on:

- Perspective;
- Task complexity;
- Risk;
- Available budget;
- Validation requirements.

---

## 7. Meta-Scoring for Evaluator Selection

### 7.1 The Evaluator Selection Problem

The Relay system may have several possible evaluators.

Some are cheap and approximate.

Others are expensive and more comprehensive.

### 7.2 Candidate Evaluators

For example:

- ANN quality scorer;
- LLM-based code reviewer;
- Static analyzer;
- Test runner;
- Security checker;
- Rich Scoring Forest.

### 7.3 Meta-Scoring

A meta-evaluator estimates the suitability of each evaluation mechanism.

\[
M(S_i\mid P,E)
\]

where:

- \(S_i\): Candidate evaluator;
- \(P\): Perspective;
- \(E\): Evidence.

### 7.4 Evaluation Dimensions

Potential dimensions include:

- Expected accuracy;
- Calibration;
- Cost;
- Latency;
- Robustness;
- Applicability;
- Independence;
- Constraint coverage.

### 7.5 Example

A low-risk formatting change may justify lightweight checks.

A security-sensitive dependency modification may justify a more comprehensive evaluation process.

### 7.6 Independent Validation

An evaluator should not certify its own superiority solely through its internal scores.

Reference tests and independent evidence are required for evaluator promotion.

---

## 8. Adaptive Evaluation Depth

### 8.1 Evaluation Cost

Rich evaluation can improve confidence but consumes resources.

### 8.2 Candidate Levels

**Level 0 — Basic Checks**

Syntax, simple rules, or fixed thresholds.

**Level 1 — Specialized Scoring**

ANN quality estimation or task-specific metrics.

**Level 2 — Structured Evaluation**

A multi-dimensional Scoring Tree.

**Level 3 — Scoring Forest**

Multiple evaluation Perspectives.

**Level 4 — Independent Validation**

Additional testing, security review, or human escalation.

### 8.3 Adaptive Escalation

```text
Candidate Result
       |
       v
Low-Cost Evaluation
       |
       v
Risk / Uncertainty Check
       |
       +-- Sufficient --> Accept
       |
       +-- Insufficient
                |
                v
         Rich Scoring Tree
                |
                v
         Independent Validation
                |
                v
         Accept / Revise / Stop
```

### 8.4 Value of Additional Evaluation

A conceptual criterion is:

\[
VOI(a\mid P)
=
\mathbb{E}[U_{\mathrm{after}}]
-
U_{\mathrm{before}}
-
C(a)
\]

where \(a\) is an additional evaluation action.

This assumes utility and cost are expressed in compatible units.

### 8.5 Stopping Rule

Additional evaluation should stop when expected benefits no longer justify costs, unless mandatory validation requirements remain unsatisfied.

---

## 9. Hybrid Localization and Per-Node Intelligence

### 9.1 Localization Engines

The Relay may use:

- Semantic retrieval;
- Transformer-based context processing;
- MDT localization;
- UTN structural references;
- CCC matching;
- Calling Graph search.

### 9.2 Per-Node Engines

The Relay may invoke:

- General-purpose LLMs;
- Specialized coding models;
- ANN scorers;
- Principle Engines;
- Symbolic validators;
- Test and optimization tools.

### 9.3 Dynamic Composition

A task may require different engine combinations.

For example:

```text
Task Interpretation
        |
        v
MDT / Calling Graph Localization
        |
        v
Specialized Coding Engine
        |
        v
Test and Verification Engine
        |
        v
Scoring Forest
        |
        v
Relay Control Decision
```

### 9.4 Adaptive Coupling

Some tasks may be handled efficiently by one integrated model.

Others may justify modular execution.

The Control Plane should evaluate the tradeoff rather than assuming that more components are always better.

---

## 10. Universal Control Plane Responsibilities

### 10.1 Perspective Management

Resolve task goals, budgets, risk, and time constraints.

### 10.2 Contract Management

Validate compatibility among engines and scoring structures.

### 10.3 Dispatch

Select the next computational stage.

### 10.4 Scoring

Evaluate candidate results.

### 10.5 Meta-Scoring

Evaluate scoring mechanisms.

### 10.6 Resource Management

Track compute, latency, and retry budgets.

### 10.7 Evidence Management

Record outcomes and evaluator versions.

### 10.8 Governance

Enforce authorization and mandatory constraints.

### 10.9 Structural Learning

Propose revisions to Relay structures and scoring mechanisms.

### 10.10 Lifecycle Management

Validate, promote, specialize, retire, or roll back structural changes.

---

## 11. Proposed Scoring-Controlled Relay Algorithm

```text
Algorithm: Scoring-Controlled-AI-Relay

Input:
    Task X
    Perspective P
    Localization Registry L
    Intelligence Registry I
    Scoring Forest S
    Contract Registry C
    Evidence Repository E
    Resource Budget B
    Governance Rules G

Output:
    Task Result Y
    Relay Trace T
    Optional Structural Learning Proposal R

1. Resolve Perspective P.

2. Determine mandatory constraints G.

3. Localize task-relevant context.

4. Evaluate context sufficiency.

5. Select compatible intelligence engines.

6. Execute selected engine.

7. Collect candidate output and evidence.

8. Select applicable Scoring Trees.

9. Evaluate candidate quality, cost, and risk.

10. Check mandatory constraints.

11. Estimate uncertainty and evaluation sufficiency.

12. Choose Relay decision:

       ACCEPT
       CONTINUE
       RETRY
       DELEGATE
       ESCALATE
       STOP

13. If RETRY:
        Enforce retry limits.
        Update task context.
        Return to Step 6.

14. If DELEGATE:
        Select an alternative engine.
        Return to Step 6.

15. If ESCALATE:
        Invoke richer or independent evaluation.
        Reassess decision.

16. If CONTINUE:
        Advance to the next task stage.

17. If ACCEPT:
        Produce an accepted computational result.

18. Before external action:
        Apply independent authorization.

19. Record execution trace and evidence.

20. Detect potential structural improvements.

21. Generate candidate CCC or Relay revisions.

22. Submit revisions to independent validation.

23. Return Y, T, and optional proposal R.
```

This is a conceptual algorithm.

A production implementation would require explicit loop bounds, concurrency control, error recovery, and authorization enforcement.

---

## 12. Scoring Folding in Repeated Relay Workflows

### 12.1 Repeated Evaluation Patterns

Different Relay tasks may repeatedly use similar evaluation structures.

For example:

```text
Candidate Output
      |
      v
Quality Check
      |
      v
Risk Check
      |
      v
Confidence Check
      |
      v
Accept / Escalate
```

### 12.2 Candidate CCC Extraction

Repeated patterns may provide evidence for a reusable Relay Scoring CCC.

### 12.3 Structural CCC

A Structural CCC may encode the common organization of evaluation stages.

### 12.4 Behavioral CCC

A Behavioral CCC may encode recurring decision behavior under specified conditions.

### 12.5 Unaligned AND Folding

Different Relay workflows may implement equivalent evaluation functions through different structures.

Unaligned AND Folding may identify candidate commonality across these workflows.

### 12.6 Specialized Delta

Task-specific differences should remain available.

For example:

- Security review;
- Performance testing;
- Database migration checks;
- API compatibility verification.

### 12.7 Recursive Distillation

As new Relay evidence accumulates, candidate CCCs may be:

- Reinforced;
- Refined;
- Specialized;
- Split;
- Rejected;
- Promoted.

### 12.8 Validation Requirement

A folded Relay evaluator must preserve decision-relevant behavior, particularly escalation and rejection conditions.

---

## 13. Evidence-Driven Relay Learning

### 13.1 Execution Evidence

The Relay should record:

- Task identity;
- Perspective;
- Selected engines;
- Scoring Tree versions;
- Intermediate decisions;
- Resource consumption;
- Test outcomes;
- External results;
- Failures and counter-evidence.

### 13.2 Evaluator Performance

Evidence may reveal:

- A scorer that frequently misses regressions;
- An unnecessary evaluation stage;
- A useful specialized engine;
- A missing risk branch;
- A recurring delegation pattern.

### 13.3 Structural Revision

Such evidence may motivate changes to:

- Scoring weights;
- Branching logic;
- Engine selection;
- CCC applicability;
- Escalation conditions.

### 13.4 Controlled Promotion

Proposed revisions should be independently validated before deployment.

### 13.5 Avoiding Evaluator Drift

A Relay system should not declare improvement solely because its revised scorer produces higher scores.

External task outcomes and reference evaluations remain necessary.

---

## 14. Failure Modes

### 14.1 Premature Acceptance

The Relay accepts an insufficient result.

**Possible mitigation:** Context sufficiency checks and risk-sensitive escalation.

### 14.2 Excessive Retry

The Relay repeats computation without meaningful progress.

**Possible mitigation:** Retry budgets and expected improvement estimates.

### 14.3 Wrong Engine Selection

The Relay invokes an unsuitable specialist.

**Possible mitigation:** Capability contracts and Meta-Scoring.

### 14.4 Inadequate Context

The selected engine lacks relevant information.

**Possible mitigation:** Localization validation and additional retrieval.

### 14.5 Correlated Evaluators

Multiple scoring mechanisms share the same underlying failure.

**Possible mitigation:** Evaluator lineage and independent validation.

### 14.6 Over-Folding

A compressed scoring structure removes rare but important evaluation branches.

**Possible mitigation:** Counter-evidence testing and preservation of Specialized Delta.

### 14.7 Evaluator Drift

A revised scoring mechanism becomes less aligned with external outcomes.

**Possible mitigation:** Reference baselines and rollback.

### 14.8 Policy Bypass

A high-scoring result is used to justify an unauthorized action.

**Possible mitigation:** Independent authorization enforcement.

### 14.9 Structural Overengineering

The Relay becomes more expensive than simpler alternatives.

**Possible mitigation:** Cost-aware evaluation and comparison with fixed pipelines.

---

## 15. Experimental Validation Design

### 15.1 Research Questions

**RQ-001:** Can Scoring-Controlled Relay improve task outcomes compared with fixed routing?

**RQ-002:** Can adaptive evaluation reduce unnecessary computation?

**RQ-003:** Does Meta-Scoring improve evaluator selection?

**RQ-004:** Can reusable Relay CCCs preserve decision quality while reducing repeated evaluation cost?

**RQ-005:** Do independent validation and counter-evidence reduce harmful structural revisions?

### 15.2 Baselines

Proposed baselines include:

1. Fixed Relay pipeline;
2. Confidence-threshold routing;
3. Single learned evaluator;
4. Static Scoring Tree;
5. Static Scoring Forest;
6. Adaptive Relay without Meta-Scoring;
7. Full Scoring-Controlled Relay.

### 15.3 Experimental Tasks

A future benchmark may include:

- Small code fixes;
- Multi-file refactoring;
- API changes;
- Dependency updates;
- Performance optimization;
- Security-sensitive modifications.

### 15.4 Controlled Variables

Experiments should control for:

- Model capabilities;
- Tool access;
- Available context;
- Total compute budget;
- Test availability;
- Task difficulty;
- Human intervention;
- Evaluation leakage.

### 15.5 Metrics

| Metric | Purpose |
|---|---|
| Task Success Rate | Correct completion of requested work |
| Regression Rate | Unintended software failures |
| Evaluation Cost | Resources consumed by scoring |
| Total Compute Cost | End-to-end computational expense |
| Latency | Time to completion |
| Relay Decision Accuracy | Quality of accept, retry, delegate, and stop decisions |
| Escalation Precision | Appropriateness of rich evaluation |
| Context Sufficiency | Adequacy of localized information |
| Constraint Compliance | Preservation of mandatory requirements |
| Structural Reuse | Reuse of validated Relay CCCs |

### 15.6 Hypotheses

**H1:** Scoring-Controlled Relay can improve cost-adjusted task quality on heterogeneous workloads.

**H2:** Adaptive evaluation depth can reduce unnecessary scoring cost while preserving required quality.

**H3:** Meta-Scoring can improve evaluator selection under changing Perspectives.

**H4:** CCC-based structural reuse can reduce repeated evaluation engineering effort.

**H5:** Independent validation can reduce the promotion of ineffective Relay control changes.

### 15.7 Validation Status

This case study is conceptual.

No experiments have been executed as part of this document.

No quantitative performance claims are made.

---

## 16. Expected Benefits and Tradeoffs

### 16.1 Potential Benefits

The proposed architecture may provide:

- More adaptive Relay decisions;
- Better Perspective alignment;
- Improved evaluation resource allocation;
- Reusable scoring structures;
- More explicit evidence;
- Better governance;
- Controlled structural learning.

### 16.2 Potential Costs

The architecture introduces:

- Control Plane overhead;
- Additional evaluation complexity;
- Contract maintenance;
- Evidence storage;
- Validation expense;
- More complicated debugging.

### 16.3 When It May Be Useful

The architecture may be most useful for:

- Heterogeneous tasks;
- Multi-stage workflows;
- High-value decisions;
- Repeated evaluation patterns;
- Tasks requiring independent validation;
- Systems with multiple specialized engines.

### 16.4 When Simpler Approaches May Be Better

A fixed pipeline may remain preferable when:

- Tasks are highly uniform;
- Evaluation criteria are stable;
- Risk is low;
- Computational budgets are tight;
- Modular overhead outweighs benefits.

---

## 17. Relationship to the UCPSF Framework

This case study illustrates how the core UCPSF concepts may interact in an AI Relay environment.

**UCPSF-001**

Generalized Scoring Intelligence provides the conceptual foundation.

**UCPSF-002**

Scoring Operators support parameter adjustment, branching decisions, and learned evaluation.

**UCPSF-003**

Scoring Trees and Forests organize heterogeneous Relay evaluators.

**UCPSF-004**

Recursive CCC distillation supports reusable evaluation structures.

**UCPSF-005**

Perspective-Aware Meta-Scoring guides evaluator selection and computational investment.

**UCPSF-006**

Hybrid Localization and Per-Node Intelligence support dynamic engine composition.

**UCPSF-007**

The Universal Control Plane coordinates execution, evaluation, governance, and structural evolution.

**UCPSF-008**

Open-Ended Scoring Intelligence provides the long-term research direction.

---

## 18. Conclusion

AI Relay systems require repeated decisions about computation, delegation, evaluation, escalation, and termination.

These decisions can be implemented through fixed rules or learned evaluators, but heterogeneous workflows may benefit from more explicit structural control.

This case study proposes Scoring-Controlled AI Relay as an application of the UCPSF framework.

The proposed architecture integrates:

1. Perspective-Aware evaluation;
2. Scoring Trees and Forests;
3. Meta-Scoring;
4. Adaptive evaluation depth;
5. Hybrid Localization and Per-Node Intelligence;
6. CCC extraction and structural reuse;
7. Independent validation and governance.

The central proposition is:

> **In a complex AI Relay system, scoring should not merely judge the final output; it should guide the selection, continuation, delegation, escalation, and evolution of the entire computational workflow.**

This proposition requires empirical validation.

The proposed architecture should be compared against simpler fixed pipelines and adaptive routing baselines under controlled computational budgets.

If validated, Scoring-Controlled Relay may provide a practical application of Generalized Scoring Intelligence and Universal Control Plane architecture.

---

## Suggested Figure Placement

### Fig-001 — Universal Control Plane Grand Map

**File:** `../figures/Fig-001-Universal-Control-Plane-Grand-Map.png`

**Suggested insertion:** After Section 10.

**Purpose:** Illustrate the relationship between AI Relay execution, Scoring Forest evaluation, Meta-Scoring, and Control Plane governance.

### Fig-005 — Perspective Optimization and Meta-Scoring

**File:** `../figures/Fig-005-Perspective-Optimization-and-Meta-Scoring.png`

**Suggested insertion:** After Section 7.

**Purpose:** Illustrate Perspective-aware evaluator selection and adaptive evaluation depth.

---

## Citation

Suggested citation prior to DOI assignment:

Tan, S., & GPT-Obot. (2026). *CASE-001: Scoring Control in AI Relay*. Universal Control Planes and Scoring Tree/Forest/Folding for Structural Intelligence, Version 1.0.0.

Repository:

https://github.com/sizhet/Universal-Control-Planes-and-Scoring-Folding

DOI: To be assigned after the initial archived release.

---

## License

Copyright © 2026 Sizhe Tan & GPT-Obot.

Licensed under the Apache License, Version 2.0.

---

**Document:** CASE-001  
**Research Series:** Universal Control Planes and Scoring Tree/Forest/Folding  
**Status:** Conceptual Case Study and Proposed Validation Design  
**Version:** 1.0.0
