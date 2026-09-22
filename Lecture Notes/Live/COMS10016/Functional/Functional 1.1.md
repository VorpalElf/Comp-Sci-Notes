---
Date & Time: 22-09-2026 15:03
Lecturer:
  - Jess Foster
  - Samantha Frohlich
Course Name:
  - COMS10016
Lecture Name: Expressions & Evaluations
---
## Functional 

## Basic Syntax
### Running
```bash
ghci filename
```
### Comments
```Haskell
--- This is a comment

{-
Also a comment
-}
```
### Arithmetics
```ghci
ghci> 1+1
2

ghci> (4+2) * (8-2)
36
```
## Variables
- `=` means equal, instead of assign + other operations
- Cannot redefine/reassign variables
```ghci
ghci> x = 1
ghci> x = 2
ghci> x
2
```

## Functions
```ghci
ghci> (\y -> y) 5
5

ghci> (\y -> y + 2) 5
7
```
- Every lambda takes one input
- Arguments: Things after space

---
