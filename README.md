# 🎮 Python Mini Games Collection

A collection of beginner-friendly Python games built with core programming concepts like loops, conditionals, functions, and user input — implemented in Jupyter Notebook.

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success)
![Level](https://img.shields.io/badge/Level-Beginner-green)

---

## 📌 About This Repository

This repository contains **two classic console mini-games** written in Python. They were created as practice projects for learning Python fundamentals and are perfect examples of interactive command-line programs.

| # | Game | Description | Key Concepts |
|---|------|-------------|--------------|
| 1 | 🔢 **Guess Number Game** | Guess a secret number between 1–100 with Warm / Cold hints | `random`, `while` loop, `abs()`, input validation, list tracking |
| 2 | 🔄 **Changing Position Game** | Replace items in a 3-element list by position | `functions`, `input()`, list indexing, `clear_output`, game loop |

---

## 📁 Project Structure

```text
python-mini-games/
│
├── README.md
│
├── guess-number-game/
│   ├── Guess-Number-Game.ipynb
│   └── README.md
│
└── changing-position-game/
    ├── Changing-Position-Game.ipynb
    └── README.md
```

> 💡 **Tip:** Each game has its own folder with a dedicated README, so you can run, share, or expand them independently while keeping one professional main repository.

---

## 🎯 Games Overview

### 1️⃣ 🔢 Guess Number Game — `guess-number-game/`

A Warm / Cold guessing game. The computer picks a random number between **1 and 100**, and you have to find it.

**Rules:**
- If your first guess is **within 10** of the secret number → `WARM!`
- If it is **more than 10 away** → `COLD!`
- From the second guess on:
  - Closer than previous guess → `WARMER!`
  - Farther than previous guess → `COLDER!`
- Guesses outside 1–100 → `OUT OF BOUNDS!`
- Win message shows the number of attempts.

**Example run:**

```text
WELCOME TO GUESS ME
I'm thinking of a number between 1 and 100
...
What is your guess? 15
Warm!
What is your guess? 25
Colder!
What is your guess? 11
Congratulation! You guessed it in only 10 guesses!
```

**Run it:**

```bash
cd guess-number-game
jupyter notebook "Guess Number Game.ipynb"
```

---

### 2️⃣ 🔄 Changing Position Game — `changing-position-game/`

A simple interactive list-manipulation game. You see a list `[0, 1, 2]` and replace any position with your own text.

**How it plays:**
1. Current list is displayed: `Here is the current list` → `[0, 1, 2]`
2. You pick a position: `0`, `1`, or `2` (invalid input is rejected)
3. You type a string to place at that position
4. Updated list is shown
5. You choose `Y` to continue or `N` to quit → `Goodbye!`

**Example run:**

```text
Here is the current list
[0, 1, 2]
Pick a position to replace (0, 1, 2): 1
Type a string to place at the position: Hello
Here is the current list
[0, 'Hello', 2]
Would you like to keep playing? Y or N N
Goodbye!
```

**Run it:**

```bash
cd changing-position-game
jupyter notebook "Changing Position Game.ipynb"
```

---

## 🚀 Getting Started

### Requirements

- Python **3.8+**
- Jupyter Notebook or JupyterLab

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/NazaninFereydouniF/Numbers-Game
cd python-mini-games

# 2. (Optional) Create a virtual environment
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

# 3. Install Jupyter
pip install notebook ipython

# 4. Launch
jupyter notebook
```

Then open any `.ipynb` file and run all cells.

> `Changing Position Game` uses `IPython.display.clear_output` — it works best inside Jupyter. For terminal use, replace `clear_output()` with `print("\n" * 20)` or `os.system('cls'/'clear')`.

---

## 🧠 What I Learned

- Generating random numbers with `random.randint`
- `while True` game loops with `break` / `continue`
- Input validation and handling `OUT OF BOUNDS`
- Tracking history with lists (`guesses = [0]`)
- Comparing distances with `abs()`
- Writing reusable functions (`display_game`, `position_choice`, `replacement_choice`, `game_on_choice`)
- Improving UX with `clear_output()`

---

## 🔮 Future Improvements

- [ ] Add `.py` standalone versions (no Jupyter required)
- [ ] Add difficulty levels to Guess Number Game (e.g., 1–50 / 1–500)
- [ ] Add attempt limit and scoring system
- [ ] Add input error handling for non-numeric guesses (`try/except ValueError`)
- [ ] Add Tic-Tac-Toe as Game #3

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request to add a new mini-game or improvement.

---

⭐ If you found this helpful, please give it a star!
