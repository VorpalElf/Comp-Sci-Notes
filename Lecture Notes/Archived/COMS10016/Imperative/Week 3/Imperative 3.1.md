---
Date & Time: 10-09-2026 11:56
Lecturer:
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

## Strings
```C
char textA[3] = {72, 105, 0};

printf("%s\n", textA); // prints out “Hi”
```
- An array type of char

## strings.h
```C
#include <strings.h>
char text[] = "Hello";
int length = strlen(text);
printf("%d\n", length);  // prints "2"
```
🚨 Do not print strlen() directly, as strlen() is size_t, instead of integer

## Pointers
```C
char* words[] = {"Hello", "World", "c"};
printf("%s\n", words[0]);  // prints "Hello"
printf("%c\n", *words[0]); // prints "H"
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

## Identity & Compare
- Identity: <mark style="background: #FF5582A6;">memory address</mark> of the data
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

## Other Functions
#### Copy
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
- Please check for array storage to prevent overflow

#### Concatenate 
```C
char str1[] = "Hi\n";
char str2[] = "Lo\n";
char str3[strlen(str1) + strlen(str2) + 1];

strcpy(str3, str1);
strcat(str3, str2);
printf("%s", str3);  // prints "Hi" and "Lo"
```


---
