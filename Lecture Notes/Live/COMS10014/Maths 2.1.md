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


|               | Introduction                          | Elimination                                                                         |
| ------------- | ------------------------------------- | ----------------------------------------------------------------------------------- |
| Definition    | Constructs information  required      | Extract information based on assumption and prove something else                    |
| $\Rightarrow$ | Assume $\phi$ and $\psi$ prove $\psi$ | If we have $\phi \Rightarrow \psi$ and we have $\phi$, we may conclude $\psi$       |
| $\land$       | Prove both $\phi$ and $\psi$          | If we have $\phi \land \psi$, we may conclude $\phi$ and separately conclude $\psi$ |
| $\lor$        | Prove $\phi$ and/or $\psi$            |                                                                                     |
💡Assume $p$ is true for $\Rightarrow$, as consequent always true if antecedent is false



Introduction:
- To prove $\phi \Rightarrow \psi$, <mark style="background: #FFB86CA6;">assume</mark> $\phi$ is true, <mark style="background: #ABF7F7A6;">then prove</mark> $\psi$
- Use facts that we already have
<mark style="background: #FFB86CA6;">Assumption</mark>, <mark style="background: #ABF7F7A6;">goal</mark>


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
#Maths #Incomplete