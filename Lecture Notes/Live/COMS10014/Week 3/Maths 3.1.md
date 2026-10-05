---
Date & Time: 05-10-2026 11:04
Lecturer:
  - Xiyue Zhang
Course Name:
  - COMS10014
Lecture Name: Predicates & Quantifiers
---
## Introduction
Atomic Propositions: Statements that are True or False

## Predicates
- Statements that contain variables
- Can have any number of variables
- E.g. The temperature is greater than 18˚C

## Quantifiers
- A way to create a proposition from a propositional function
- Domain: The set of values that a variable can take
- Assume $x$ is the universe
### Universal
 - $\forall$, "for all" elements
 - $\forall x \space P(x)$ is true, if all elements are true
 - $\forall x \space P(x) \equiv P(x_1) \land P(x_2) \land \space ...$
 - 
### Existential
- $\exists$, one or more elements in the domain
- True if any values of $x$ is true
- The true $x_n$ is called a witness
- $\forall x \space P(x) \equiv P(x_1) \lor P(x_2) \lor \space ...$

### Empty Domains
- $\forall x \space P(x)$ is vacuously true, because no elements are false
- $\exists x \space P(x)$ is trivially false, because no elements are true

## Applications
### Precedence of Quantifiers
- Higher precedence than all connectives
- $\forall x \space P(x) \lor Q(x)$ means $(\forall x \space P(x)) \lor Q(x)$

Bound: A quantifier is used on $x$, within the scope
Free: Not bound
$\alpha$-renaming: Rename bound variables to any other symbols, as long doesn't appear as any free variables

E.g. $\exists x (P(x) \Rightarrow Q(x)) \land \forall x \space R(x)$, all variables are bound
E.g. $\forall x (\exists y (P(y) \lor Q(x, y))  \land R(x,y)$

### De Morgan's Laws for Quantifiers
$\neg \forall x \space P(x) \equiv \exists x \space \neg P(x)$
$\neg \exists x \space Q(x) \equiv \forall x \space \neg Q(x)$
- Move negations, change operators

### Order of Quantifiers
Let mother(x, y) $\equiv$ $x$ is the mother of $y$
- Every person has a mother
$\exists x \space \forall y$ Mother(x,y) means "There is someone who is everyone's mother"

### Translation of Natural Language
1. All Students work hard
2. Some students don't sleep at night
3. There are some hard-working people doesn't sleep at night

Let S(x): x is a student, W(x): x works hard, Sleep(x): x sleeps at night
1. $\forall x (S(x) \Rightarrow W(x))$
2. $\exists x (S(x) \land \neg Sleep(x))$
3. $\exists x (W(x) \land \neg Sleep(x))$


---
#Maths #Incomplete