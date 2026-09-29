---
Date & Time: 29-09-2026 15:11
Lecturer:
  - Samantha Frohlich
Course Name:
  - COMS10016
Lecture Name:
---
## Environment & Scope
```Haskell
y = 5

expression = y + 2

scopeExample = ((\y -> y) 5) + ((\y -> y) 2)
```
- Same scope within brackets

## Branching
```Haskell
foo x = case x of
	1 -> "bish"
	2 -> "bash"
	3 -> "bosh"
```




---
