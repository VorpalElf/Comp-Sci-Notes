## Boolean Algebra

| Name        | Axiom 1          | Axiom 2             |
| ----------- | ---------------- | ------------------- |
| Identity    | $x \land 1 ≡ x$  | $x \lor 0 ≡ x$      |
| Null        | $x \land 0 ≡ 0$  | $x \lor 1 ≡ 1$      |
| Idempotency | $x \land x ≡ x$  | $x \lor x ≡ x$      |
| Inverse     | $x \land ¬x ≡ 0$ | $x \lor \neg x ≡ 1$ |

| Name          | Axiom(s)                                                   | Hints 💡                                  |
| ------------- | ---------------------------------------------------------- | ----------------------------------------- |
| Commutativity | $x ∧ y ≡ y ∧ x$                                            | Same thing                                |
| Association   | $(x ∧ y) ∧ z ≡ x ∧ (y ∧ z)$<br>$(x ∨ y) ∨ z ≡ x ∨ (y ∨ z)$ | Move brackets                             |
| Distribution  | $x ∧ (y ∨ z) ≡ (x∧y)∨(x∧z)$<br>$x ∨ (y ∧ z) ≡ (x∨y)∧(x∨z)$ | Multiplications<br>AND -> OR<br>OR -> AND |
| Absorption    | $x ∧ (x ∨ y) ≡ x$                                          |                                           |
| de Morgan's   | $¬(x ∧ y) ≡ ¬x ∨ ¬y$                                       | Flip operator & extract NOT               |
| Equivalence   | $x ≡ y ≡ (x ⇒ y) ∧ (y ⇒ x)$                                | Two-way                                   |
| Implication   | $x ⇒ y ≡ ¬x ∨ y$                                           | one-way                                   |
| Involution    | $¬¬x ≡ x$                                                  |                                           |

---
#Summary #Architecture