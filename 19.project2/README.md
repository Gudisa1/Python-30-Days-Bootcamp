
# 🎮 Rock-Paper-Scissors Challenge

## 📌 Overview

This project is a simple **command-line Rock-Paper-Scissors game** built in Python for two players. The game runs in rounds and determines a winner based on classic rules.

The first player to reach **2 points wins the game**, or the game ends after **3 rounds**.

---

## 🚀 Features

* Two-player interactive gameplay
* Input validation (accepts only `R`, `P`, `S`)
* Score tracking after each round
* Early win detection (first to 2 points)
* Final game summary

---

## 🧠 Game Rules

* **R** → Rock
* **P** → Paper
* **S** → Scissors

### Winning Logic:

* Rock beats Scissors
* Scissors beats Paper
* Paper beats Rock
* Same choices result in a **tie**

---

## 🛠️ How It Works

### 1. Player Input

Each player is prompted to enter their choice:

```
R (Rock), P (Paper), or S (Scissors)
```

Invalid inputs are rejected until a valid choice is entered.

---

### 2. Round Evaluation

The function `determine_winner()`:

* Compares both player inputs
* Returns:

  * `"player1"` → Player 1 wins
  * `"player2"` → Player 2 wins
  * `"tie"` → No winner

---

### 3. Score Tracking

* Scores are updated after each round
* Displayed immediately after each round

---

### 4. Game End Conditions

The game ends when:

* A player reaches **2 points**, OR
* **3 rounds** have been completed

---

### 5. Final Result

At the end, the program prints:

* Final scores
* Winner (or draw)

---

## ▶️ How to Run

1. Make sure you have Python installed
2. Save the script as `rps_game.py`
3. Run the program:

```bash
python rps_game.py
```

---

## 📂 Project Structure

```
rps_game.py   # Main game script
README.md     # Project documentation
```

---

## 🧪 Example Gameplay

```
Write R for Rock, P for Paper, S for Scissors Shoot Player 1: R
Write R for Rock, P for Paper, S for Scissors Shoot Player 2: S

Player 1 Score: 1
Player 2 Score: 0
```

---

## 💡 Possible Improvements

* Add single-player mode (vs computer)
* Add GUI using Tkinter or PyQt
* Track game history
* Add animations or sound effects
* Allow custom number of rounds


