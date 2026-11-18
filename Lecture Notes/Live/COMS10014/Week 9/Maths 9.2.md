---
Date & Time: 18-11-2026 11:05
Lecturer:
  - Eddie Jones
Course Name:
  - COMS10014
Lecture Name: Conditional Probability
---
## Introduction
$$P(A \space|\space B) = \frac{P(A \cap B)}{P(B)}$$
$$\begin{array}{c|ccc|c}
 & <3 & =3 &>3 &\\
\hline
Even & \frac{1}{6} & 0 & \frac{2}{6} & \frac{1}{2} \\
Odd & \frac{1}{6} & \frac{1}{6} & \frac{1}{6} & \frac{1}{2} \\
\hline
& \frac{1}{3} & \frac{1}{6} & \frac{1}{2} & 1 \\
\end{array}$$
$$P(Even \space | \space > 3) = \frac{P(Even \space \cap > 3)}{P (>3)}$$
## Properties
- $P(\emptyset \space | \space B) = 0$
- $P(\space \overline S \space | \space B) = P(S \space | \space B) + P(\space T \space | \space B) \rightarrow P(S \cap T \space | \space B)$
- $P(A) = P(A \cap B) + P(\overline A \cap B) = P(A \space|\space B) \cdot P(B) + P(A\space|\space \overline B) \cdot P(\overline B)$

## Bayes' Theorem
$$\because P(A \space|\space B) = \frac{P(A \cap B)}{P(B)}$$
$$\therefore P(A \space | \space B) = \frac{P(B \space | \space A) \cdot P(A)}{P(B)}$$
- Based on belief updates
### Examples (credits to Kirby)
- Suppose 5% of the population suffers from a disease, a company developed a test that is 90% accurate
- $P(P_0 \space | \space D) = 0.9$ and $P(P_{Ne} \space|\space \overline D) = 0.9$
- $P(D \space|\space P_0) = \frac{P(P_0 \space | \space D) \cdot P(D)}{P(P_0)} = P(P_0 \space|\space D) \cdot P(D) + P(P_0 \space|\space \overline D) \cdot P(D)$
- $0.9 \times 0.05 + 0.1 \times 0.95 = 0.14$
⭐️⭐️⭐️ $$P(A \space|\space B) = \frac{P(B \space | \space A) \cdot P(A)}{P(B)}$$⭐️⭐️⭐️

### Independence
- Two events $A, B \subseteq \Omega$ are independent if $P(A \space | \space B) = P(A) \cdot P(B)$
- $\Leftrightarrow P(A|B) = $



---
