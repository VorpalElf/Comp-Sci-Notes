---
Date & Time: 12-09-2026 23:27
Lecturer:
  - Daniel Page
Course Name:
  - COMS10015
Lecture Name: Integer Representation
---
## Endian
- Little Endian: Right to left $⟨X_0, X_1, X_2, X_3, X_4, X_5, X_6⟩$
- Big Endian: Left to right $⟨X_6, X_5, X_4, X_3, X_2, X_1, X_0⟩$
- Most Significant Bit: Heaviest bit
- Least Significant Bit: Lightest bit

## Hamming
- Hamming Weight: No. of bits = 1
- $\sum_{i=0}^{n-1} X_i$
- Hamming Distance: number of bits in X that diﬀer from the corresponding bit in Y
- $\sum_{i=0}^{n-1} X_i \oplus Y_i$

## Positional Number System
- Express the value of a number $x$ using a base-*b*
- $\sum_{i=0}^{n-1} x̂_i \cdot b^i$
⚠️ If $b > 10$, use letters to represent values > 9

### Numeric Operations
- Left Shift: Multiplication by $b^y$
- Right Shift: Division $b^y$
- 




---
