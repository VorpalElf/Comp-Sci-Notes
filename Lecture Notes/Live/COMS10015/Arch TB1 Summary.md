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


---
#Summary #Architecture