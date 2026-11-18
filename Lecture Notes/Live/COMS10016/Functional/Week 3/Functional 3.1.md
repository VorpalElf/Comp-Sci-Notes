---
Date & Time: 06-10-2026 15:10
Lecturer:
  - Samantha Frohlich
  - Jess Foster
Course Name:
  - COMS10016
Lecture Name: Lists
---
## Lists
```Haskell
egList :: [ Int ]
egList = []
```

## Operations
```haskell
head :: [Int] -> Int
head xs = case xs of
x : xs' -> x
```
⭐️ Prove by Induction
💡 Base case, then assume other cases

![[Pasted image 20261118100541.png]]

## Special Symbols
#### Constructors
```Haskell
(:) :: a -> [a] -> [a]
```
- Join an `Any` and an array of `Any` to a new array of `Any`
#### Such That
```Haskell
|
```
#### Drawn From
```Haskell
<-
```
#### Generator
```Haskell
x <- [1,2,3]
```





---
#Functional