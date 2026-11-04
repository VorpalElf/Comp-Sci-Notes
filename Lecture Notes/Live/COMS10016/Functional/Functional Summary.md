
## Types
- `f :: A -> B` $\equiv$ `e :: A` and `f e :: B`
- Tuples: Finite sequence of components with different types
- E.g. `(False, 'a', 1) :: (Bool, Char, Int)`
### Function Types
- Function: Mapping from arguments of one type to results of another type
- `T1 -> T2` $\equiv$ Argument: T1, result: T2
```Haskell
add :: (Int, Int) -> Int
add (x,y) = x + y
```
### Curried Functions
```Haskell
add' :: Int -> (Int -> Int)
add' x y = x + y
```
- Returning functions as results (i.e. output of a function -> func it again)
1. Takes x as an input
2. Return add' x
3. Takes y as input
4. Return x + y

## Fold
```

## Folds
```Haskell

```