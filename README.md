# 🎰 Python Slot Machine Simulator

![Python](https://img.shields.io/badge/Python-3.x-blue.svg?logo=python&logoColor=white)
![Interface](https://img.shields.io/badge/Interface-CLI-yellow)
![Focus](https://img.shields.io/badge/Focus-Control_Flow-green)
![Logic](https://img.shields.io/badge/Concept-Randomization_&_Validation-purple)

An interactive, terminal-based slot machine game allowing users to deposit virtual funds, place multi-line bets, and spin until they cash out or go broke.

**The Problem:** Transitioning from simple, single-execution scripts to continuous, state-driven applications is a major hurdle for beginners. Real-world applications require managing unpredictable user input dynamically without crashing the program, alongside maintaining active variables (like a user's balance) across multiple loops.

**The Solution:** A functional CLI game that forces practical problem-solving. While inspired by a "Tech With Tim" tutorial, this project was built using independent logic and problem-solving to genuinely understand the *why* behind the code. It serves as a practical sandbox for implementing continuous `while` loops, strict input validation (`try/except`, `.isdigit()`), and nested data structures.

---

## 📸 Capabilities
* **Dynamic Betting System:** Users can choose to bet on 1, 2, or up to 3 lines simultaneously, with the system multiplying their wager by the line value.
* **State Management (Bankroll):** Tracks the player's balance dynamically, adding winnings and subtracting losses in real-time. Prevents users from betting more money than they currently hold.
* **Bulletproof Input Validation:** Built to handle human error. Uses string methods like `.isdigit()` and `try/except` blocks to catch invalid keystrokes and politely prompt the user to try again instead of crashing the application.
* **Continuous Game Loop:** Allows the player to hit "Enter" to seamlessly spin again or type "q" to cash out and safely terminate the program.

## 🛠 Tech Stack
| Component | Technology | Description |
| :--- | :--- | :--- |
| **Core** | Python 3.x | Main language for all logic and game mechanics |
| **Mathematics** | `random` Module | Generates the weighted, randomized outcomes for the slot wheels |
| **Data Handling** | Lists & Dictionaries | Used to store and map the values and frequencies of slot symbols |
| **Environment** | CLI | Executed natively in the terminal |

## 🚀 Quick Start

```bash
# 1. Clone the repo
git clone [https://github.com/cunhanina/Slot-Machine.git](https://github.com/cunhanina/Slot-Machine.git)
cd Slot-Machine

# 2. Run the game
python slotmachine.py
```

## 🧠 System Architecture
This project is built around a robust procedural event loop:
1.  **Initialization Phase:** The application asks for an initial deposit, sanitizing the input to ensure it is a valid integer greater than zero.
2.  **The Game Loop:** A continuous `while` loop encapsulates the core gameplay. It checks the current balance, calculates the total risk (bet $\times$ lines), and validates that the user can afford the spin.
3.  **Spin Engine:** The `random` library is utilized to select symbols based on predetermined frequencies. The program evaluates the generated columns and rows to check for matching patterns across the active bet lines.
4.  **Resolution:** Payouts are calculated, the user's balance is mutated, and the loop repeats until the user manually triggers the exit condition or the balance drops to zero.

---

<div align="center">

### Built with ❤️ by [Nina Cunha](https://github.com/maxykoin)

**Data Science · Industrial Automation · Software Engineering**

[![LinkedIn](https://img.shields.io/badge/Connect-LinkedIn-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/nscunha/)
[![GitHub](https://img.shields.io/badge/Follow-GitHub-181717?style=for-the-badge&logo=github)](https://github.com/maxykoin)

</div>

---
