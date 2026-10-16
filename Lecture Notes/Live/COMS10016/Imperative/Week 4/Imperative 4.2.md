---
Date & Time: 16-10-2026 10:03
Lecturer:
  - Oliver Ray
Course Name:
  - COMS10016
Lecture Name: Structures & User Types
---
## Introduction
```C
struct item{
	int x, y;
}
```
- Group similar things together into one data type
- Use `struct` to make new data type
- Structs are <mark style="background: #FFB86CA6;">pass-by-value</mark>

```C
int main() {
	struct item = {137, 91};
	i.x++;
}
```
- Use `{}` to initialise data type
- Use `.` to access elements inside the struct




---
#Imperative