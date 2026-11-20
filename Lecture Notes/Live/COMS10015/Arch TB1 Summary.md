## Boolean Algebra

| Name        | Axiom 1          | Axiom 2             |
| ----------- | ---------------- | ------------------- |
| Identity    | $x \land 1 ≡ x$  | $x \lor 0 ≡ x$      |
| Null        | $x \land 0 ≡ 0$  | $x \lor 1 ≡ 1$      |
| Idempotency | $x \land x ≡ x$  | $x \lor x ≡ x$      |
| Inverse     | $x \land ¬x ≡ 0$ | $x \lor \neg x ≡ 1$ |

| Name          | Axiom(s)                                                   | Hints 💡                                  |
| ------------- | ---------------------------------------------------------- | ----------------------------------------- |
| Commutativity | $x ∧ y ≡ y ∧ x$                                            | Same thing                                |
| Association   | $(x ∧ y) ∧ z ≡ x ∧ (y ∧ z)$<br>$(x ∨ y) ∨ z ≡ x ∨ (y ∨ z)$ | Move brackets                             |
| Distribution  | $x ∧ (y ∨ z) ≡ (x∧y)∨(x∧z)$<br>$x ∨ (y ∧ z) ≡ (x∨y)∧(x∨z)$ | Multiplications<br>AND -> OR<br>OR -> AND |
| Absorption    | $x ∧ (x ∨ y) ≡ x$                                          |                                           |
| de Morgan's   | $¬(x ∧ y) ≡ ¬x ∨ ¬y$                                       | Flip operator & extract NOT               |
| Equivalence   | $x ≡ y ≡ (x ⇒ y) ∧ (y ⇒ x)$                                | Two-way                                   |
| Implication   | $x ⇒ y ≡ ¬x ∨ y$                                           | one-way                                   |
| Involution    | $¬¬x ≡ x$                                                  |                                           |

## Binary Arithmetic
### Endianness
- Little Endian: Smaller value first
- Big Endian: Big value first
- Least Significant Bit (LSB): Smallest value
- Most Significant Bit (MSB): Largest value
### Hamming
- Hamming Weight: No. of bits = 1
- $\sum_{i=0}^{n-1} X_i$
- Hamming Distance: number of bits in X that diﬀer from the corresponding bit in Y
- $\sum_{i=0}^{n-1} X_i \oplus Y_i$

| Aim                    | Operation                                |
| ---------------------- | ---------------------------------------- |
| Set bits               | $x \vee (1 \ll i)$ or $x \vee (0 \ll i)$ |
| Extract Bits           | $(x \gg i) \land 1$                      |
| Extract m-bit sub-word | $(x \gg i) \land ((1 \ll m) -1)$         |
### Overflow
- Extra bit produced after arithmetic operation
- Bit unable to fit in the register
- Actions: Truncate/clamp the result

## Transistors & Logic Gates
⭐️ P-Type: extra holes (i.e. positive)
⭐️ N-Type: extra electrons (i.e. negative)
![[Screenshot 2026-09-23 at 10.28.06 AM.png|280]]
- Charge flow between channel
- Channel width controlled by p.d.
- MOSFET have induced channels

|                | P-Type MOSFET                                                           | N-Type MOSFET                                                               |
| -------------- | ----------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| Channel        | <mark style="background: #BBFABBA6;">P-Type</mark>                      | <mark style="background: #FF5582A6;">N-Type</mark>                          |
| Body           | <mark style="background: #FF5582A6;">N-Type</mark>                      | <mark style="background: #BBFABBA6;">P-Type</mark>                          |
| Remove PD -> ? | Widens channel -> <mark style="background: #FFB86CA6;">connected</mark> | Narrows channel -> <mark style="background: #D2B3FFA6;">disconnected</mark> |
| Diagram        | ![[Screenshot 2026-09-23 at 10.35.22 AM.png\|152]]                      | ![[Screenshot 2026-09-23 at 10.35.06 AM.png\|158]]                          |

## Combinatorial Logic
![[Telephony_multiplexer_system.gif]]

| Name                 | Definition                                             | Expression                                                                        | Circuit                                           |
| -------------------- | ------------------------------------------------------ | --------------------------------------------------------------------------------- | ------------------------------------------------- |
| Multiplexer          | Select one of the input signals, output to one signal  | $r = (\neg c \land x) \lor (c \land y)$                                           | ![[Screenshot 2026-10-05 at 1.27.44 PM.png\|166]] |
| Demultiplexer        | Select one input signals, output to one of the signals | $r_0 = \neg c \land x$<br>$r_1 = c \land x$                                       | ![[Screenshot 2026-10-05 at 1.27.58 PM.png\|170]] |
| Half Adder           | Component output sum & carry-out                       | $co = x \land y$<br>$s = x \oplus y$                                              | ![[Screenshot 2026-10-05 at 1.34.31 PM.png\|166]] |
| Full Adder           | Half adder that supports carry-in                      | $co = (x \land y) \lor ((x \oplus y) \land ci)$<br><br>$s = x \oplus y \oplus ci$ | ![[Screenshot 2026-10-05 at 1.34.55 PM.png\|157]] |
| Equality Comparator  | Check if both values are equal                         | r = $\neg (x \oplus y)$                                                           | ![[Screenshot 2026-10-20 at 2.46.51 PM.png\|182]] |
| Less-than Comparator | if a value is smaller than the latter                  | r = $\neg x \land y$                                                              | ![[Screenshot 2026-10-20 at 2.47.27 PM.png\|188]] |
![[Screenshot 2026-10-05 at 1.44.26 PM.png|564]]

Encoder: $n$-bit input $\rightarrow$ $m$-bit code word
Decoder: $m$-bit code word $\rightarrow$ $n$-bit input
### Method 1: Truth Table
1. Make truth table
2. Highlight all '1' outputs
3. Deduce expression every row (Use AND as connectives)
4. Combine them together with OR
### Method 2: Karnaugh Maps
1. Draw map
	- Draw 2 maps (assume 0 & 1) for value guessing questions 
	- Draw n maps for n-outputs
2. Highlight '1's in group of 1,2,4,8 and corners
3. Make AND expressions
4. Connect with OR expressions






---
#Summary #Architecture