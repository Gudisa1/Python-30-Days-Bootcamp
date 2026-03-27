

# 🔐 Password Generator

## 📌 Overview

This project is a **secure password generator** built in Python. It allows users to create strong, customizable passwords based on selected criteria such as length and character types.

The program uses Python’s **`secrets` module**, ensuring cryptographically strong random password generation.

---

## 🚀 Features

* Custom password length
* Option to include:

  * Uppercase letters (A–Z)
  * Lowercase letters (a–z)
  * Numbers (0–9)
  * Symbols (!, @, #, etc.)
* Input validation for secure and correct usage
* Recursive handling if no character type is selected
* Secure randomness using `secrets.choice()`

---

## 🧠 How It Works

### 1. User Input

The program prompts the user to:

* Enter a **password length**
* Choose which character types to include:

  * Uppercase
  * Lowercase
  * Numbers
  * Symbols

Example:

```id="zz9e8m"
Password Length: 12
Include uppercase letters? (y/n): y
Include lowercase letters? (y/n): y
Include numbers? (y/n): y
Include symbols? (y/n): n
```

---

### 2. Character Pool Creation

Based on user selections, a pool of characters is built using:

* `string.ascii_uppercase`
* `string.ascii_lowercase`
* `string.digits`
* Custom symbol set

---

### 3. Password Generation

The function `generate_password()`:

* Randomly selects characters from the pool
* Uses `secrets.choice()` for better security
* Builds a password of the desired length

---

### 4. Validation

* Ensures password length is a **positive integer**
* Ensures **at least one character type** is selected
* If not, the user is prompted again

---

## ▶️ How to Run

1. Ensure Python is installed
2. Save the script as `password_generator.py`
3. Run the program:

```bash id="6d8h2x"
python password_generator.py
```

---

## 📂 Project Structure

```id="8l2kqz"
password_generator.py   # Main script
README.md               # Documentation
```

---

## 🧪 Example Output

```id="9o2x7c"
--- Password Generator ---

Password Length: 10
Include uppercase letters? (y/n): y
Include lowercase letters? (y/n): y
Include numbers? (y/n): y
Include symbols? (y/n): y

New Password:  A9f#k2P!xQ
```

---

## 🔒 Why Use `secrets` Instead of `random`?

* The `secrets` module is designed for **security-sensitive applications**
* It generates **cryptographically strong random numbers**
* Ideal for passwords, tokens, and authentication

---

## 💡 Possible Improvements

* Add option to avoid ambiguous characters (e.g., `O` vs `0`)
* Ensure at least one character from each selected type appears
* Save generated passwords to a file
* Add GUI (Tkinter, PyQt)
* Allow batch password generation
* Add password strength indicator


