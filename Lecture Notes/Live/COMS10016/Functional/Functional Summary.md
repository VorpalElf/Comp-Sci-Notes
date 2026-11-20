## Pattern Matching
```Haskell
foo x = case x of
	1 -> "bish"
	2 -> "bash"
	3 -> "bosh"
	_ -> "bool"
	
egGuardSugar x
	| x < 0 = "negative"
	| x <= 9 = "single digit"
	| otherwise = "multi-digit"
```
---
## Recursion
1. Define the type
2. Enumerate cases
3. Define simple cases
4. Define other cases
5. Generalise & Simplify
---
## Types
- `f :: A -> B` $\equiv$ `e :: A` and `f e :: B`
- Tuples: Finite sequence of components with different types
- E.g. `(False, 'a', 1) :: (Bool, Char, Int)`
#### Function Types
- Function: Mapping from arguments of one type to results of another type
- `T1 -> T2` $\equiv$ Argument: T1, result: T2
```Haskell
add :: (Int, Int) -> Int
add (x,y) = x + y
```
#### Curried Functions
```Haskell
add' :: Int -> (Int -> Int)
add' x y = x + y
```haskell
- Returning functions as results (i.e. output of a function -> func it again)
1. Takes x as an input
2. Return add' x
3. Takes y as input
4. Return x + y
### Type Classes
- A set of types
1. `Eq`: Support equality testing
2. `Ord`: Types that supports ordering
3. `Show`: Can be represented as String
4. `Read`: Support String to Any
5. `Enum`: Sequentially ordered, can enumerate
6. `Bounded`: Have upper & lower bounds
7. `Num`: Numeric
	- `Integral`: Real & Integers
	- `Floating`: Floating points (e.g. `float` & `double`)



## Fold
```

---
## ADTs
```Haskell
type Pos = (Int, Int)

data Player = Rock | Paper | Scissors
```
- `type`: Make new type based on built-in types
- `data`: Make new type
#### Instances
```Haskell
instance Eq Player where
	Rock == Rock = True
	...

-- Quicker way
data Player = Rock | Paper | Scissors deriving (Eq)
```



---
## Folds
```Haskell

```