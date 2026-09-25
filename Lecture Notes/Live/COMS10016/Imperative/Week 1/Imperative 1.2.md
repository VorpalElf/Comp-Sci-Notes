---
Date & Time: 21-09-2026 15:33
Lecturer:
  - Tilo Burghardt
Course Name:
  - COMS10016
Lecture Name: Types, Variables & Scopes
---
## Arithmetic Expressions
![[Screenshot 2026-08-31 at 12.10.23 PM.png|621]]

## Input & Types
```C
int length;
scanf("%d", &length);
```
- %d: Set type as integer
- &: Allocate data to address of variable length

![[Screenshot 2026-08-31 at 6.51.58 PM.png]]
- Type matters due to different sizes (i.e. memory allocation)
- 
## Memory

```C
int main(void) {
	signed char a = 100;
	printf("A is %d\n", a);
	printf("The address of a is: %p\n", &a);
}
```
- %p: Pointer address

---
#Imperative