# The game

Peg solitaire is a classic board game for one player. You can find more information in [Wikipedia](https://en.wikipedia.org/wiki/Peg_solitaire). This code implements a european board.

Any peg can jump over an adjacent peg into an empty cell. After that the jumped peg is being removed. The main goal is to left only one peg on the board. You lose if you can't make a move and there are two or more pegs on the board.

# Interface

Every turn the game will ask you for two inputs. You should input the coordinates of the peg you want to move and the coordinates of the destination cell. Coordinate pair is a two-digit number: the first digit represents a row, the second one represents a column.

For example:
```
  1234567
1   ***
2  *****
3 ***.***
4 *******
5 *X*****
6  *****
7   ***
```
X-cell has coordinates 52: row 5 and column 2.

As you can see, firstly you have only one empty cell (34). So, the only four possible moves at the very beginning are:
```
32
34
```

```
14
34
```

```
36
34
```

```
54
34
```

# Implementation

Yes, I implemented the whole game only with `dc` capabilities, because I can, damn it!

I think I commented the code pretty fine, so if you are familiar with a basic `dc` syntax, you'll figure out what's going on easily (well, as easily as `dc` syntax permits, lol).

# How to run

```
dc -f game.dc
```
