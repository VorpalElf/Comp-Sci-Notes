---
Date & Time: 09-11-2026 11:01
Lecturer:
  - Xiyue Zhang
Course Name:
  - COMS10014
Lecture Name: Combinatorics
---
## Counting Rules
### Product Rule
- Involve independent stages
- E.g. 10 choices, then another 26 choices $\Rightarrow 10 \times 26$
### Sum Rule
- Can do either options
- E.g. username with 3 digits or 3 letters $\Rightarrow 10^3 + 26^3$

## Permutations & Factorials
#### Factorial
$$n! = 1 \times 2 \times ... \times n, \space n \in \mathbb{N}$$ with 0! = 1

#### Permutations
Choose and arrange $m$ distinct elements out of $n$
$$P(n,m) = \frac{n!}{(n-m!)}$$
E.g. How many 3-place prize winners can be awarded among 12 finalists?
$$P(12,3) = 12 \times 11 \times 10 = 1320$$
#### Permutations with Repetition
- I.e. independent permutation stages
$$\frac{n!}{n_1! \times n_2! \times ... \times n_k!} = \frac{n!}{n_1!} \times \frac {n!}{n_2!} \times ...$$
E.g. No. of distinct permutations for `BALLOON`
$$= \frac{7!}{2!\times5!}$$


## Restricted Permutations
#### Relative-order Constraints
E.g. Arrange all letters for `ALGORITHM`, where A before M
1. 9 Letters to arrange $\Rightarrow 9!$
2. Only half of the permutations matches the case $\Rightarrow \frac{1}{2}$
3. Multiply $\Rightarrow \frac{9!}{2}$
#### Adjacency Constraints
E.g. 8 students line up and two particular students must sit together
1. 7 blocks to arrange (6 students + 1 pair) $\Rightarrow 7!$
2. Inside the pair, students could swap positions $\Rightarrow 2!$
3. Multiply $\Rightarrow 7! \times 2!$
#### Circular Arrangements
E.g. Seating around a round table with no distinguished first seat




---
