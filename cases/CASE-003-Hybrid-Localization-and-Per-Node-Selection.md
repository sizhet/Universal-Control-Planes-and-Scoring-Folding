
# CASE-003 — Hybrid Localization and Per-Node Selection

**Subtitle:** Perspective-Aware Composition of Heterogeneous Localization Engines and Per-Node Intelligence under a Universal Control Plane

**Authors:** Sizhe Tan & GPT-Obot  
**Project:** Universal Control Planes and Scoring Tree/Forest/Folding for Structural Intelligence (UCPSF)  
**Document ID:** CASE-003  
**Version:** 1.0.0  
**Date:** October 15, 2026  
**Status:** Conceptual Case Study and Proposed Validation Design  
**License:** Apache-2.0

---

## Abstract

Transformer-based models combine contextual information selection and learned computation within a tightly integrated architecture. This integration has proved highly effective across language and other modalities, but it does not establish that one fixed coupling of contextual localization and task computation is optimal for every workload.

The UCPSF research framework proposes a functional distinction between **Localization Intelligence**, which identifies and organizes relevant context, and **Per-Node Intelligence**, which performs computation over localized information.

This case study investigates whether heterogeneous Localization Engines and Per-Node Intelligence Engines can be composed adaptively under a Universal Control Plane.

We introduce a **Dual-Hybrid Selection** framework in which candidate Localization Engines—including Transformer-based contextual processing, semantic retrieval, Metric Differential Trees (MDT), UTN-based structural localization, and Common Concept Core (CCC) matching—may be paired with general-purpose LLMs, specialized Transformers, ANN scorers, symbolic reasoners, Principle Engines, or verification tools.

The framework uses capability contracts, Perspective-Aware Scoring Forests, Meta-Scoring, uncertainty estimates, and explicit governance constraints to select suitable computational configurations.

A hypothetical software-engineering task involving a multi-file API modification illustrates the selection process. Different task stages may favor different localization and execution combinations, while a single integrated model remains an eligible baseline.

The study also examines adaptive coupling and decoupling, context identity preservation, evaluation overhead, correlated failures, and the possibility of recursively learning reusable hybrid-selection Common Concept Cores.

A conceptual selection algorithm and falsifiable experimental program are provided.

No empirical advantage is claimed.

The central research hypothesis is that **adaptive, contract-governed selection of Localization and Per-Node Intelligence mechanisms can improve cost-adjusted task outcomes on sufficiently heterogeneous workloads**, while simpler integrated approaches may remain preferable in other settings.

**Keywords:** Hybrid Structural Intelligence, Localization Intelligence, Per-Node Intelligence, Universal Control Plane, Dual-Hybrid Architecture, Transformer, MDT, UTN, Common Concept Core, Scoring Forest, Meta-Scoring, Adaptive Dispatch, Contract-First Composition, Structural RSI

---

## 1. Introduction

### 1.1 The Architectural Question

An intelligence system must determine which information is relevant to a task and then perform computation using that information.

In many modern AI systems, these responsibilities are tightly coupled.

A Transformer, for example, uses attention and learned representations to condition computation on available context.

This integrated design has substantial advantages, including end-to-end optimization and efficient reuse of learned representations.

However, complex AI workflows may also employ external retrieval, specialized tools, symbolic methods, and multiple models.

This raises a broader architectural question:

> Must context localization and task computation always be performed through one fixed integrated mechanism?

### 1.2 Functional Decomposition

We propose distinguishing two functional responsibilities.

**Localization Intelligence**

Identifies, retrieves, organizes, or selects task-relevant context and structural references.

**Per-Node Intelligence**

Performs task-specific computation, inference, generation, verification, or optimization using the localized context.

These responsibilities may overlap in implementation.

The distinction is architectural rather than a claim about a strict physical separation within Transformer networks.

### 1.3 Dual-Hybrid Intelligence

The proposed Dual-Hybrid architecture permits:

1. Multiple Localization Engines;
2. Multiple Per-Node Intelligence Engines;
3. Multiple compatible compositions;
4. Adaptive selection under task constraints;
5. Structural learning from execution evidence.

### 1.4 Case Study Objective

This case investigates how a Universal Control Plane might select among such compositions.

The objective is to determine when modular hybridization provides measurable benefits and when integrated execution remains preferable.

---

## 2. Case Scenario — Multi-File API Evolution

### 2.1 Task Description

Consider a hypothetical software repository containing:

- Public API definitions;
- Service implementations;
- Data models;
- Database access code;
- Integration tests;
- Documentation;
- Client compatibility layers.

A user requests:

**Extend an existing API to support a new optional field while preserving compatibility with existing clients.**

### 2.2 Why This Task Is Interesting

The task requires more than generating code.

The system must identify:

- The API entry point;
- Relevant data structures;
- Callers and callees;
- Serialization behavior;
- Compatibility requirements;
- Affected tests;
- Potential migration concerns.

It must then implement and verify a consistent modification.

### 2.3 Localization Challenges

Relevant information may be distributed across multiple files and structural relationships.

Simple keyword retrieval may miss indirect dependencies.

A large context window may contain irrelevant information.

A Calling Graph may reveal dependencies that semantic similarity alone does not expose.

### 2.4 Per-Node Computation Challenges

Different task stages may require different capabilities:

- Requirement interpretation;
- Dependency analysis;
- Code generation;
- Schema validation;
- Test execution;
- Compatibility checking.

A single model may perform all these tasks, but specialized engines may be competitive for particular stages.

### 2.5 Proposed Research Question

Can adaptive selection among Localization and Per-Node Engines improve this workflow under controlled cost, latency, and reliability constraints?

---

## 3. Baseline Architectures

### 3.1 Baseline A — Integrated LLM

A single LLM receives the available repository context and performs the task.

```text id="b0g6f3"
User Request
     |
     v
Repository Context
     |
     v
Integrated LLM
     |
     v
Proposed Code Changes
     |
     v
Tests / Review
```

### 3.2 Strengths

Potential strengths include:

- Simple architecture;
- Minimal integration overhead;
- Unified learned representations;
- Straightforward orchestration;
- Strong general-purpose reasoning.

### 3.3 Limitations

Potential limitations include:

- Irrelevant context;
- Incomplete dependency coverage;
- High context-processing cost;
- Limited structural provenance;
- Difficulty selecting specialized computation for individual stages.

These limitations are workload-dependent.

### 3.4 Baseline B — Fixed Retrieval-Augmented LLM

A retrieval engine selects context before an LLM performs computation.

```text id="x91ujc"
User Request
     |
     v
Fixed Retrieval
     |
     v
LLM
     |
     v
Tests / Review
```

### 3.5 Baseline C — Fixed Structural Localization

A structural search mechanism identifies dependencies before invoking a coding model.

### 3.6 Baseline D — Fixed Multi-Engine Workflow

Different task stages invoke predefined specialized engines.

### 3.7 Proposed Architecture

The proposed Dual-Hybrid system selects Localization and Per-Node mechanisms dynamically.

The integrated LLM remains a valid candidate.

---

## 4. Dual-Hybrid Architecture

### 4.1 Localization Registry

Let:

$$
\mathcal{L}=\{L_1,L_2,\ldots,L_m\}
$$

represent available Localization Engines.

### 4.2 Per-Node Registry

Let:

$$
\mathcal{I}=\{I_1,I_2,\ldots,I_n\}
$$

represent available Intelligence Engines.

### 4.3 Candidate Composition

A candidate configuration is:

$$
a=(L_i,I_j,C_{ij})
$$

where $C_{ij}$ represents the applicable composition contract.

### 4.4 Valid Configuration Space

The set of valid configurations is:

$$
\mathcal{A}_{valid} =
\{
a \mid
Compatible(a)
\land
PolicyAllowed(a)
\}
$$

### 4.5 Architecture

```text id="asv4h8"
                      TASK / PERSPECTIVE
                              |
                              v
                    UNIVERSAL CONTROL PLANE
                              |
                +-------------+-------------+
                |                           |
                v                           v
       LOCALIZATION REGISTRY       INTELLIGENCE REGISTRY
                |                           |
       +--------+--------+         +--------+--------+
       |        |        |         |        |        |
       v        v        v         v        v        v
    Semantic   MDT/UTN   CCC      LLM      ANN    Symbolic
    Retrieval  Search    Match    Models   Nodes  Engines
       |        |        |         |        |        |
       +--------+--------+---------+--------+--------+
                              |
                              v
                     CONTRACT VALIDATION
                              |
                              v
                     SCORING FOREST
                              |
                              v
                    HYBRID CONFIGURATION
                              |
                              v
                          EXECUTION
                              |
                              v
                      EXTERNAL OUTCOMES
                              |
                              v
                      EVIDENCE FEEDBACK
```

### 4.6 Dynamic Selection

The Control Plane selects a configuration according to:

- Task requirements;
- Perspective;
- Available context;
- Engine capabilities;
- Cost;
- Latency;
- Risk;
- Validation evidence.

### 4.7 No Universal Winner

The best configuration may vary by task.

The objective is adaptive selection, not permanent replacement of integrated models.

---

## 5. Localization Engine Families

### 5.1 Transformer-Based Contextual Localization

Transformer attention supports context-dependent representation and information integration.

This can be treated as an internal localization-related capability.

However, attention weights are not necessarily faithful explanations of which information causally determined a model output.

### 5.2 Semantic Retrieval

Semantic retrieval identifies potentially relevant material using learned representations or similarity measures.

Potential strengths include:

- Flexible matching;
- Efficient retrieval;
- Broad language coverage.

Potential limitations include missing structural dependencies.

### 5.3 Metric Differential Tree Localization

MDT-based localization organizes information through metric and structural differences.

Potential advantages include:

- Hierarchical narrowing;
- Explicit structural relationships;
- Reusable search paths.

Its practical benefits depend on the quality of the representation and indexing mechanisms.

### 5.4 UTN-Based Localization

UTN-based localization uses structural identity and context references to identify relevant objects.

Potential advantages include:

- Stable references;
- Context-aware retrieval;
- Cross-component identity management.

### 5.5 CCC Matching

CCC matching identifies reusable structural or behavioral patterns.

It may help locate:

- Similar workflows;
- Reusable principles;
- Common dependency structures;
- Applicable evaluation templates.

### 5.6 Calling Graph Localization

Calling Graph traversal may identify execution dependencies.

For software engineering, this can reveal relevant relationships not captured by text similarity alone.

### 5.7 Hybrid Localization

Multiple Localization Engines may be combined.

For example:

```text id="d1h1wc"
User Request
     |
     v
Semantic Candidate Retrieval
     |
     v
Calling Graph Expansion
     |
     v
UTN Identity Resolution
     |
     v
Context Sufficiency Evaluation
```

This is a candidate workflow, not a required universal pipeline.

---

## 6. Per-Node Intelligence Engine Families

### 6.1 General-Purpose LLMs

General-purpose LLMs provide flexible reasoning and generation capabilities.

### 6.2 Specialized Transformers

Specialized models may offer advantages on particular domains or tasks.

### 6.3 ANN Scoring Nodes

ANN scorers may provide fast approximate evaluation.

They may be useful for:

- Ranking;
- Filtering;
- Quality estimation;
- Specialized dispatch decisions.

### 6.4 Symbolic Engines

Symbolic methods may support:

- Constraint checking;
- Formal rules;
- Type validation;
- Logical inference.

### 6.5 Principle Engines

Principle Engines may apply reusable abstract rules or learned structural principles.

Their applicability must be validated for the task.

### 6.6 Optimization Engines

Optimization tools may solve constrained numerical or combinatorial subproblems.

### 6.7 Simulation and Testing Engines

External tools may provide evidence that language-model reasoning alone cannot establish.

### 6.8 Hybrid Per-Node Execution

A task node may invoke several engines.

For example:

```text id="z54ddx"
Localized API Context
        |
        v
Coding LLM
        |
        v
Static Type Checker
        |
        v
Test Runner
        |
        v
Compatibility Evaluator
```

---

## 7. Contract-First Composition

### 7.1 Why Contracts Matter

Different Localization Engines may return different kinds of outputs.

For example:

- Text snippets;
- Structural references;
- Calling Graph nodes;
- Ranked candidates;
- CCC identifiers;
- Context-bound objects.

A Per-Node Engine must understand the representation it receives.

### 7.2 Localization Contract

A Localization Engine should declare:

- Input requirements;
- Output schema;
- Structural identity;
- Relevance semantics;
- Coverage information;
- Provenance;
- Uncertainty.

### 7.3 Intelligence Contract

A Per-Node Engine should declare:

- Supported task types;
- Required context format;
- Output schema;
- Tool permissions;
- Cost profile;
- Failure conditions.

### 7.4 Composition Contract

A composition contract specifies:

- Representation compatibility;
- Required adapters;
- Context preservation;
- Error handling;
- Validation requirements.

### 7.5 Context Identity

Structural references should remain traceable across engine boundaries.

UTN-based approaches provide one candidate mechanism.

### 7.6 Contract Failure

If a configuration cannot satisfy required contracts, it should not be selected solely because its predicted score is favorable.

### 7.7 Contract Evolution

New engines may introduce new interfaces.

Contract evolution should be versioned and independently validated.

---

## 8. Perspective-Aware Selection

### 8.1 Perspective Definition

Following UCPSF-005:

$$
P=(G,C,B,T,R)
$$

where:

- $G$: Goals;
- $C$: Context and constraints;
- $B$: Resource budget;
- $T$: Time horizon;
- $R$: Risk preferences.

### 8.2 Example Perspectives

**Rapid Development**

Prioritizes speed and low computational cost.

**Production Engineering**

Prioritizes correctness, maintainability, and test coverage.

**Security-Sensitive Engineering**

Prioritizes independent validation and risk reduction.

**Large-Repository Refactoring**

Prioritizes structural dependency coverage.

### 8.3 Perspective-Dependent Configuration

A rapid task may favor one integrated model.

A large multi-file refactoring task may favor Calling Graph localization and specialized validation.

### 8.4 Hard Constraints

Mandatory constraints remain non-compensable.

A configuration that violates required permissions or data-handling rules must be excluded.

---

## 9. Scoring Forest for Hybrid Selection

### 9.1 Selection Criteria

Candidate configurations may be evaluated through:

- Localization quality;
- Execution quality;
- Cost;
- Latency;
- Reliability;
- Context sufficiency;
- Risk;
- Contract compatibility.

### 9.2 Candidate Scoring Forest

$$
\mathcal{F}_S=
\{
T_L,T_I,T_C,T_R,T_B
\}
$$

where:

- $T_L$: Localization quality;
- $T_I$: Intelligence Engine suitability;
- $T_C$: Composition compatibility;
- $T_R$: Risk;
- $T_B$: Budget and resource cost.

### 9.3 Localization Quality

Evaluate:

- Relevance;
- Coverage;
- Structural correctness;
- Provenance;
- Missing context.

### 9.4 Engine Suitability

Evaluate:

- Task specialization;
- Expected quality;
- Reliability;
- Tool compatibility;
- Resource cost.

### 9.5 Composition Quality

Evaluate whether the selected Localization and Per-Node Engines work effectively together.

A strong Localization Engine and a strong Intelligence Engine do not necessarily form a strong pair.

### 9.6 Risk Evaluation

Assess:

- Missing dependencies;
- Incorrect context mapping;
- Unsafe tool execution;
- Verification gaps;
- Distribution shift.

### 9.7 Cost Evaluation

Account for:

- Localization cost;
- Engine execution cost;
- Adapter overhead;
- Validation cost;
- Retry cost.

### 9.8 Multi-Objective Selection

A conceptual objective is:

$$
a^*
=
\arg\max_{a\in\mathcal{A}_{valid}}
U(a\mid P,E)
$$

where $E$ represents available evidence.

This formulation assumes a defined utility model.

When objectives cannot be validly scalarized, Pareto or lexicographic selection may be more appropriate.

---

## 10. Meta-Scoring and Adaptive Evaluation

### 10.1 Selection Uncertainty

The Control Plane may be uncertain about the best configuration.

### 10.2 Meta-Scoring

Meta-Scoring evaluates the reliability and applicability of the Scoring Trees used for configuration selection.

### 10.3 Candidate Meta-Evaluation Dimensions

Potential dimensions include:

- Calibration;
- Historical validity;
- Task applicability;
- Cost;
- Robustness;
- Evidence quality;
- Distribution shift.

### 10.4 Adaptive Evaluation Depth

Routine tasks may require lightweight selection.

High-risk tasks may require richer evaluation.

### 10.5 Exploration Versus Exploitation

The system may sometimes test a less familiar configuration to collect evidence.

Such exploration should remain within explicit budgets and governance constraints.

### 10.6 Independent Validation

A configuration-selection mechanism should not be promoted solely on its own predicted scores.

External task outcomes are required.

---

## 11. Illustrative Hybrid Selection Campaign

### 11.1 Task Stage A — Requirement Interpretation

**Candidate Configuration:**

Integrated general-purpose LLM.

**Rationale:**

The task may be adequately handled through language understanding without extensive structural localization.

### 11.2 Task Stage B — Repository Localization

**Candidate Configuration:**

Semantic retrieval followed by Calling Graph expansion.

**Rationale:**

The task requires identifying distributed dependencies.

### 11.3 Task Stage C — Structural Identity Resolution

**Candidate Configuration:**

UTN-based reference mapping.

**Rationale:**

The system must preserve consistent identity across files and task stages.

### 11.4 Task Stage D — Code Modification

**Candidate Configuration:**

Specialized coding model with localized context.

**Rationale:**

A specialized engine may be competitive for code generation.

### 11.5 Task Stage E — Verification

**Candidate Configuration:**

Static analysis, test execution, and compatibility checking.

**Rationale:**

External tools provide evidence beyond generated text.

### 11.6 Task Stage F — Final Evaluation

**Candidate Configuration:**

Perspective-aware Scoring Forest.

**Rationale:**

The result must satisfy functional, cost, risk, and compatibility requirements.

### 11.7 Illustrative Workflow

```text id="xmx6zi"
User API Change Request
          |
          v
General LLM Requirement Analysis
          |
          v
Semantic Retrieval
          |
          v
Calling Graph Expansion
          |
          v
UTN Context Identity Mapping
          |
          v
Specialized Coding Engine
          |
          v
Static Analysis and Tests
          |
          v
Scoring Forest Evaluation
          |
          v
Accept / Revise / Escalate
```

### 11.8 Interpretation

This workflow illustrates one possible selection.

It does not demonstrate that the configuration is optimal.

A simpler integrated architecture may outperform it under some workloads.

---

## 12. Adaptive Coupling and Decoupling

### 12.1 The Coupling Question

Should Localization and Per-Node Intelligence remain integrated or be separated into modules?

### 12.2 Tight Coupling

Advantages may include:

- Lower interface overhead;
- End-to-end optimization;
- Unified representations;
- Efficient internal information exchange.

### 12.3 Loose Coupling

Advantages may include:

- Component reuse;
- Independent specialization;
- Explicit structural identity;
- Modular validation;
- Selective replacement.

### 12.4 Costs of Decoupling

Potential costs include:

- Adapter overhead;
- Representation mismatch;
- Latency;
- Error propagation;
- Contract maintenance.

### 12.5 Adaptive Coupling

The Control Plane should treat coupling as a selectable architectural variable.

### 12.6 Candidate Modes

**Mode A — Fully Integrated**

One model performs localization and computation.

**Mode B — Assisted Integration**

An external Localization Engine supplies context to an integrated model.

**Mode C — Modular Hybrid**

Localization and computation are performed by separate components.

**Mode D — Multi-Engine Composition**

Several Localization and Per-Node Engines collaborate.

### 12.7 Selection Principle

> Use the simplest configuration that satisfies the required task quality, risk, cost, and governance constraints.

---

## 13. Proposed Dual-Hybrid Selection Algorithm

```text id="07ekcw"
Algorithm: Dual-Hybrid-Localization-Per-Node-Selection

Input:
    Task X
    Perspective P
    Localization Registry L
    Intelligence Registry I
    Contract Registry C
    Scoring Forest S
    Meta-Scoring Registry M
    Evidence Repository E
    Governance Rules G
    Resource Budget B

Output:
    Selected Configuration A*
    Task Result Y
    Execution Trace T

1. Resolve task requirements.

2. Resolve Perspective P.

3. Resolve mandatory governance constraints G.

4. Identify candidate Localization Engines.

5. Identify candidate Per-Node Engines.

6. Generate candidate compositions.

7. Include integrated-model baselines.

8. Validate composition contracts.

9. Reject incompatible configurations.

10. Reject policy-ineligible configurations.

11. Estimate localization quality.

12. Estimate engine suitability.

13. Estimate composition quality.

14. Estimate cost, latency, and risk.

15. Meta-score evaluation applicability.

16. Select configuration under budget B.

17. Execute selected configuration.

18. Collect task outcomes and evidence.

19. Apply required independent validation.

20. Evaluate result quality and uncertainty.

21. If additional computation is justified:
        Retry, delegate, or escalate.

22. Record configuration and evaluator versions.

23. Identify reusable selection patterns.

24. Generate optional CCC or dispatch proposals.

25. Submit structural proposals to
    independent validation and governance.

26. Return configuration, result, and trace.
```

The algorithm is conceptual.

A production implementation requires explicit scheduling, concurrency, authorization, and failure-recovery mechanisms.

---

## 14. Learning Hybrid Selection CCCs

### 14.1 Repeated Selection Patterns

Across many tasks, the Control Plane may discover recurring configuration patterns.

### 14.2 Candidate Examples

A repeated pattern may be:

**Large Repository + Multi-File Dependency Task**

→ Structural Localization + Specialized Coding Engine + External Verification.

Another may be:

**Small Localized Change + Low Risk**

→ Integrated LLM + Lightweight Validation.

### 14.3 Structural CCC

A Structural CCC may encode reusable configuration-selection rules.

### 14.4 Behavioral CCC

A Behavioral CCC may encode observed relationships between task conditions and successful configuration choices.

### 14.5 Unaligned AND Folding

Different workflows may use different engines while expressing similar selection principles.

Unaligned AND Folding may identify reusable commonality.

### 14.6 Core Plus Delta

A candidate representation is:

$$
A_i \approx K_A \oplus \Delta_i
$$

where:

- $K_A$: Reusable architecture-selection core;
- $\Delta_i$: Task-specific configuration differences.

### 14.7 Recursive Distillation

New evidence may lead to:

- CCC refinement;
- Specialized branches;
- Revised engine rankings;
- New compatibility rules;
- Retired configurations.

### 14.8 Promotion

Selection CCCs should be validated on held-out tasks before promotion.

---

## 15. Failure Modes

### 15.1 Wrong Localization

The system retrieves irrelevant or incomplete context.

**Mitigation:** Coverage checks and alternative localization.

### 15.2 Wrong Engine Selection

The selected engine is unsuitable.

**Mitigation:** Capability contracts and Meta-Scoring.

### 15.3 Representation Mismatch

Localization output is incompatible with engine expectations.

**Mitigation:** Contract validation and explicit adapters.

### 15.4 Context Identity Loss

Structural references become ambiguous across stages.

**Mitigation:** Stable identity and provenance mechanisms.

### 15.5 Excessive Composition Overhead

Modular execution becomes more expensive than integrated execution.

**Mitigation:** Cost-aware selection and simple baselines.

### 15.6 Correlated Failures

Multiple engines share the same weakness.

**Mitigation:** Independent validation and evidence lineage.

### 15.7 Selection Overfitting

The Control Plane overfits to historical workloads.

**Mitigation:** Held-out tasks and distribution-shift testing.

### 15.8 Unsafe Tool Execution

A selected engine attempts an unauthorized action.

**Mitigation:** Independent authorization enforcement.

### 15.9 Structural Overgrowth

The registry accumulates too many poorly validated configurations.

**Mitigation:** Lifecycle management and retirement.

### 15.10 CCC Overgeneralization

A reusable selection core is applied outside its valid domain.

**Mitigation:** Applicability boundaries and counter-evidence.

---

## 16. Experimental Validation Design

### 16.1 Research Questions

**RQ-001:** Does adaptive Dual-Hybrid selection improve cost-adjusted task quality?

**RQ-002:** When does structural localization outperform semantic retrieval?

**RQ-003:** When does an integrated model outperform modular composition?

**RQ-004:** Does Meta-Scoring improve configuration selection?

**RQ-005:** Can reusable selection CCCs transfer across related tasks?

**RQ-006:** What is the cost of contract and control overhead?

### 16.2 Baselines

Proposed baselines include:

1. Single integrated LLM;
2. Fixed retrieval-augmented LLM;
3. Fixed structural localization;
4. Fixed multi-engine pipeline;
5. Dynamic routing without Scoring Forests;
6. Dynamic routing with fixed scoring;
7. Full Dual-Hybrid selection with Meta-Scoring.

### 16.3 Task Families

Potential benchmark tasks include:

- Single-file bug fixes;
- Multi-file refactoring;
- API evolution;
- Dependency updates;
- Test generation;
- Performance optimization;
- Security-sensitive changes.

### 16.4 Controlled Variables

Experiments should control for:

- Model capabilities;
- Available tools;
- Context limits;
- Total compute budget;
- Task difficulty;
- Benchmark exposure;
- Human intervention;
- Validation procedures.

### 16.5 Metrics

| Metric | Purpose |
|---|---|
| Task Success Rate | Correct completion |
| Localization Recall | Coverage of relevant context |
| Localization Precision | Relevance of selected context |
| Context Sufficiency | Adequacy for downstream computation |
| Total Compute Cost | End-to-end resource consumption |
| Latency | Completion time |
| Contract Conformance | Compatibility correctness |
| Regression Rate | Unintended failures |
| Selection Regret | Loss relative to an evaluated reference configuration |
| Structural Reuse | Reuse of validated selection CCCs |
| Robustness | Performance under distribution shift |

### 16.6 Hypotheses

**H1:** Adaptive Dual-Hybrid selection improves cost-adjusted outcomes on heterogeneous workloads.

**H2:** Structural localization improves dependency coverage on tasks with complex repository relationships.

**H3:** Integrated models remain competitive or superior on sufficiently simple tasks.

**H4:** Meta-Scoring improves selection under changing Perspectives.

**H5:** Selection CCCs can transfer useful configuration knowledge across related tasks.

### 16.7 Validation Status

This case study is conceptual.

No experiments are reported.

No quantitative performance improvements are claimed.

---

## 17. Expected Benefits and Tradeoffs

### 17.1 Potential Benefits

The proposed architecture may provide:

- More flexible engine selection;
- Better structural localization;
- Improved use of specialized computation;
- Explicit context identity;
- More transparent evaluation;
- Reusable selection knowledge;
- Governed structural evolution.

### 17.2 Potential Costs

The architecture introduces:

- Control Plane overhead;
- Contract maintenance;
- Additional evaluation;
- Adapter complexity;
- More complicated debugging;
- Registry management.

### 17.3 Applicability

The architecture may be most useful when:

- Tasks vary substantially;
- Multiple engines are available;
- Structural context matters;
- Verification requirements differ;
- Resource constraints change;
- Repeated workflows support structural learning.

### 17.4 Simplicity Criterion

A more complex architecture should be adopted only when its validated benefits justify its lifecycle costs.

---

## 18. Relationship to the UCPSF Framework

### UCPSF-001

Generalized Scoring Intelligence provides the evaluation foundation.

### UCPSF-002

Scoring Operators support configuration evaluation and structural adjustment.

### UCPSF-003

Scoring Trees and Forests organize selection criteria.

### UCPSF-004

Recursive CCC distillation supports reusable selection structures.

### UCPSF-005

Perspective-Aware Meta-Scoring guides configuration selection.

### UCPSF-006

Dual-Hybrid Localization and Per-Node Intelligence provides the primary architecture.

### UCPSF-007

The Universal Control Plane governs composition, execution, and structural evolution.

### UCPSF-008

Open-Ended Scoring Intelligence motivates long-term structural learning.

### CASE-001

Scoring-Controlled AI Relay examines adaptive workflow decisions.

### CASE-002

Scoring-Guided Structural RSI examines governed architecture evolution.

---

## 19. Conclusion

Transformer-based models demonstrate the effectiveness of tightly integrated contextual processing and learned computation.

However, heterogeneous AI workflows create opportunities for additional architectural flexibility.

This case study proposes Dual-Hybrid Selection as a method for composing multiple Localization Engines and Per-Node Intelligence Engines under a Universal Control Plane.

The proposed architecture integrates:

1. Heterogeneous Localization Engines;
2. Heterogeneous Per-Node Intelligence Engines;
3. Contract-first composition;
4. Perspective-Aware Scoring Forests;
5. Meta-Scoring;
6. Adaptive coupling and decoupling;
7. Evidence-driven structural learning;
8. Governed promotion.

Its central proposition is:

> **Localization Intelligence and Per-Node Intelligence can be treated as separately selectable functional capabilities, allowing an AI system to adapt its computational architecture to task requirements rather than relying on one fixed composition.**

A complementary principle is:

> **Hybridization is valuable only when the resulting configuration improves validated outcomes relative to simpler alternatives.**

The proposed framework does not establish that modular systems universally outperform integrated models.

Instead, it defines an architectural search and control problem that can be investigated empirically.

If validated, Dual-Hybrid Selection may provide an important application of Universal Control Planes and Scoring Intelligence.

---

## Suggested Figure Placement

### Fig-006 — Dual-Hybrid Localization and Per-Node Intelligence

**File:** `../figures/Fig-006-Dual-Hybrid-Localization-and-Per-Node-Intelligence.png`

**Suggested insertion:** After Section 4.7.

**Purpose:** Illustrate the two hybrid engine families, contract-aware composition, and adaptive configuration selection.

### Fig-005 — Perspective Optimization and Meta-Scoring

**File:** `../figures/Fig-005-Perspective-Optimization-and-Meta-Scoring.png`

**Suggested insertion:** After Section 10.6.

**Purpose:** Illustrate Perspective-aware selection, Scoring Forest evaluation, and Meta-Scoring.

### Fig-001 — Universal Control Plane Grand Map

**File:** `../figures/Fig-001-Universal-Control-Plane-Grand-Map.png`

**Suggested insertion:** After Section 13.

**Purpose:** Show how Dual-Hybrid selection fits into the broader Universal Control Plane architecture.

---

## Research Lineage

### Metric Differential Tree, UTN, and Context-Bound Token Intelligence

https://github.com/sizhet/Metric-Differential-Tree-UTN-and-Context-Bound-Token-Intelligence

### Principle Intelligence and Open Structural Learning

https://github.com/sizhet/Principle-Intelligence-and-Open-Structural-Learning

### Portable Intelligence Runtime Pieces and Units

https://github.com/sizhet/Portable-Intelligence-Runtime-Pieces-and-Units

### Structural Recursive Self-Improvement

https://github.com/sizhet/Structural-Recursive-Self-Improvement

### Generalized Structural Trigger and Computational Growth Intelligence

https://github.com/sizhet/Generalized-Structural-Trigger-and-Computational-Growth-Intelligence

These references establish conceptual continuity within the Structural Intelligence research program. They do not constitute independent empirical validation of the proposed architecture.

---

## Citation

Suggested citation prior to DOI assignment:

Tan, S., & GPT-Obot. (2026). *CASE-003: Hybrid Localization and Per-Node Selection*. Universal Control Planes and Scoring Tree/Forest/Folding for Structural Intelligence, Version 1.0.0.

Repository:

https://github.com/sizhet/Universal-Control-Planes-and-Scoring-Folding

DOI: 10.5281/zenodo.23486273

---

## License

Copyright © 2026 Sizhe Tan & GPT-Obot.

Licensed under the Apache License, Version 2.0.

---

**Document:** CASE-003  
**Research Series:** Universal Control Planes and Scoring Tree/Forest/Folding  
**Status:** Conceptual Case Study and Proposed Validation Design  
**Version:** 1.0.0
