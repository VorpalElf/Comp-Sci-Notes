---
Date & Time: 23-09-2026 11:02
Lecturer:
  - Eddie Jones
Course Name:
  - COMS10014
Lecture Name: Boolean Algebra
---
## Introduction
- Syntax: Representations
- Semantics: Meaning/Thing
- Equivalent: Equal under all assignments (i.e. same output in truth table)
⭐️ Use $\phi \space \psi \space \rho$ to represent propositions
⭐️ Use p, q, r to represent variables

## Laws of Boolean Algebra
| Name        | Axiom 1      | Axiom 2      |
| ----------- | ------------ | ------------ |
| Identity    | $x ∧ 1 ≡ x$  | $x ∨ 0 ≡ x$  |
| Null        | $x ∧ 0 ≡ 0$  | $x ∨ 1 ≡ 1$  |
| Idempotency | $x ∧ x ≡ x$  | $x ∨ x ≡ x$  |
| Inverse     | $x ∧ ¬x ≡ 0$ | $x ∨ ¬x ≡ 1$ |
⭐️ Idempotency: It's just the same, so operators doesn't matter

| Name          | Axiom(s)                                                   | Hints 💡                                  |
| ------------- | ---------------------------------------------------------- | ----------------------------------------- |
| Commutativity | $x ∧ y ≡ y ∧ x$                                            |                                           |
| Association   | $(x ∧ y) ∧ z ≡ x ∧ (y ∧ z)$<br>$(x ∨ y) ∨ z ≡ x ∨ (y ∨ z)$ | Move brackets                             |
| Distribution  | $x ∧ (y ∨ z) ≡ (x∧y)∨(x∧z)$<br>$x ∨ (y ∧ z) ≡ (x∨y)∧(x∨z)$ | Multiplications<br>AND -> OR<br>OR -> AND |
| Absorption    | $x ∧ (x ∨ y) ≡ x$                                          |                                           |
| de Morgan     | $¬(x ∧ y) ≡ ¬x ∨ ¬y$                                       | Flip operator                             |
| Equivalence   | $x ≡ y ≡ (x ⇒ y) ∧ (y ⇒ x)$                                | Two-way                                   |
| Implication   | $x ⇒ y ≡ ¬x ∨ y$                                           | one-way                                   |
| Involution    | $¬¬x ≡ x$                                                  |                                           |
## Extra
| Name          | Axiom(s)                                                   | Hints 💡                                  |
| ------------- | ---------------------------------------------------------- | ----------------------------------------- |
| Commutativity | $xy ≡ yx$                                                  |                                           |
| Association   | $(xy)z ≡ x(yz)$<br>$(x+y)+z ≡ x+(y+z)$                     | Move brackets                             |
| Distribution  | $x ∧ (y ∨ z) ≡ (x∧y)∨(x∧z)$<br>$x ∨ (y ∧ z) ≡ (x∨y)∧(x∨z)$ | Multiplications<br>AND -> OR<br>OR -> AND |
| Absorption    | $x ∧ (x ∨ y) ≡ x$                                          |                                           |
| de Morgan     | $¬(x ∧ y) ≡ ¬x ∨ ¬y$                                       | Flip operator                             |
| Equivalence   | $x ≡ y ≡ (x ⇒ y) ∧ (y ⇒ x)$                                | Two-way                                   |
| Implication   | $x ⇒ y ≡ ¬x ∨ y$                                           | one-way                                   |
| Involution    | $¬¬x ≡ x$                                                  |                                           |



---
#Maths #Boolean 