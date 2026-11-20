---
Date & Time: 05-10-2026 10:07
Lecturer:
  - Otto Brookes
  - Tilo Burghardt
Course Name:
  - COMS10016
Lecture Name: Strings
---
## Introduction
```C
char c = 65;

printf("%hhi\n", c); // prints out the number “65”
```

```C
#include <ctype.h>
char up = 'g' - ('a' - 'A');
char up = toupper(g);
```

![[Screenshot 2026-10-05 at 10.09.20 AM.png]]
### Null Character
- Byte with every bit off -> (All 0s)
- Mark the end of a string
## Strings
```C
char textA[3] = {72, 105, 0};

printf("%s\n", textA); // prints out “Hi”
```
- An array type of char

## Pointers
```C
char* words[] = {"Hello", "World", "c"};
printf("%s\n", words[0]);  // prints "Hello"
printf("%c\n", *words[0]); // prints "H"
```
- A variable that stores the memory address of another variable
- Like the 

## strings.h
```C
#include <strings.h>
char text[] = "Hello";
int length = strlen(text);
printf("%d\n", length);  // prints "2"
```
🚨 Do not print strlen() directly, as strlen() is size_t, instead of integer

![[Screenshot 2026-10-05 at 10.25.36 AM.png]]

## Other Functions
### Identity & Compare
- Identity: same <mark style="background: #FF5582A6;">memory address</mark> of the data
- Check identity with == operator
```C
void checkIdentity(char str1[], char str2[]) {
	if (str1 == str2) {
		printf("Strings are identical.");
	} else {
		printf("Strings are not identical.");
	}
}

void main() {
	char str1[] = "Hi";
	char str2[] = "Hi";
	checkIdentity(str1, str2); // Not identical
	checkIdentity(str1, str1); // Identical
}
```

- Use strcmp to compare <mark style="background: #FFB86CA6;">contents</mark>
```C
void main() {
	char str1[] = "Hi";
	char str2[] = "Hi";
	int cmp = strcmp(str1, str2); 
	// cmp > 0, later; cmp = 0, same; cmp < 0, earlier
}
```
### Copy
```C
#include <string.h>
#include <stdio.h> ...

int main() {
char str1[] = "Hi";
char str2[3];
strcpy(str2, str1);
printf("%s\n", str2); // prints “Hi”
return 0;
}
```
⚠️ Check for array storage to prevent overflow
### Concatenate 
![[Screenshot 2026-10-05 at 10.41.06 AM.png]]
```C
char str1[] = "sun\n";
char str2[] = "set\n";
char str3[strlen(str1) + strlen(str2) + 1];

strcpy(str3, str1);
strcat(str3, str2);
printf("%s", str3);  // prints "Sunset"
```
- Copy "sun" into str3 $\rightarrow$ Join "sun" and "set"
### Printing Strings into Strings
```C
int main(void) {
	char str[10];
	sprintf(str, "Room %d", 42);
	printf("%s\n", str);
	return 0;
}
```

## Command Line Arguments
```C
#include <stdio.h>

int main(int argc, char* argv[])
{
    if (argc == 2)
    {
        printf("hello, %s\n", argv[1]);
    }
    else
    {
        printf("hello, world\n");
    }
}
```
- argc: Argument count => no. of arguments
- argv: Argument vector => Arguments itself

Output:
```bash
./greet David
hello, David
```
🚨 Remember to check argc before execute
🚨 Argv is an array of strings

---
#Imperative