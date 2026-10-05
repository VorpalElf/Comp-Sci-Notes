---
Date & Time: 05-10-2026 13:01
Lecturer:
  - Daniel Page
Course Name:
  - COMS10015
Lecture Name: Combinatorial Logic (1)
---
## Special-purpose Design Patterns
### 1. Reuse
- $r = x \land y$ and $r' = x \land y$. Then rewrite as $r = r'$
- Called Common Sub-expression Elimination (CSE)
### 2. Decomposition
- Divide big problem into smaller problems
- E.g. $f: \mathbb{B} ^n \rightarrow \mathbb{B} ^m$. Then $f_i$ are such that
$$
f_0: \mathbb{B} ^n \rightarrow \mathbb{B} ^m \newline
$$
$$f_1: \mathbb{B} ^n \rightarrow \mathbb{B} ^m$$
$$f_{m-1}: \mathbb{B} ^n \rightarrow \mathbb{B} ^m$$
### 3. Independent Replication
- Repeat same elements
- $r_i = x_i \land y_i$
- For $n = 4$, this means
$$ r_0 = x_0 \land y_0$$
$$r_1 = x_1 \land y_1$$
$$r_2 = x_2 \land y_2$$
$$r_3 = x_0 \land y_3$$
### 4. Dependent Replication
$r = \land^{n-1}_{i=0} \space x^i$ is computed via $r = x_0 \land (x_1 \land ... (x_{n-1}))$
For $n=4$, this means
$$r = x_0 \land (x_1 \land x_2 \land (x_3)) $$
$$r = (x_0 \land x_1) \land (x_2 \land x_3) $$
## Special-purpose Building Blocks
### Choice
![[Telephony_multiplexer_system.gif]]
#### 1. Multiplexer
- has $m$ inputs
- has 1 output
- uses a $log_2(m)$ bit control signal input to choose which input is connected to the output (e.g. clock)
#### 2. Demultiplexer
- has 1 input
- has m outputs
- uses a $log_2(m)$ bit control signal input to choose which output is connected to the input (e.g. clock)
⭐️ Inputs & Outputs should match the same bit length
### Addition
#### 1. Half Adder
- 2 inputs: x and y
- computes the 2-bit result $x+y$
- 2 ouputs: sum $s$, and a carry out $co$
#### 2. Full Adder
- 3 inputs: x, y, and carry in $ci$
- computes $x+y+ci$
- 2 ouputs: sum $s$, and a carry out $co$
⭐️ Inputs & Outputs are 1-bit

### Comparison
#### Equality Comparator
- 2 inputs
- Check if both values are equal
- Computes an output
#### Less-than Comparator
- 2 inputs
- Check if a value is smaller than the latter
- Computes an output
### Control
#### Translation
![[Screenshot 2026-10-05 at 1.44.26 PM.png|564]]

Encoder: $n$-bit input $\rightarrow$ $m$-bit code word
Decoder: $m$-bit code word $\rightarrow$ $n$-bit input

### Summary

| Name                 | Definition | Expression                                                                                                                               | Circuit                                           |
| -------------------- | ---------- | ---------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------- |
| Multiplexer          |            | $r = (\neg c \land x) \lor (c \land y)$                                                                                                  | ![[Screenshot 2026-10-05 at 1.27.44 PM.png\|126]] |
| Demultiplexer        |            | $r_0 = \neg c \land x$<br>$r_1 = c \land x$                                                                                              | ![[Screenshot 2026-10-05 at 1.27.58 PM.png\|170]] |
| Half Adder           |            | $co = x \land y$<br>$s = x \oplus y$                                                                                                     | ![[Screenshot 2026-10-05 at 1.34.31 PM.png\|160]] |
| Full Adder           |            | $co = (x \land y) \lor (x \land ci) \lor (y \land ci)$<br>$= (x \land y) \lor ((x \oplus y) \land ci)$<br><br>$s = x \oplus y \oplus ci$ | ![[Screenshot 2026-10-05 at 1.34.55 PM.png\|117]] |
| Equality Comparator  |            | r = $\neg (x \oplus y)$                                                                                                                  |                                                   |
| Less-than Comparator |            | r = $\neg x \land y$                                                                                                                     |                                                   |



---
#Architecture 