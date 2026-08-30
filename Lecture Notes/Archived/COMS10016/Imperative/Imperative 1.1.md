---
Date & Time: 30-08-2026 12:12
Lecturer:
  - Tilo Burghardt
  - Oliver Ray
  - Jess Foster
  - Samantha Frohlich
Course Name:
  - COMS10016
Lecture Name: Welcome
---
## Introduction
- C is an imperative and procedural language
- Imperative: Telling how the computer to do things, using <mark style="background: #FFF3A3A6;">statements</mark>
- Procedural: Sequences constructed in small, <mark style="background: #BBFABBA6;">reusable</mark> chunks	

## Compiler

```Bash
$ clang -std=c11 -Wall minimal.c -o minimal
$ ./minimal
```
- clang: Runs clang compiler
- -std=...: Language standard to use
- -Wall: Turn on all standard warnings
- -o: Customise output filename

## Library Modules
```C
#include <stdio.h>
```
- stdio.h is a <mark style="background: #FF5582A6;">header</mark> file
- stdio: standard input/output

## Output
```C
#include <stdio.h>

int main(void) {
	// Print
	printf("Hello World\n");
	return 0;
}
```

## Diagrams
![[Pasted image 20260830213508.png|400]]
Diagram of types of Programming Languages

![[Screenshot 2026-08-30 at 11.37.42 PM.png]]
Basic Elements of a Function

---
#Imperative