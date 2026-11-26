---
Date & Time: 26-11-2026 11:23
Lecturer:
  - Daniel Page
Course Name:
  - COMS10015
Lecture Name: Register Machines (2)
---
## Introduction
| Term                 | Definition                                                                                                                                                  |
| -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Program Counter      | <mark style="background: #FFB86CA6;">Special purpose register</mark> that holds the <mark style="background: #BBFABBA6;">next address</mark> to be executed |
| Instruction Register | Holds the instruction <mark style="background: #FFF3A3A6;">currently</mark> being executed                                                                  |
| Instruction Decoder  |                                                                                                                                                             |

## Fetch-Decode-Execute Cycle
1. Fetch Stage
	a) Load instruction into IR
	b) Increment PC
2. Decode Stage
	a) Decode IR into control signals
3. Execute Stage
	a) Execute decoded instruction
====================================
4. Memory Access Stage
	a) Perform any memory accesses required
5. Write-back Stage
	a) Store results from computation



---
