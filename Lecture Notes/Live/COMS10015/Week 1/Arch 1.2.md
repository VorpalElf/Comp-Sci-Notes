---
Date & Time: 21-09-2026 13:04
Lecturer:
  - Daniel Page
Course Name:
  - COMS10015
Lecture Name: Introduction
---
## Introduction
Proposition is a statement where
1. can be evaluated to yield a truth value: <mark style="background: #FFB86CA6;">True or false</mark>
2. must be <mark style="background: #FF5582A6;">unambiguous</mark> (e.g. it's too hot, but the temperature is 20˚C instead)
3. can include <mark style="background: #FFF3A3A6;">free variables</mark> (e.g. the temperature is $x$˚C)
4. can be represented using <mark style="background: #BBFABBA6;">short-hand variable</mark> or function (e.g. $g(x) = x˚$C)

| Common | Prof.                                                             | Notation   |
| ------ | ----------------------------------------------------------------- | ---------- |
| NOT    | Negation                                                          | ¬          |
| AND    | Conjunction                                                       | ∧          |
| OR     | <mark style="background: #FFB86CA6;">Inclusive</mark> Disjunction | ∨          |
| XOR    | <mark style="background: #FFB8EBA6;">Exclusive</mark> Disjunction | $\oplus$   |
|        | Implication                                                       | $\implies$ |
|        | Equivalence                                                       | ≡          |
- Truth table: Statement of the expression

## Boolean Algebra
1. Work with the set $\mathbb{B} = {0,1}$ of binary digits, to represent true or false
2. Shorten every statement into either a variable or function
3. Functional completeness
4. Manipulate expressions according to rules

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
#Boolean #Architecture