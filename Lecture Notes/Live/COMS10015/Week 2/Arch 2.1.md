---
Date & Time: 28-09-2026 09:09
Lecturer:
  - Daniel Page
Course Name:
  - COMS10015
Lecture Name:
---
## Introduction
$\hat X \rightarrow X$, where $\hat X$ is the representation of X, and $X$ is the value

## Endianness
- Little Endian: Smaller value first
- Big Endian: Big value first
E.g. $X = 11101011$
Small: $11010111$
Big: $11101011$

- Least Significant Bit (LSB): Smallest value
- Most Significant Bit (MSB): Largest value

## Hamming
- Hamming Weight: No. of bits = 1
- $\sum_{i=0}^{n-1} X_i$
- Hamming Distance: number of bits in X that diﬀer from the corresponding bit in Y
- $\sum_{i=0}^{n-1} X_i \oplus Y_i$

## Positional Number System
- Express the value of a number $x$ using a base-*b*
- $\sum_{i=0}^{n-1} x̂_i \cdot b^i$
⚠️ If $b > 10$, use letters to represent values > 9

### Unsigned Binary
- Left Shift: Multiplication by $b^y$ (Notated by $<<$)
- Right Shift: Division $b^y$ (Notated by $>>$)

| Aim                    | Operation                                |
| ---------------------- | ---------------------------------------- |
| Set bits               | $x \vee (1 \ll i)$ or $x \vee (0 \ll i)$ |
| Extract Bits           | $(x \gg i) \land 1$                      |
| Extract m-bit sub-word | $(x \gg i) \land ((1 \ll m) -1)$         |

### Signed Binary
| Name             | Description                        | Formula                                                               | Example                           |
| ---------------- | ---------------------------------- | --------------------------------------------------------------------- | --------------------------------- |
| Sign-Magnitude   | First bit: Sign<br>Rest: Positive  | $(-1)^{\hat x_{n-1}} \cdot \sum^{n-2}_{i=0}{\hat x_i \cdot 2^i}$      | $1111 1011_{(2)}$ = $-123_{(10)}$ |
| Two's Complement | First bit: Sign<br>Rest: -256+.... | $\hat x_{n-1} \cdot -2^{n-1} + \sum^{n-2}_{i=0} {\hat x_i \cdot 2^i}$ | $1000 0101_{(2)}$ = $-123_{(10)}$ |





---
#Binary #Architecture