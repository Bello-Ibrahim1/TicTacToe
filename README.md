# TicTacToe
This is a TicTacToe Game that uses the implementation of ideas from discrete structures.
The Logic of Discrete Structures is implemented to determine which player wins, loses, or draws. 

## Overview
This game is played on a 3x3 grid or board. Players 1 and 2( Computer) mark the board with either an 'X' or 'O'. Three of either mark in a row, vertically, horizontally, or diagonally, will indicate a win.


---

## Rules of the Game

1. Player 1 uses "X" and Player 2 uses "O".
2. The game board is a 3x3 grid, with positions indexed from 0 to 2 rows and columns.
3. A player wins if they get three marks in a row, horizontally, vertically, or diagonally.
4. The game is a draw if all positions are filled.

---

## Winning Scenarios

### Horizontal Winning Possibilities

- **Row 0**: (0,0), (0,1), (0,2)
- **Row 0**: (1,0), (1,1), (1,2)
- **Row 0**: (2,0), (2,1), (2,2)

### Vertical Winning Possibilities

- **Column 0**: (0, 0), (1, 0), (2, 0)
- **Column 1**: (0, 1), (1, 1), (2, 1)
- **Column 2**: (0, 2), (1, 2), (2, 2)

### Diagonal Winning Possibilities

- **Diagonal 1**: (0, 0), (1, 1), (2, 2)
- **Diagonal 2**: (0, 2), (1, 1), (2, 0)

---

## Draw Scenario

The game ends in a draw if the board is filled without a winner. It is considered a draw if all cells are occupied and no player has won.

---

## Propositional Logic Used

- **p**: Player 1 (X) gets three marks in a row.
- **q**: Player 1 wins.
- **r**: Player 2 (O) gets three marks.
- **s**: Player 2 wins.

### Winning Logic (Propositional Form):
- **If p, then q**: If Player 1 gets three marks in a row, Player 1 wins.
- **If r, then s**: If Player 2 gets three marks in a row, Player 2 wins.

### Draw Logic:
- **If not p and not r**, then it is a draw: If neither player gets three marks in a row, the game results in a draw.

---

### Modus Ponens Application

The logic applied in the Tic Tac Toe game can be described using the **Modus Ponens** inference rule. Modus Ponens is a fundamental rule of inference that can be summarized as follows:

- **If p → q** (If p, then q) and **p** is true, then **q** must also be true.

This is directly applied to the game logic:

- **If Player 1 gets three marks in a row (p), then Player 1 wins (q)**. When Player 1 achieves three marks in a row, the system applies Modus Ponens to conclude that Player 1 has won.
- **If Player 2 gets three marks in a row (r), then Player 2 wins (s)**. Similarly, when Player 2 achieves three marks in a row, the system applies Modus Ponens to conclude that Player 2 has won.

Thus, after each move, the system checks if the condition (p or r) holds, and if so, the corresponding conclusion (q or s) is drawn.

---

## Example Gameboards

### Example 1: Player 1 Wins Horizontally

| Row/Col | 0 | 1 | 2 |
|---------|---|---|---|
| **0**   | X | X | X |
| **1**   |   | O |   |
| **2**   | O |   |   |

**Result**: Player 1 wins with three "X"s in the top row.

---

### Example 2: Player 2 Wins Vertically

| Row/Col | 0 | 1 | 2 |
|---------|---|---|---|
| **0**   | X |   |   |
| **1**   | X | O |   |
| **2**   | X |   |   |

**Result**: Player 2 wins with three "O"s in the middle column.

---

### Example 3: Draw Scenario

| Row/Col | 0 | 1 | 2 |
|---------|---|---|---|
| **0**   | X | O | X |
| **1**   | O | X | O |
| **2**   | O | X | O |

**Result**: The game is a draw. No player has three marks in a row, and the board is full.





