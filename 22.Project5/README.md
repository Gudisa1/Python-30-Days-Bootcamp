# 🎮 Hangman Game (ASCII Art Edition)

## 📌 Overview

This project is a **command-line Hangman game** built in Python, featuring visual **ASCII art** that updates as the player loses lives.

The player must guess the hidden word one letter at a time before running out of lives.

---

## 🚀 Features

* Interactive CLI gameplay
* ASCII art that visually represents player progress
* Random word selection
* Input validation (only single alphabet letters allowed)
* Tracks guessed letters
* Win/Loss detection with final result display

---

## 🧠 Game Rules

* You have **6 lives** ❤️
* Guess one letter at a time
* Each incorrect guess reduces your lives
* The hangman drawing progresses with each mistake
* You win if you guess the word before lives run out

---

## 🎨 ASCII Art Preview

Each wrong guess updates the hangman:

```
 ----- 
 |   |
 O   |
/|\  |
/ \  |
     |
=========
```

⬇️ gradually disappears as lives decrease...

---

## 🛠️ How It Works

### 1. Word Selection

* A random word is selected from a predefined list:

```id="w1"
["python", "hangman", "developer", "challenge", "keyboard"]
```

---

### 2. Game State Tracking

* `word_display` → shows guessed letters and blanks (`_`)
* `guessed_letters` → stores previous guesses
* `lives` → starts at 6

---

### 3. Player Input

* Only accepts:

  * Single alphabet letters
* Rejects:

  * Numbers, symbols, multiple characters
  * Already guessed letters

---

### 4. Game Loop

Each round:

1. Display current hangman stage
2. Show word progress (`_ _ a _ _`)
3. Prompt user for a guess
4. Update:

   * Correct guess → reveal letters
   * Wrong guess → lose a life

---

### 5. Game End

* ✅ **Win** → all letters guessed
* 💀 **Lose** → lives reach 0

Final result displays the correct word.

---

## ▶️ How to Run

1. Ensure Python is installed
2. Save the script as `hangman.py`
3. Run the program:

```bash id="run1"
python hangman.py
```

---

## 📂 Project Structure

```id="struct1"
hangman.py   # Main game file
README.md    # Documentation
```

---

## 🧪 Example Gameplay

```id="ex1"
🎮 Welcome to Hangman with ASCII Art!

Word: _ _ _ _ _ _
Guessed Letters:
Lives Left: 6

Guess a letter: a
❌ Wrong guess!

Lives Left: 5
```

---

## 💡 Possible Improvements

* Add categories (animals, countries, tech, etc.)
* Load words from a file or API
* Add difficulty levels
* Implement hints system
* Track high scores
* Add multiplayer mode
* Build GUI version (Tkinter / PyQt)
* Add sound effects 🔊

---

## ⚠️ Limitations

* Limited word list
* Runs only in terminal
* No persistence (scores reset each run)


