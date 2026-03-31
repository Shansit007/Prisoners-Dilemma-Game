# 🧠 Prisoner's Dilemma Tournament

A Python-based simulation of the **Iterated Prisoner’s Dilemma**, where multiple strategies compete against each other in a tournament to determine the most effective long-term decision-making behavior.

---

## 📌 Project Overview

This project models **multi-agent strategic interactions** using the classic concept of the **Prisoner’s Dilemma** from game theory.

Each strategy plays against every other strategy over multiple rounds, and their performance is evaluated based on accumulated scores.

---

## 🎯 Objective

* Simulate repeated interactions between agents
* Analyze cooperation vs defection behavior
* Identify the most successful strategies over time
* Demonstrate emergence of trust and retaliation patterns

---

## ⚙️ How It Works

1. All strategy files are loaded from the `exampleStrats/` folder
2. Each strategy plays against every other strategy (pairwise)
3. Each match runs for **200+ randomized turns**
4. Moves are stored in a **history matrix**
5. Scores are calculated based on payoff rules
6. Final rankings are generated and saved in `results.txt`

---

## 🧩 Payoff Matrix

|               | Opponent Cooperates | Opponent Defects |
| ------------- | ------------------- | ---------------- |
| **Cooperate** | +3, +3              | 0, +5            |
| **Defect**    | +5, 0               | +1, +1           |

---

## 📁 Project Structure

```
PrisonersDilemmaTournament/
│
├── code/
│   ├── prisonersDilemma.py     # Main tournament logic
│   ├── exampleStrats/          # Strategy implementations
│   │   ├── titForTat.py
│   │   ├── grimTrigger.py
│   │   ├── detective.py
│   │   ├── simpleton.py
│   │   ├── alwaysCooperate.py
│   │   ├── alwaysDefect.py
│   │   └── ...
│
├── results.txt                 # Output leaderboard (generated)
├── README.md
```

---

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/your-username/PrisonersDilemmaTournament.git
cd PrisonersDilemmaTournament/code
```

### 2. Run the simulation

```bash
python prisonersDilemma.py
```

### 3. View results

* Output will be saved in `results.txt`

---

## 🤖 Available Strategies

Some implemented strategies include:

* **Tit-for-Tat** – Cooperate first, then mimic opponent
* **Grim Trigger** – Cooperate until betrayed, then defect forever
* **Detective** – Tests opponent and adapts behavior
* **Simpleton** – Switches behavior based on opponent response
* **Always Cooperate / Defect** – Basic baseline strategies
* **Random Strategy** – Random decisions
* **Forgiving Tit-for-Tat (FTFT)** – More tolerant version

---

## 🧠 Key Concepts

* Game Theory
* Iterated Decision Making
* Multi-Agent Systems
* Cooperation vs Competition
* Strategy Optimization

---

## ➕ Adding Your Own Strategy

Create a new `.py` file inside `exampleStrats/`:

```python
def strategy(history, memory):
    # history: past moves
    # memory: stored state
    return 1, None  # Example: always cooperate
```

Your strategy will automatically be included in the tournament.

---

## 📊 Output

The `results.txt` file contains:

* Match-by-match results
* Move history
* Final scores
* Ranked leaderboard of strategies

---

## 💡 Insights

* Purely selfish strategies fail in long-term interactions
* Cooperative strategies with retaliation perform best
* Balance between trust and punishment is key

---

## 🚀 Applications

* Artificial Intelligence
* Economics & Negotiation Systems
* Evolutionary Algorithms
* Behavioral Strategy Modeling

---

## 👨‍💻 Author

**Shansit Suman**
B.Tech CSE (AI/ML), VIT Bhopal

---
