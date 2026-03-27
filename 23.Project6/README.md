
# 🎮 Tic-Tac-Toe (Player vs Computer)

## 📌 Overview

This project is a **command-line Tic-Tac-Toe game** built in Python where a player competes against a computer opponent.

The player uses **X**, and the computer uses **O**. The game continues until there is a winner or a draw.

---

## 🚀 Features

* Player vs Computer gameplay
* Dynamic 3x3 board
* Input validation for user moves
* Randomized computer moves
* Win and draw detection
* Clean and simple CLI interface

---

## 🧠 Game Rules

* The board is a **3×3 grid**
* Player = **X**
* Computer = **O**
* Players take turns placing their symbol
* First to align **3 symbols** wins:

  * Horizontally
  * Vertically
  * Diagonally
* If all spaces are filled → **Draw**

---

## 🛠️ How It Works

### 1. Board Creation

* A 3×3 grid is created using a list of lists:

```id="b1"
[[' ', ' ', ' '],
 [' ', ' ', ' '],
 [' ', ' ', ' ']]
```

---

### 2. Display Board

* The board is printed with row/column indices:

```id="b2"
  0   1   2
0 X | O |  
  ---------
1   | X |  
  ---------
2   |   | O
```

---

### 3. Player Move

* User inputs:

  * Row (0–2)
  * Column (0–2)
* Validates:

  * Input is numeric
  * Within range
  * Spot is not already taken

---

### 4. Computer Move

* Randomly selects from available empty cells using:

```id="b3"
random.choice(empty)
```

---

### 5. Win Detection

The function `is_winner()` checks:

* Rows
* Columns
* Diagonals

---

### 6. Draw Detection

* If all cells are filled and no winner → draw

---

## ▶️ How to Run

1. Make sure Python is installed
2. Save the script as `tic_tac_toe.py`
3. Run the program:

```bash id="run_ttt"
python tic_tac_toe.py
```

---

## 📂 Project Structure

```id="struct_ttt"
tic_tac_toe.py   # Main game file
README.md        # Documentation
```

---

## 🧪 Example Gameplay

```id="ex_ttt"
🎮 Welcome to Tic-Tac-Toe!

  0   1   2
0   |   |  
  ---------
1   |   |  
  ---------
2   |   |  

Your Turn (X)
Choose row (0-2): 1
Choose column (0-2): 1
```

---

## 🤖 Computer Logic

* Currently uses **random moves**
* Does not implement strategy or AI

---

## 💡 Possible Improvements

* Add **AI (Minimax algorithm)** 🤖
* Add difficulty levels (easy, medium, hard)
* Multiplayer mode (2 players)
* GUI version (Tkinter / PyQt)
* Highlight winning combination
* Add score tracking system
* Improve UI with colors

---

## ⚠️ Limitations

* Computer is not intelligent (random moves only)
* CLI-only (no graphical interface)
* No persistent scores


