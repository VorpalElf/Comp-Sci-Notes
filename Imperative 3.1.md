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