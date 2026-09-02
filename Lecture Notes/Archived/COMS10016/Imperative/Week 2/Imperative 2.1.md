---
Date & Time: 01-09-2026 15:57
Lecturer:
  - Tilo Burghardt
Course Name:
  - COMS10016
Lecture Name: Literals, Enums & Constraints
---
## 4 Laws of Programs
1. Programs must <mark style="background: #FFF3A3A6;">work correctly</mark>
2. Programs must be <mark style="background: #BBFABBA6;">readable</mark>
3. Programs must be <mark style="background: #FF5582A6;">compact</mark>
4. Programs must be efficient

## Constants & Enums
```C
const int FIRST_BOUNDARY = 70;
```
- Define constants in CAPITALS for better readability
- Use constants to improve readability

```C
enum { MON, TUE, WED, THY, FRI, SAT, SUN};

const int MON = 0, TUE = 1, ..., SUN = 6;
```
- Assign identifiers to non-changing items (indexed as integers)
- Integers only (e.g. MON will return 0)

```C
enum { MON, TUE, WED, THY, FRI, SAT, SUN};

void dayRoutine(int day) {
	switch(day) {
		case MON: ;
		break;
	}
}
```

## Conversion
```C
#include <stdio.h>
float x = 5.0001;
printf("Number:%7f\n", x);
```

## Ternary Operator
```C
int max = a > b ? a : b;

// Identical to
int max;
if (a>b) {
	max = a;
} else {
	max = b;
}
```



---
#Imperative