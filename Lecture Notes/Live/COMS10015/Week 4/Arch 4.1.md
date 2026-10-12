---
Date & Time: 12-10-2026 09:09
Lecturer:
  - Daniel Page
Course Name:
  - COMS10015
Lecture Name: Sequential Logic (1)
---
## Introduction
- Output is a function of the input
- Computation viewed discretely (i.e. step-by-step)

## Clock
![[Screenshot 2026-10-12 at 9.12.54 AM.png|554]]
- Signal that oscillates between 1 & 0
- An input / Produced internally by a clock generator
- Used to
	1. Trigger Events
	2. Synchronise components
- Clock frequency should be sufficient for fast & slow operations

## Bistable Components
It can
- Retain some current state $Q$
- Be updated to some next state $Q'$
under control of **enable signal**
1. Level-triggered: Updated by a given level (i.e. **latch**)
2. Edge-triggered: Update by a given edge (i.e. **flip-flop**)
Described with excitation table


---
#Architecture