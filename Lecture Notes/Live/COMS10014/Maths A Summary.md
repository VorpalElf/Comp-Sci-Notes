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
| Definition    | Constructs information required       | Extract information based on assumption and prove something else                       |
| $\Rightarrow$ | Assume $\phi$ and $\psi$ prove $\psi$ | If we have $\phi \Rightarrow \psi$ and we have $\phi$, we may conclude $\psi$          |
| $\land$       | Prove both $\phi$ and $\psi$          | If we have $\phi \land \psi$, we may conclude $\phi$ and separately conclude $\psi$    |
| $\lor$        | Prove $\phi$ and/or $\psi$            | Assuming either $\phi$ or $\psi$, we may prove $\rho$                                  |
| $\neg$        | Assume $\phi$ and derive $\bot$       | If we have both $\phi$ and $\neg \phi$, we may conclude any proposition $\psi$ we like |
| $\top$        | We can always derive $\top$           |                                                                                        |
| $\bot$        |                                       | If we have $\bot$, we may conclude any proposition                                     |
|               |                                       |                                                                                        |
⭐️ LEM: $\phi \lor \neg \phi \equiv \top$
💡Assume $p$ is true for $\Rightarrow$, as consequent always true if antecedent is false

## Week 3: Predicates & Qualifiers
### Predicates
- Statements that contain variables
- Can have any number of variables
- E.g. The temperature is greater than 18˚C
### Quantifiers
- A way to create a proposition from a propositional function
- Domain: The set of values that a variable can take
### Universal
 - $\forall$, "for all" elements
 - $\forall x \space P(x)$ is true, if all elements are true
 - $\forall x \space P(x) \equiv P(x_1) \land P(x_2) \land \space ...$
### Existential
- $\exists$, one or more elements in the domain
- True if any values of $x$ is true
- The true $x_n$ is called a witness
- $\forall x \space P(x) \equiv P(x_1) \lor P(x_2) \lor \space ...$
### Empty Domains
- $\forall x \space P(x)$ is vacuously true, because no elements are false
- $\exists x \space P(x)$ is trivially false, because no elements are true
### De Morgan's Laws for Quantifiers
$\neg \forall x \space P(x) \equiv \exists x \space \neg P(x)$
$\neg \exists x \space Q(x) \equiv \forall x \space \neg Q(x)$
- Move negations, change operators
## Proofs
### Prove Strategies
| Strategy         | Goal              | Approach                         |
| ---------------- | ----------------- | -------------------------------- |
| Direct           | $P \Rightarrow Q$ | Assume $P$, derive $Q$           |
| Indirect         | $P \Rightarrow Q$ | Assume $\neg Q$, derive $\neg P$ |
| Contradiction    | Prove P           | Assume $\neg P$, derive $\bot$   |
| Case Distinction | Prove P           | Split into exhaustive cases      |
### Informal Proofs
| Informal Strategy                 | Key rule(s)                     | How                                       |
| --------------------------------- | ------------------------------- | ----------------------------------------- |
| Direct proof of $P \Rightarrow Q$ | $\Rightarrow I$                 | Assume $P$, derive $Q$                    |
| Applying $P \Rightarrow Q$ to $P$ | $\Rightarrow E$                 | $Q$ (modus ponens)                        |
| Indirect proof (Contrapositive)   | $\Rightarrow I, \neg I, \neg E$ | Prove $\neg Q \Rightarrow \neg P$ instead |
| Proof by contradiction            | LEM, $\neg E$                   | Split $P \lor \neg P$, rule out $\neg P$  |
| Case Distinction                  | $\lor E$                        | Prove goal in each case                   |

### Quantifiers Proof
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
#Summary