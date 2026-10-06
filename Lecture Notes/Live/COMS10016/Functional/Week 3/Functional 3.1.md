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


---
#Functional