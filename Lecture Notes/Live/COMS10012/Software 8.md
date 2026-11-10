---
Date & Time: 10-11-2026 11:12
Lecturer:
  - Matthew Edwards
Course Name:
  - COMS10012
Lecture Name: Debugging
---
## strace
- Intercepts and displays system calls made by the process
```Bash
strace [command]
```
- `-e`: Identify only specific system calls
- `-p`: Attach `strace` to already running process
## ltrace
```Bash
ltrace [command]
```
- Track libraries
## Valgrind
- Tools for dynamic analysis (i.e. understanding your process as it runs)
- `memcheck`: Check for memory leaks
- call using `valgrind --leak-check=yes [FILE]`
#### Types of Memory Loss
1. "definitely lost": Allocated memory, but lost the pointer
2. "indirectly lost": Allocated memory, but lost the pointer where I stored the pointer
3. "possibly lost": Probably lost my pointer
4. "still reachable": You've never freed your memory
5. "suppressed": You told valgrind shut up
#### Other usage
- `cachegrind`: Profile my code (i.e. which instructions executed most often)
- `callgrind`: Creates call graph between calls
- `hellgrind` & `drd`: Thread errors
- `massif`: Measure memory usage
## GDB
1. Run the program
2. Stop at specific points
3. Inspecting what has happened
4. Change values live
#### Breakpoints
- Add breakpoints
```Bash
(gdb) break [FunctionName / linenumber]
```
- See breakpoint options
```Bash
(gdb) info functions
All defined functions:

File valgrinddemo.c:
18:     int main(void);
3:      void tennumbers(void);
```
#### Inspection
```Bash
Breakpoint 1, tennumbers () at valgrinddemo.c:4
4	  int* x = malloc(10 * sizeof(int));
```
- `step`: Step the program until reaches a different source line
- `stepi`: Step one instruction exactly
- `next`: Step program, proceeding through subroutine calls
#### Change Values



---
