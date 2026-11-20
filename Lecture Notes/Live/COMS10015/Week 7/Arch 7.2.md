---
Date & Time: 05-11-2026 11:09
Lecturer:
  - Daniel Page
Course Name:
  - COMS10015
Lecture Name: Integer Arithmetic
---
## Multiplication
1. Operand Scanning
- Iterate outer loop (e.g. $y_i$)
	- Iterate inner loop (e.g. $x_i$)
![[Screenshot 2026-11-05 at 11.13.40 AM.png|324]]

2. Product Scanning
![[Screenshot 2026-11-05 at 11.18.48 AM.png|288]]
- An outer loop steps through $r_k$
- Two inner loop matching $x_i$ and $y_j$, where $i+j = k$

3. Repeated Addition
$$\because 7x = x + x + x + x + x + x + x$$
$$\therefore y \times x = (\sum ^{n-1} _{i=0} y_i \space \cdot 2^i) \times x$$
$$= (y_0 \cdot x \cdot 2^0) \space ... \space (y_{n-1} \cdot x \cdot 2^{n-1})$$

## Circuits
### Combinatorial
$$r = y \times x = y \times x = \sum ^{n-1} _{i=0} y_i \space \cdot 2^i \cdot x$$
where we know that
$t \cdot 2^i \equiv t \ll i$ and $y_i \cdot t$ will be either $0$ or $t$

Hence,
1. Some AND gate to produce a product (e.g. $y_i \cdot x$)
2. Some left shift components to scale the partial products
3. Some adder components to sum the partial scaled products

![[Screenshot 2026-11-05 at 11.36.16 AM.png|546]]
✅ Executed in one step                         ❌ The step is very long
✅ No state control needed                   ❌ Requires large data path

### Sequential
- Start with the general step
$$r^r \leftarrow y_i \cdot x+2 \cdot r$$
- specialise to read
	- If $y_i = 0$, $2 \cdot r \space \equiv (r \ll 1)$
	- If $y_i = 1$, $x+2 \cdot r \equiv \space x + (r \ll 1)$ 
	- Maps it to $r^r$

- using it to accumulate the result step-by-step
![[Screenshot 2026-11-05 at 11.47.02 AM.png|318]]![[Screenshot 2026-11-05 at 11.47.20 AM.png|376]]
![[Screenshot 2026-11-05 at 11.47.44 AM.png|692]]
✅ Smaller data path                                                ❌ Requires large control path (e.g. entire FSM)
✅ Shorter critical path (i.e. each step is shorter)❌ Require more steps


---
