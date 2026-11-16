---
Date & Time: 09-11-2026 13:04
Lecturer:
  - Daniel Page
Course Name:
  - COMS10015
Lecture Name: Finite State Machines
---
## Introduction
- A model of computation
- Act like a flow chart
1. Input
2. Syntax & Semantics Check
3. Output (i.e. change some states)
#### Components
1. Finite set of states $S$, which include a starting state $s$
2. Finite set of accepting states $A$, where $A \subseteq S$
3. Input & Output alphabet, $\Sigma, \Gamma$
4. Transition Function (i.e. change states)
$$\delta = S \times \Sigma \rightarrow S$$
5. Output Function
- Moore: $\omega = S \rightarrow \Gamma$
- Mealy: $\omega = S \times \Sigma \rightarrow \Gamma$
#### Examples
Decides whether a binary sequence $X$ has an odd number of '1' elements
![[Screenshot 2026-11-09 at 1.32.06 PM.png|457]]

## Applications
#### Regex
![[Screenshot 2026-11-09 at 1.41.13 PM.png|514]]
![[Screenshot 2026-11-09 at 1.41.28 PM.png|509]]
#### TCP
![[Screenshot 2026-11-09 at 1.42.22 PM.png|447]]
![[Screenshot 2026-11-09 at 1.44.17 PM.png|489]]



---
#FSM