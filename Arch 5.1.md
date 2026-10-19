---
Date & Time: 19-10-2026 09:07
Lecturer:
  - Daniel Page
Course Name:
  - COMS10015
Lecture Name: Verilog (1)
---
## Hardware Description Language (HDL)
1. Facilitate automation
	- Simulation
	- Verification
	- Translation
2. Address the challenge of scale

## Verilog
```Verilog
GATE t0( OUTPUT, INPUT1, INPUT2)
```
Example

![[Screenshot 2026-10-19 at 9.22.45 AM.png|357]]
```v
module fa(output wire co, output wire s, input wire ci, input wire x, input wire y)

wire w0, w1, w2;

xor t0( w0, x, y);
and t1()
```
### Levels of Verilog
1. Switch Level
	- `pmos( t, VDD, b)`
2. Gate Level
	- `nor t( a, b, c)` 
3. Register Transfer Level
	- `assign a = ~(b | c)`
	- Continuously drive the wire with the result
4. Behavioural-level Verilog
	- `a = ~(b | c)`
	- A register equals to the result of the evaluation

## Wires & Values
- Wire: Form of **net** used to <mark style="background: #FFB86CA6;">communicate values</mark>
- `wire [7:0] x;`
- Values
	1. Support concept of 3-state logic
		- 0 $\Rightarrow$ 0 (i.e. logical false)
		- 1 $\Rightarrow$ 1 (i.e. logical true)
		- $X \Rightarrow$ <mark style="background: #FF5582A6;">unknown</mark> (i.e. neither 1 or 0)
		- $Z \Rightarrow$ <mark style="background: #ADCCFFA6;">high impedance</mark> (i.e. Disconnected)
	2. Can be written in binary, decimal or hexadecimal
		- 2'b10  $\Rightarrow$ a 2-bit binary literal, with the value $10_2$
		- 8'd17  $\Rightarrow$ a 8-bit decimal literal, with the value $17_{10}$
		- 4'hF  $\Rightarrow$ a 4-bit hexadecimal literal, with the value $F_{16}$
	3. Can include 3-state values on a per-bit basis
		- 1'bX $\Rightarrow$ a 1-bit binary literal, the bit is unknown
		- 4'b10X $\Rightarrow$ a 4-bit decimal literal, that are 1, 0, unknown and high impedance

| Name        | Diagram                                           |
| ----------- | ------------------------------------------------- |
| Subscript   | ![[Screenshot 2026-10-19 at 1.14.02 PM.png]]      |
| Concatenate | ![[Screenshot 2026-10-19 at 1.14.47 PM.png\|383]] |
| Replicate   | ![[Screenshot 2026-10-19 at 1.15.11 PM.png\|342]] |



---
#Architecture