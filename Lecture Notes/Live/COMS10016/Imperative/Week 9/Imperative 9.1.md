---
Date & Time: 16-11-2026 10:38
Lecturer:
  - Oliver Ray
Course Name:
  - COMS10016
Lecture Name: Modules
---
## Introduction
```C
int add(int a, int b);
```

```C
#include "add.h"
int main() {
	add(a, b);
}
```
- Bundle functions into a module, available to other modules

## Local
```C
static void swap();
extern void hi();
```
- `static`: Function within the module
- `extern`: By default; linkable with other modules
![[Screenshot 2026-11-20 at 10.36.53 AM.png]]
```C
int f() {
	static int a = 1;
	auto int b = 2;
}
```
- `static`: Stay in scope and DATA even f() finished
- `auto`: By default; vanish after scope cleared


---
