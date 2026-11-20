---
Date & Time: 20-11-2026 10:41
Lecturer:
  - Oliver Ray
Course Name:
  - COMS10016
Lecture Name: Preprocessor
---
## Introduction
- Program run before the compiler
- Directives: `#`, symbols `__`

## Macros
- Replaceable identifier
- `#define IDENTIFIER REPLACEMENT`
```C
#define PI 3.14159  // No arguments
#define DISC(radius) ((PI) * (radius) * (radius))
```
⭐️ Use parentheses
- `\`: Continues the statement in next line
- `#undef`: Undefine the macro



---
