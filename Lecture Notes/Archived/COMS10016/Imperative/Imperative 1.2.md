---
Date & Time: 31-08-2026 12:02
Lecturer:
  - Tilo Burghardt
Course Name:
  - COMS10016
Lecture Name: |-
  Types, Variables
  & Scope
---
## Introduction
```C
#include <stdio.h>

// Calculate area of walls and ceiling.
int area(int length, int width, int height) {
return 2 * (width + length) * height + length * width;
}

// Print out the area of paint for my room.
int main(void) {
printf("The paint area is: %d\n", area(5, 3, 2));
return 0;
}
```
- Area is defined before the main function, so the compiler knows about the function before main calls it.
- Use camelCase
- ✅ Define variables during initalisation
- 

## Arithmetic Expressions
![[Screenshot 2026-08-31 at 12.10.23 PM.png]]

## Input
```C
int length;
scanf("%d", &length);
```
- %d: Set type as integer
- 

## Diagrams

---
#Tags