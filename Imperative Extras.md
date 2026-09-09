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