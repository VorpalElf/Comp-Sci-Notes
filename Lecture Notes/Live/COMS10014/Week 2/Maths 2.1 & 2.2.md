---
Date & Time: 28-09-2026 11:05
Lecturer:
  - Eddie Jones
Course Name:
Lecture Name: Natural Deduction
---
## Introduction
$\sqrt 2$ cannot be expressed as a fraction

E.g. Prove $2(x+3) -6 = 2x$
$$=2x+6-6$$
$$=2x$$

## Informal Proofs
- Skip steps
- Have grey areas

## Natural Deduction
- Propositions as evidence
- Proof $\approx$ providing evidence

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
⭐️ LEM: $\phi \lor \neg \phi \equiv \top$
💡Assume $p$ is true for $\Rightarrow$, as consequent always true if antecedent is false

## Examples

| Assumptions                         | Goals                                        | Reasoning                                          |
| ----------------------------------- | -------------------------------------------- | -------------------------------------------------- |
|                                     | $((p \Rightarrow p) \Rightarrow q) \equiv q$ |                                                    |
| $((p \Rightarrow p) \Rightarrow q)$ | $q$                                          |                                                    |
|                                     | $p \Rightarrow p$                            | If we can show $p \Rightarrow p$, $q$ must be true |
| $p$                                 | $p$                                          | Done ✅                                             |
Conclusion
$$\because p \Rightarrow p$$
$$ \therefore q$$




---
#Maths