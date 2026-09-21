---
Date & Time: 21-09-2026 10:05
Lecturer:
  - Tilo Burghardt
Course Name:
  - COMS10016
Lecture Name: Introduction
---
## Introduction
![[Pasted image 20260830213508.png | 400]]

## Background
- C is an imperative and procedural language
- Imperative: Telling how the computer to do things, using <mark style="background: #FFF3A3A6;">statements</mark>
- Procedural: Sequences constructed in <mark style="background: #FFB86CA6;">small</mark>, <mark style="background: #BBFABBA6;">reusable</mark> chunks	


![[Screenshot 2026-08-30 at 11.37.42 PM.png]]
- Must contain exactly one ```main``` function (```main``` is the )

## Running
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
- <> means "look in the standard place" (i.e. /usr/include/stdio.h)

## Output
```C
#include <stdio.h>

int main(void) {
	// Print
	printf("Hello World\n");
	return 0;
}
```





---
#Imperative