---
Date & Time: 09-10-2026 10:21
Lecturer:
  - Tilo Burghardt
Course Name:
Lecture Name:
---
## Recap
![[Screenshot 2026-08-31 at 6.51.58 PM.png]]

## Hex Representation
```C
unsigned char byte = 0x0E;
printf("%02x\n", byte);
```
- %..x: Hex
- 02, 04...: Byte

## Type Mixing
```C
unsigned char byte = 255;
signed char byte2 = (signed char)byte;
```
🚨 Avoid using casts to preserve accuracy and expected outcome
⚠️ Use -Wnarrowing or -Wconversion for compiler alerts
### Endian-ness
```C
unsigned short word = 0x00FF; 
unsigned char *bytes = &word;
printf("%hhu, %hhu\n", bytes[0], bytes[1]);
```
- Output byte-by-byte
- Endian-ness causes different output order (255, 0 or 0, 255)
### Integer Promotion
```C
signed char a = 64, b = 8, c = 2, result;
result = (a * b) / c; // promoted result 0x100 truncated to 0
printf("%hhi\n", result); // 0, since result did not fit char
```
- All variables will be promoted to integer in integer expressions

## Bitwise Operations
| Operators | Operation   |
| --------- | ----------- |
| `&`       | AND         |
| \|        | OR          |
| `~`       | NOT         |
| `^`       | XOR         |
| `>>`      | Right shift |
| `<<`      | Left shift  |



---
#Imperative