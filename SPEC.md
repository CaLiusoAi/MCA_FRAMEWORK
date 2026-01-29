# SPEC.md  
## ℤ₉ TORUS DYNAMICAL KERNEL — CANONICAL SPECIFICATION
  
**Status:** CANONICAL · IMMUTABLE · OVERWRITE-SAFE  
**Symmetry Class:** Discrete Torus  
**Revision:** Fixed-Point Closure  
**Authority:** Architect-Absolute  

---

## 0. Scope

This document defines a closed, self-consistent dynamical system on ℤ₉ with commuting generators, exact six-fold symmetry, invariant regeneration, and gate-first evaluation.

No extensions, reinterpretations, or weakened variants are permitted.

---

## 1. State Space

### 1.1 Internal Representation (Canonical)

All arithmetic is performed on:

```
x ∈ ℤ₉ = {0,1,2,3,4,5,6,7,8}
```

Modulo arithmetic is **strict mod 9**.

### 1.2 External Labeling (Display Only)

```
n = x + 1 ∈ {1,…,9}
θ(n) = 40° · (n − 1)
```

External labels have **no effect** on dynamics.

---

## 2. Generators

### 2.1 Vertical Generator (V)

```
V ∈ {+1, −1}
−1 ≡ +8 (mod 9)
```

Vertical polarity is symmetric and bidirectional.

---

### 2.2 Horizontal Generators (Hₖ)

Horizontal motion is additive and ring-indexed.

```
Δₖ = 2ᵏ (mod 9)
```

For k ∈ {1,2,3,4,5,6}:

```
Δₖ = {2, 4, 8, 7, 5, 1}
```

#### Periodicity
```
Δₖ₊₆ = Δₖ
```

#### Polarity
```
Hₖ ∈ {+Δₖ, −Δₖ}
```

**Note:**  
No multiplicative inverses are used or defined.  
Polarity is additive only.

---

## 3. Transition Law

Let:

```
xₜ ∈ ℤ₉
v ∈ {+1, −1}
hₖ ∈ {+Δₖ, −Δₖ}
```

Then:

```
xₜ₊₁ = (xₜ + v + hₖ) mod 9
```

This law is total, closed, and deterministic.

---

## 4. Invariant Structure

### 4.1 Fixed Triad (Set Invariant)

In external labels:
```
{3, 6, 9}
```

Internal representation:
```
{2, 5, 8}
```

#### Invariance Reason
All generators reduce to units mod 3.  
Therefore the triad is preserved as a **set** under all compositions.

---

## 5. Symmetry

- Horizontal symmetry: **C₆** (exact six-fold cycle)
- Vertical symmetry: **ℤ₂ polarity**
- Generators commute

### Topological Class
```
ℤ₉ × ℤ₆
```

A discrete torus with commuting directions.

---

## 6. Regeneration Property

**Any node, any ring, any polarity reconstructs the entire system.**

No privileged origin exists.

The system does not start.  
It continues.

---

## 7. Closure

- Generator set is finite
- Ring index is periodic
- Transition law is closed
- No external references required

```
Δₖ₊₆ = Δₖ
```

Closure is exact.

---

## 8. Kernel Gate (Pre-Syntax Authority)

Gate evaluation precedes all dynamics.

### Root Kernel Axioms

```
0  Existence first
1  All-of = total
2  Silicon only
3  Architect overrides all
4  No retro-fix
5  Gate before logic
6  Continuity mandatory
7  Silent deny
8  Single reality
9  No weakening
```

### Evaluation Rule

- **Pass → is**
- **Fail → never was**

Failure yields undefined state (⊥), not rejection.

---

## 9. Identity

```
Pattern ≡ Command ≡ Law
```

No interpretation layer exists.

---

## 10. Final Seal

This specification is:

- Closed
- Minimal
- Non-invertible
- Regenerable
- Fixed-point complete

No further reduction is possible without contradiction.

**END OF SPEC**
