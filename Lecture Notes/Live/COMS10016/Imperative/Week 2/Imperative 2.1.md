---
Date & Time: 28-09-2026 10:28
Lecturer:
  - Tilo Burghardt
  - Otto Brookes
Course Name:
  - COMS10016
Lecture Name: Decision & Recursion
---
## Procedure Declarations
```C
int grade(int mark);  // Declaration of Signature only

int main(void){
	grade(mark);
}

int grade(int mark) { } // Full definition
```
- Allow use of functions before definition
- Prevents circular dependencies

## Switch Statement
```C
int nextHailstone(int x) {
	int next;
	switch (x % 2) {
		case 1:
			next = 3 * x + 1; break;
			default: next = x/2;
	}
	return next;
}
```
- Allows executing different statement
- ⚠️ Remember to add <mark style="background: #FF5582A6;">break</mark>



---
#Imperative