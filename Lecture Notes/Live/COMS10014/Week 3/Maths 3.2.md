---
Date & Time: 07-10-2026 11:02
Lecturer:
  - Xiyue Zhang
Course Name:
  - COMS10014
Lecture Name: Predicate Logic and Proofs
---
## Syntax
- Variables: VL is a set of variables
- Constants: CL is a set of constants
- Connectives: All connectives from propositional logic
- Functions: FNL is a set of n-nary functions
	- father(x): a function mapping person x to their father
	- day(dd, mm, yyyy): Returns day of the week from date
- Predicates: PL is a set of predicates
## Prove Strategies
| Strategy         | Goal              | Approach                         |
| ---------------- | ----------------- | -------------------------------- |
| Direct           | $P \Rightarrow Q$ | Assume $P$, derive $Q$           |
| Indirect         | $P \Rightarrow Q$ | Assume $\neg Q$, derive $\neg P$ |
| Contradiction    | Prove P           | Assume $\neg P$, derive $\bot$   |
| Case Distinction | Prove P           | Split into exhaustive cases      |
## Informal Proofs
| Informal Strategy                 | Key rule(s)                     | How                                       |
| --------------------------------- | ------------------------------- | ----------------------------------------- |
| Direct proof of $P \Rightarrow Q$ | $\Rightarrow I$                 | Assume $P$, derive $Q$                    |
| Applying $P \Rightarrow Q$ to $P$ | $\Rightarrow E$                 | $Q$ (modus ponens)                        |
| Indirect proof (Contrapositive)   | $\Rightarrow I, \neg I, \neg E$ | Prove $\neg Q \Rightarrow \neg P$ instead |
| Proof by contradiction            | LEM, $\neg E$                   | Split $P \lor \neg P$, rule out $\neg P$  |
| Case Distinction                  | $\lor E$                        | Prove goal in each case                   |

## Quantifiers Proof
### 1. Witness Strategy
- Applies for $\exists x$
- Show example of any elements in set
### 2. Arbitrary Element Strategy
- For $\forall x$
1. Assume $x$ is arbitrary
2. Proof it with any proof strategies
3. Conclude, "since $x$ is arbitrary, *CLAIM$"

### 3. Natural Induction
|           | Introduction                                                                                                                                                                                                      | Elimination                                                                                                  |
| --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| $\forall$ | Let $x$ be an arbitrary element of $D$<br>Make no further assumptions of $x$ beyond $D$<br><br>🚨 $x$ must not be a free variable<br>which ensures x is truly arbitrary and not secretly fixed by some hypothesis | If we have $\forall x$, we can conclude $P(t)$ where $t \in D$                                               |
| $\exists$ | If we have $P(t)$ where $t \in D$, we may conclude & take $t$ as witness                                                                                                                                          | If we have $\exists x$ and from the assumption $P(x_0)$, where $x_0$ is fresh, we may prove and conclude $Q$ |


---
#Maths