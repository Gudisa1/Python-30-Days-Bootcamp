
# ⏳ Countdown Timer with Reminder

## 📌 Overview

This project is a simple **command-line countdown timer** built in Python. It allows users to set a timer (in seconds) and attach a custom reminder message that displays when the time is up.

---

## 🚀 Features

* User-defined countdown duration (in seconds)
* Real-time timer display (MM:SS format)
* Custom reminder message
* Input validation for numeric values
* Simple and lightweight CLI tool

---

## 🧠 How It Works

### 1. User Input

The program asks the user to:

* Enter the countdown time (in seconds)
* Enter a reminder note

Example:

```id="h2k8sm"
Enter countdown time in seconds: 10
Enter a reminder note: Drink water
```

---

### 2. Countdown Logic

The `countdown()` function:

* Converts seconds into minutes and seconds using `divmod`
* Updates the timer display every second
* Uses `time.sleep(1)` to pause execution

---

### 3. Live Timer Display

The timer updates in place using:

```id="k39d1a"
print(timer, end='\r')
```

This creates a smooth countdown effect in the terminal.

---

### 4. Completion Alert

When the timer reaches zero:

* A message is displayed:

```id="a8d0z1"
⏰ Time's up! Reminder: <your note>
```

---

### 5. Error Handling

* If the user enters a non-numeric value, the program:

  * Catches a `ValueError`
  * Prompts the user with an error message

---

## ▶️ How to Run

1. Ensure Python is installed
2. Save the script as `countdown_timer.py`
3. Run the program:

```bash id="q1n8vb"
python countdown_timer.py
```

---

## 📂 Project Structure

```id="t9m2kq"
countdown_timer.py   # Main script
README.md            # Documentation
```

---

## 🧪 Example Output

```id="p7x3dl"
Enter countdown time in seconds: 5
Enter a reminder note: Stand up

00:05
00:04
00:03
00:02
00:01

⏰ Time's up! Reminder: Stand up
```

---

## 💡 Possible Improvements

* Add sound alert 🔊 when time is up
* Support minutes/hours input format
* Pause and resume functionality
* Multiple timers at once
* GUI version using Tkinter or PyQt
* Desktop notifications

---

## ⚠️ Limitations

* Runs only in terminal/command prompt
* Timer accuracy depends on system timing and execution delays


