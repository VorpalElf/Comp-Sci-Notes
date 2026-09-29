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
	_ -> "bool"
```
- foo: variable name
- x: arguments
- _ : Default/else

```Haskell
fooSugar 1 = "bish"
fooSugar 2 = "bash"
fooSugar 3 = "bool"
```

```Haskell
-- If
egIfSugar x = if x > 10
then "Bigger than 10"
else "10 or less"
```
``
```Haskell
-- Guard
egGuardSugar x
	| x < 0 = "negative"
	| x <= 9 = "single digit"
	| otherwise = "multi-digit"
```

## Let & Where
```Haskell
letEg x =
	let xCubed = x * x * x
		result = xCubed + xSquared
		xSquared = x * x
	in result

  

whereEg x = result
	where
		result = xCubed + xSquared
		xCubed = x * x * x
		xSquared = x * x
```




---
