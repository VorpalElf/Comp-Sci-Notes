---
Date & Time: 19-10-2026 10:05
Lecturer:
  - Oliver Ray
Course Name:
  - COMS10016
Lecture Name: Dynamic Data
---
## Introduction
Stack: LIFO data structure. Where arguments, local variables and return addresses are allocated during function calls
Heap: Memory set aside for dynamic allocation. For data needs to be <mark style="background: #FFB86CA6;">persistent</mark>

## Malloc & Free
```C
#include <stdlib.h>

int main() {
	char *s = malloc(4);
	strcpy(s, "cat");
	printf("%s\n", s);
	free(s);
}
```
`malloc()`: Allocate memory and link to pointers. Represented with <mark style="background: #BBFABBA6;">bytes</mark>. Return with `void`
`free()`: Free memory of things linked to pointer
🚨🚨🚨 <mark style="background: #FF5582A6;">FREE</mark> all allocated memory to prevent <mark style="background: #FFB86CA6;">memory leak</mark> 🚨🚨🚨
⚠️ Always point pointers to allocated memory ⚠️
💡 Use `valgrind` to detect memory leaks

## Calloc
- Set all values in the allocated memory to 0, return to pointer
```C
int *numbers = calloc(10, sizeof(int));

calloc(size_t amount, size_t size);
```
`amount`: Amount of items
`size`: Size for each item, in Bytes

## Realloc
- Allocates new array, copies from old array, free the old array
```C
int capacity = 4;
char *s = malloc(capacity);
…
capacity = capacity * 3 / 2;
s = realloc(s, capacity);
…
free(s);
```
⚠️ <mark style="background: #FFB86CA6;">Update pointer</mark> during realloc



---
#Imperative