---
Date & Time: 21-09-2026 11:06
Lecturer:
  - Eddie Jones
Course Name:
  - COMS10014
Lecture Name: Boolean & Truth Tables
---
## Booleans
- Basic data type of Computer Science
- Proposition: Statement / Condition that is either true or false
- True : $\top$, False: $\bot$

## Truth Tables
- Expression of Boolean functions

| Night Option | Past 5pm | Night Mode |
| ------------ | -------- | ---------- |
| $\bot$       | $\bot$   | $\bot$     |
| $\bot$       | $\top$   | $\bot$     |
| $\top$       | $\bot$   | $\bot$     |
| $\top$       | $\top$   | $\top$     |

## Operations

| Name        | Common        | Definition                                        | Notations      |
| ----------- | ------------- | ------------------------------------------------- | -------------- |
| Conjunction | AND           | Both propositions must be true                    | $p \land q$    |
| Disjunction | OR            | Either proposition is true                        | $p \lor q$     |
| Negation    | NOT           | Only one input, flip false to true, true to false | $\neg p$       |
| Implication | IF... THEN... |                                                   | $p \implies q$ |


## Implication
$p \Rightarrow q \equiv \neg p \lor q$

| p      | q      | $p \Rightarrow q$ | Examples                                            |
| ------ | ------ | ----------------- | --------------------------------------------------- |
| $\bot$ | $\bot$ | $\top$            | Didn't rain, so promise not broken (vacuously true) |
| $\bot$ | $\top$ | $\top$            | Didn't rain, so promise not broken (vacuously true) |
| $\top$ | $\bot$ | $\bot$            | Did rain but no umbrella                            |
| $\top$ | $\top$ | $\top$            | Did rain and brought umbrella                       |
- E.g. p = rain, q bring umbrella
- ⚠️ Convention: $p \Rightarrow q \Rightarrow r \equiv p \Rightarrow (q \Rightarrow r)$
- Vacuous: Makes no real claim about the world

## Operator Precedence
1. Parentheses
2. Negation
3. Conjunction
4. Disjunction
5. Implication
E.g. $p \land q \lor r$  means $(p \land q) \lor r$
💡Treat AND as $\times$, OR as $+$

## Associativity
- Operations that are interchangeable
- $(p \land q) \land r ≡ p \land (q \land r)$

## Trees

![[Screenshot 2026-09-21 at 11.34.59 AM.png]]
![[Screenshot 2026-09-21 at 11.38.51 AM.png]]

## Functional Completeness
- Functions that could express any arbitrary Boolean function
- E.g. $\land, \lor$ and $\neg$
- XOR is derived from these operators


---
#Maths #Logic #Boolean