---
Date & Time: 31-08-2026 23:58
Lecturer:
  - Daniel Page
Course Name:
  - COMS10015
Lecture Name: Boolean Algebra
---
## Introduction
Proposition is a statement where
1. can be evaluated to yield a truth value: <mark style="background: #FFB86CA6;">True or false</mark>
2. must be <mark style="background: #FF5582A6;">unambiguous</mark>
3. can include <mark style="background: #FFF3A3A6;">free variables</mark>
4. can be represented using <mark style="background: #BBFABBA6;">short-hand variable</mark> or function

| Common | Prof.                                                             | Notation                                                                                                                          |
| ------ | ----------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| NOT    | Negation                                                          | ¬                                                                                                                                 |
| AND    | Conjunction                                                       | ∧                                                                                                                                 |
| OR     | <mark style="background: #FFB86CA6;">Inclusive</mark> Disjunction | ∨                                                                                                                                 |
| XOR    | <mark style="background: #FFB8EBA6;">Exclusive</mark> Disjunction | ![{\displaystyle \oplus }](https://wikimedia.org/api/rest_v1/media/math/render/svg/8b16e2bdaefee9eed86d866e6eba3ac47c710f60)      |
|        | Implication                                                       | ![{\displaystyle \Rightarrow }](https://wikimedia.org/api/rest_v1/media/math/render/svg/469b737d167b9b28a74e27c7f5e35b5ea9256100) |
|        | Equivalence                                                       | ≡                                                                                                                                 |
## Simplifications
| Name          | Axiom(s)                                               | Hints 💡                                  |
| ------------- | ------------------------------------------------------ | ----------------------------------------- |
| Commutativity | x ∧ y ≡ y ∧ x                                          |                                           |
| Association   | (x ∧ y) ∧ z ≡ x ∧ (y ∧ z)<br>(x ∨ y) ∨ z ≡ x ∨ (y ∨ z) | Move brackets                             |
| Distribution  | x ∧ (y ∨ z) ≡ (x∧y)∨(x∧z)<br>x ∨ (y ∧ z) ≡ (x∨y)∧(x∨z) | Multiplications<br>AND -> OR<br>OR -> AND |
| Absorption    | x ∧ (x ∨ y) ≡ x                                        |                                           |
| de Morgan     | ¬(x ∧ y) ≡ ¬x ∨ ¬y                                     | Flip operator                             |

| Name        | Axiom 1    | Axiom 2    |
| ----------- | ---------- | ---------- |
| Identity    | x ∧ 1 ≡ x  | x ∨ 0 ≡ x  |
| Null        | x ∧ 0 ≡ 0  | x ∨ 1 ≡ 1  |
| Idempotency | x ∧ x ≡ x  | x ∨ x ≡ x  |
| Inverse     | x ∧ ¬x ≡ 0 | x ∨ ¬x ≡ 1 |





---
#Boolean 