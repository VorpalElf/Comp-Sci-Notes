---
Date & Time: 15-10-2026 11:03
Lecturer:
  - Daniel Page
Course Name:
  - COMS10015
Lecture Name: Sequential Logic (3)
---
## Introduction
![[Screenshot 2026-10-15 at 11.07.38 AM.png]]
- Each word takes $w$ bits

## Memory
- Constructed from
1. Memory array of replicated cells
2. Row Decoder
3. Column Decoder
⭐️ Decoder: (De)activates address in the array

And some signal-compatibility infrastructure
1. Bit line conditioning
	- Ensure bit lines are strong enough
2. Sense amplifiers
	- Ensure output from array is usable

|                      | Static RAM (SRAM)                                                      | Dynamic RAM (DRAM)                                                      |
| -------------------- | ---------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| Manufacture          | Low Density                                                            | High Density                                                            |
| Cost                 | Expensive                                                              | Cheap                                                                   |
| Access Time          | Fast                                                                   | Slow                                                                    |
| Interface Difficulty | Easy                                                                   | Hard                                                                    |
| Application          | <mark style="background: #FFB86CA6;">Latency</mark> optimised contexts | <mark style="background: #BBFABBA6;">Capacity</mark> optimised contexts |
### SRAM
![[Screenshot 2026-10-15 at 11.21.07 AM.png|266]]![[Screenshot 2026-10-15 at 11.21.32 AM.png|269]]

- 2 NOT gates
- Bit lines: $bl$ and $\neg bl$
- Word line: $wl$
- 6T SRAM $=$ 6 transistors needed

### DRAM
![[Screenshot 2026-10-15 at 11.25.48 AM.png|396]]
- One transistor & one <mark style="background: #FF5582A6;">capacitor</mark>
- Simpler design $\Rightarrow$ Easy to manufacture
- Slow because of discharge of transistors

## Designs
|           | SRAM                                                                                    | DRAM |
| --------- | --------------------------------------------------------------------------------------- | ---- |
| Interface |                                                                                         |      |
| Read      | - Drive address onto A<br>- set WE = false, OE = true, CS = true                        |      |
| Write     | - Drive data onto D<br>- Drive address onto A<br>- set WE = true, OE = false, CS = true |      |
| Diagram   | ![[Screenshot 2026-10-15 at 11.38.20 AM.png]]                                           |      |


---
#Architecture #Incomplete