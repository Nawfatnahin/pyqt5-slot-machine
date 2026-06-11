# 🎰 PyQt5 Slot Machine

> A beginner-friendly desktop slot machine game built with Python and PyQt5.

[![Python](https://img.shields.io/badge/Python-3.7%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![PyQt5](https://img.shields.io/badge/PyQt5-5.x-green?logo=qt&logoColor=white)](https://pypi.org/project/PyQt5/)
[![Status](https://img.shields.io/badge/Status-Complete-brightgreen)]()

---

## 📖 What Is This?

This is a simple, interactive **slot machine game** that runs as a desktop window on your computer. You start with **$100 in virtual money**, place a bet, spin the reels, and try to match three symbols to win!

It's a great project for anyone learning:
- **Python** fundamentals (functions, conditionals, loops)
- **Object-Oriented Programming** (classes and methods)
- **PyQt5** — a library for building graphical (GUI) desktop apps

---

## ✨ Features

| Feature | Description |
|---|---|
| 💰 **Starting Balance** | Every session begins with $100 |
| 🎲 **Random Spin** | 3 reels spin independently using Python's `random` module |
| 🏆 **Win Detection** | Checks if all 3 reels match for a payout |
| 🔢 **Input Validation** | Rejects non-numeric bets, zero bets, and bets larger than your balance |
| 📊 **Live Balance** | Your balance updates after every spin |
| 🎨 **Styled UI** | Custom fonts, colors, and layout using Qt StyleSheets |

---

## 🍉 Symbols & Payouts

The game has three symbols. To win, all **3 reels must show the same symbol**:

| Symbol | Name | Payout (if all 3 match) |
|--------|------|------------------------|
| 🍉 | Watermelon | **5× your bet** |
| ⭐ | Star | **3× your bet** |
| 🍒 | Cherry | **2× your bet** |

**Example:** You bet $10 and land `⭐ ⭐ ⭐` → You win $30 (3 × $10).

If they don't all match, you lose your bet.

---

## 🛠️ Prerequisites

Before running this project, make sure you have:

1. **Python 3.7 or higher** — [Download here](https://www.python.org/downloads/)
2. **PyQt5** — the GUI library used to build the window

> 💡 **Don't have Python?** Visit [python.org/downloads](https://www.python.org/downloads/) and install the latest version. During installation, check the box that says **"Add Python to PATH"**.

---

## 📦 Installation

### Step 1 — Clone or download the project

**Option A: Clone with Git**
```bash
git clone https://github.com/Nawfatnahin/pyqt5-slot-machine.git
cd pyqt5-slot-machine
```

**Option B: Download as ZIP**
1. Click the green **"Code"** button on this page
2. Select **"Download ZIP"**
3. Extract the ZIP file to any folder on your computer

---

### Step 2 — Install PyQt5

Open your **terminal** (Command Prompt on Windows, Terminal on Mac/Linux) and run:

```bash
pip install PyQt5
```

> ✅ You should see something like `Successfully installed PyQt5-5.x.x`. If you see an error, try `pip3 install PyQt5` instead.

---

## ▶️ How to Run

Navigate to the project folder in your terminal, then run:

```bash
python SlotMachineUsingPyQt5.py
```

A game window should pop up on your screen immediately. 🎉

> **Windows users:** If double-clicking the `.py` file doesn't work, open Command Prompt, `cd` to the project folder, and use the command above.

---

## 🎮 How to Play

1. **Look at your balance** — you start with $100.
2. **Type a bet amount** in the text box (must be a whole number greater than 0).
3. **Click "Enter Your Bet"** to spin the reels.
4. **Check the result** — the three symbols appear in the middle of the screen.
5. **Win or lose** — your balance updates automatically.
6. Keep playing until you run out of money or decide to quit!

---

## 🗂️ Project Structure

```
pyqt5-slot-machine/
│
├── SlotMachineUsingPyQt5.py   # 🎯 The entire game — all logic and UI in one file
└── README.md                  # 📄 This file
```

The entire game lives in a **single Python file** with one class called `SlotMachine`. Here's what each method does:

| Method | What it does |
|--------|-------------|
| `__init__` | Sets up all UI elements and the starting balance |
| `initUI` | Arranges the widgets in a vertical layout and applies styling |
| `game_play` | Runs when you click the button — validates bet, spins, shows result |
| `spin_row` | Randomly picks 3 symbols from the symbol list |
| `get_payout` | Checks if you won and calculates the prize amount |

---

## 🧠 What You'll Learn from This Code

If you're studying this project, here are the key Python/PyQt5 concepts used:

- **`class` and `__init__`** — Object-Oriented Programming basics
- **`random.choice()`** — picking random items from a list
- **`try / except`** — handling errors gracefully (e.g., non-numeric input)
- **`QWidget`, `QLabel`, `QPushButton`, `QLineEdit`** — common PyQt5 UI elements
- **`QVBoxLayout`** — stacking widgets vertically
- **`setStyleSheet()`** — styling a Qt app with CSS-like rules
- **Signal & Slot pattern** — `button.clicked.connect(function)` — the PyQt5 way to handle button clicks

---

## 🐛 Troubleshooting

| Problem | Solution |
|---------|----------|
| `ModuleNotFoundError: No module named 'PyQt5'` | Run `pip install PyQt5` in your terminal |
| `python: command not found` | Try `python3` instead of `python`, or reinstall Python with PATH enabled |
| Window doesn't appear | Make sure you're running the script directly, not importing it |
| Non-numeric bet shows "Invalid" | Only type whole numbers (e.g., `10`, not `ten` or `10.5`) |

---

## 🤝 Contributing

This is a beginner project, and contributions are welcome! Feel free to:

- ⭐ Star the repository if you found it helpful
- 🐛 Open an issue if you find a bug
- 🔧 Fork and submit a pull request with improvements

Ideas for improvement:
- Add more symbols and reels
- Add animations or sound effects
- Track a high score
- Add a "Reset Balance" button

---

## 👤 Author

**Nawfat Nahin**
- GitHub: [@Nawfatnahin](https://github.com/Nawfatnahin)

---

## This project is open source.

---

<p align="center">Made with ❤️ and Python</p>
