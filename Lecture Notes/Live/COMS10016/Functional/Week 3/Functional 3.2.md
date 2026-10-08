---
Date & Time: 08-10-2026 15:15
Lecturer:
  - Samantha Frohlich
  - Jess Foster
Course Name:
  - COMS10016
Lecture Name: ADTs
---
## Introduction
```Haskell
data Player = White | Black
```

## Sums
```Haskell
data Player = White | Black
white :: Player
white = White
black :: Player
black = Black

eqPlayer :: Player -> Player -> Bool
eqPlayer White White = True
eqPlayer Black Black = True
eqPlayer _ _ = False
```

## Products
```haskell
data Piece' = Piece' Player PieceType

whiteQueen :: Piece
whiteQueen = MkPiece White Queen

whiteQueen' :: Piece'
whiteQueen' = Piece' White Queen

promoteToQueen :: Piece -> Piece
promoteToQueen (MkPiece c Pawn) = MkPiece c Queen
promoteToQueen (MkPiece c p) = MkPiece c p
```
- `MkPiece`: Product function (i.e. binds them together)

## Record Syntax
```Haskell
data PieceR = MkPieceR { player :: Player, pieceType :: PieceType }
```



---
#Incomplete