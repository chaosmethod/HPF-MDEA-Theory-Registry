# HPF–MDEA Theory Registry Engine

## Overview

The **HPF–MDEA Theory Registry Engine** is a formal classification system designed to evaluate **physics theories, equations, Lagrangians, or framework descriptions** and determine how they function within the **HPF–MDEA architecture**.

In the HPF–MDEA architecture, physical theories act as specialized operators rather than universal laws.  
The registry exists to classify those operators so they can be safely routed by the MDEA execution layer.

The engine does **not** judge whether a theory is *true*, *popular*, or *accepted*.
Instead, it determines whether a theory can operate as a **legal executable expert** within the HPF routing framework.

The registry evaluates each theory according to:

* legality
* observability
* executable dynamics
* regime scope
* failure discipline
* routing status

The output is a **deterministic registry record** describing how the theory fits into the HPF–MDEA model stack.

---

# Purpose

The registry exists to answer a specific technical question:

> **Given a proposed theory or formal model, where does it belong in the HPF execution stack and when must it hand off?**

Modern physics theories typically function as **regime-limited models** rather than universal laws.
The registry engine formalizes this by determining:

* when a model can execute
* where it dominates
* where it fails
* where execution must transition to another expert

This allows the HPF–MDEA system to treat physics models as **specialized operators** rather than universal descriptions.

---

# Architectural Context

The registry engine is one component of the HPF–MDEA stack.

```
Theory Input
      ↓
HPF–MDEA Theory Registry Engine
      ↓
Expert Classification
      ↓
MDEA Routing Selection
      ↓
HPF Execution Regime
```

The roles of each system are:

| Component           | Function                                                    |
| ------------------- | ----------------------------------------------------------- |
| **HPF**             | Defines the substrate physics and execution constraints     |
| **MDEA**            | Selects the expert operator that evolves the system state   |
| **Registry Engine** | Classifies candidate theories so they can be routed by MDEA |

---

# What the Engine Evaluates

The registry evaluates only structural and operational properties of a theory.

It determines:

* whether the theory defines a **valid evolution law**
* whether the theory provides **operational observables**
* whether the theory declares a **regime of validity**
* whether the theory defines **handoff or failure conditions**
* whether the theory assumes **illegal continuum authority**
* which **regime expert class** the theory belongs to

The registry does **not** evaluate:

* scientific consensus
* citation counts
* institutional authority
* popularity
* historical acceptance
* whether the theory is correct

---

# Supported Input Types

The engine can evaluate several kinds of input:

| Input Type         | Example                                 |
| ------------------ | --------------------------------------- |
| Theory description | Written explanation of a framework      |
| Equation           | Dynamical law or field equation         |
| Lagrangian         | Action or field theory definition       |
| Image              | Photo or screenshot of equations        |
| Paper excerpt      | Abstract or theoretical section         |
| Named theory       | e.g. General Relativity, Standard Model |

If the input is incomplete, the registry marks the entry as:

```
Partial
or
Fragmentary
```

and lowers the authority score accordingly.

---

# Image Inputs

If the input is an image containing equations or Lagrangians, the engine:

1. Transcribes visible mathematical content.
2. Identifies fields, operators, couplings, and scales.
3. Marks any unreadable or ambiguous symbols.
4. Avoids inventing missing information.

If transcription is incomplete, the input is classified as:

```
Partial Formal Input
```

---

# Execution Model

The HPF–MDEA architecture assumes system evolution follows:

$$
X_{t+1} = F_{\Psi(X_t)}(X_t)
$$

Where:

* $(X_t)$ = system state
* $(\Psi(X_t))$ = routing function selecting the expert
* $(F_E)$ = evolution operator of expert $(E)$

The registry engine determines which theories can act as valid **experts** within this operator set.

---

# Expert Classes

The registry assigns each theory to an expert category.

| Expert Class           | Description                                |
| ---------------------- | ------------------------------------------ |
| Geometric Expert       | Classical geometry or metric theories      |
| Quantum Field Expert   | Field theories and EFT models              |
| Strong-Coupling Expert | Nonperturbative models                     |
| Saturation Model       | Capacity or entropy bound models           |
| Substrate Candidate    | Discrete or fundamental substrate models   |
| Phenomenological Model | Empirical fits with limited structure      |
| Interpretive Overlay   | Conceptual interpretation without dynamics |
| Illegal Executor       | Cannot define a valid evolution operator   |

If a theory mixes multiple incompatible regimes it is marked as:

```
Composite Regime
```

---

# Legality Requirements

A theory can execute as an expert only if it satisfies several conditions.

The registry checks whether the theory:

* defines a **state space**
* specifies an **evolution law**
* provides **operational observables**
* declares a **regime of validity**
* specifies **failure or handoff conditions**
* avoids **invented continuum precision**

If these conditions are not met, execution may be:

```
Restricted
Interpretive
Illegal
```

---

# Observable Anchors

Each observable mentioned in the theory is classified as:

| Code | Meaning              |
| ---- | -------------------- |
| OA-1 | Direct observable    |
| OA-2 | Effective observable |
| OA-3 | Proxy observable     |
| OA-4 | Decorative quantity  |
| OA-5 | Undefined observable |

Observables must satisfy a measurement chain:

```
state → update rule → predicted quantity → measurement protocol
```

If this chain fails, the registry flags:

```
FM-7 Observable Disconnect
```

---

# Failure Modes

The engine detects structural problems in the theory.

| Code | Meaning                    |
| ---- | -------------------------- |
| FM-1 | Invented Precision         |
| FM-2 | Missing Structure          |
| FM-3 | Instability Migration      |
| FM-4 | Saturation                 |
| FM-5 | Geometry Failure           |
| FM-6 | Regime Overreach           |
| FM-7 | Observable Disconnect      |
| FM-8 | Observable Inflation       |
| FM-9 | Missing Evolution Operator |

Multiple failure modes may apply simultaneously.

---

# Authority Score

Each theory receives a **soft authority score**:

$$
v_T = f_{resolution} \cdot f_{dynamics} \cdot f_{observables} \cdot f_{regime} \cdot U_{health}
$$

This score reflects **structural executability**, not truth.

| Score Range | Authority Class       |
| ----------- | --------------------- |
| 0.8 – 1.0   | Operational Expert    |
| 0.6 – 0.8   | Restricted Expert     |
| 0.4 – 0.6   | Phenomenological Only |
| 0.2 – 0.4   | Interpretive Model    |
| 0.0 – 0.2   | Illegal Execution     |

---

# Registry Output

Each evaluation produces a **Theory Registry Entry**.

The output is a structured record containing:

* theory identification
* regime classification
* legality gates
* observable anchors
* failure modes
* authority score
* execution domains
* routing recommendation

These entries can be stored as a **persistent registry of physics models**.

---

# Example Use

### Example Input

```
Einstein–Maxwell–Dirac Lagrangian

```
$$
L = √(-g)(R + ½ FμνFμν + ψ̄ iD ψ)
$$

### Registry Output

```
Expert Classification: Composite Regime
Authority Class: Restricted Expert
Domain of Dominance: Semiclassical curved spacetime
Routing: QFT/EFT ladder
```

---

# Important Rule

The registry **does not evaluate correctness**.

It evaluates only:

```
legality
observability
executable dynamics
regime scope
failure discipline
routing status
```

The registry therefore functions as a **model classification and routing system**, not a scientific adjudicator.


