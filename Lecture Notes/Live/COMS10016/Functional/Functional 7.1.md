---
Date & Time: 18-11-2026 10:29
Lecturer:
  - Samantha Frohlich
Course Name:
  - COMS10016
Lecture Name: Folding
---
## Introduction
- Encapsulates pattern of recursion
```Haskell
syn :: Num a => [a] -> a
sum = foldr (+) 0
-- i.e.
sum = foldr 
```

### Foldr
- Fold right
```Haskell
foldr :: Foldable t => (a -> b -> b) -> b -> t a -> b
```


---
