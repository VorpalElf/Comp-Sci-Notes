---
Date & Time: 17-09-2026 11:13
Lecturer:
  - Tilo Burghardt
Course Name:
  - COMS10016
Lecture Name: Bits
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

```C
unsigned short word = 0x00FF; 
unsigned char *bytes = &word;
printf("%hhu, %hhu\n", bytes[0], bytes[1]);
```
- Output byte-by-byte
- Endian-ness causes different output order (255, 0 or 0, 255)

## Integer Promotion





---
#Imperative #Incomplete