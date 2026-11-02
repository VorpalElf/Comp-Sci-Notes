---
Date & Time: 02-11-2026 11:05
Lecturer:
  - Xiyue Zhang
Course Name:
  - COMS10014
Lecture Name: Induction
---
## Introduction
- To solve questions with infinite many cases
- Use direct when $P \Rightarrow Q$

## Prove by Induction
1. Prove base case
2. Prove $S(n) \Rightarrow S(n+1)$, with $n$ a free variable
💡If starting from $n $\geq k$, change the base case to $k$
💡If proving $L(n) = R(n)$, try expand $R(n+1)$ first in case you're stuck

## Well-Ordering
- If $S(x)$ is false for $x \in \mathbb{N}$, there should be a smallest value of such $x$
- If can't such $x$ term doesn't exists, then prove by induction must work

## Structure Induction
E.g. Prove $P$ holds for all objects of a recursively defined type
1. Base case: Show $P$ holds for every object in the basic rule
2. Induction: Assume Z from A...B, prove $P(A), P(B)...$ then $P(Z)$ is true
### Rules
1. Value Term: An integer
2. Variable Term: A free variable
3. Operation Term: 
4. 



---
