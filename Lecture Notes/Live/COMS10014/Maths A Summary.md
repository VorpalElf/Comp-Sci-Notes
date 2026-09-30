## Week 1: Boolean Algebra
| Name        | Common        | Definition                                        | Notations      |
| ----------- | ------------- | ------------------------------------------------- | -------------- |
| Conjunction | AND           | Both propositions must be true                    | $p \land q$    |
| Disjunction | OR            | Either proposition is true                        | $p \lor q$     |
| Negation    | NOT           | Only one input, flip false to true, true to false | $\neg p$       |
| Implication | IF... THEN... |                                                   | $p \implies q$ |
### Operator Precedence
1. Parentheses
2. Negation
3. Conjunction
4. Disjunction
5. Implication
E.g. $p \land q \lor r$  means $(p \land q) \lor r$
💡 Treat AND as $\times$, OR as $+$

### Laws of Boolean Algebra
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

## Week 2: Natural Deduction
- Propositions as evidence
- Proof $\approx$ providing evidence
- Assumption: A condition under which we believe the goal follows
- Goal: Proposition trying to prove

|               | Introduction                          | Elimination                                                                            |
| ------------- | ------------------------------------- | -------------------------------------------------------------------------------------- |
| Definition    | Constructs information  required      | Extract information based on assumption and prove something else                       |
| $\Rightarrow$ | Assume $\phi$ and $\psi$ prove $\psi$ | If we have $\phi \Rightarrow \psi$ and we have $\phi$, we may conclude $\psi$          |
| $\land$       | Prove both $\phi$ and $\psi$          | If we have $\phi \land \psi$, we may conclude $\phi$ and separately conclude $\psi$    |
| $\lor$        | Prove $\phi$ and/or $\psi$            | Assuming either $\phi$ or $\psi$, we may prove $\rho$                                  |
| $\neg$        | Assume $\phi$ and derive $\bot$       | If we have both $\phi$ and $\neg \phi$, we may conclude any proposition $\psi$ we like |
| $\top$        | We can always derive $\top$           |                                                                                        |
| $\bot$        |                                       | If we have $\bot$, we may conclude any proposition                                     |
|               |                                       |                                                                                        |
⭐️ LEM: $\phi \equiv \phi \lor \neg \phi$
💡Assume $p$ is true for $\Rightarrow$, as consequent always true if antecedent is false
