# 🧠 Prisoner's Dilemma Tournament

A Python-based simulation of the **Iterated Prisoner’s Dilemma**, where multiple strategies compete against each other in a tournament to determine the most effective long-term decision-making behavior.

---

## 📌 Project Overview

This project models **multi-agent strategic interactions** using the classic concept of the **Prisoner’s Dilemma** from game theory.

It goes beyond traditional simulation by **integrating core Computer Science concepts with behavioral and emotional intelligence (EI) principles**, demonstrating how trust, retaliation, forgiveness, and exploitation emerge in repeated interactions.

---

## 🎯 Objective

* Simulate repeated interactions between intelligent agents
* Analyze cooperation vs defection behavior
* Model **trust-building, betrayal, and forgiveness** dynamics
* Bridge **algorithmic decision-making with emotional intelligence (EI)**
* Identify the most successful strategies over time

---

## ⚙️ How It Works

1. All strategy files are loaded from the `exampleStrats/` folder
2. Each strategy plays against every other strategy (pairwise)
3. Each match runs for **200+ randomized turns**
4. Moves are stored in a **history matrix**
5. Strategies use past interactions (memory) to make decisions
6. Scores are calculated based on payoff rules
7. Final rankings are generated and saved in `results.txt`

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
git clone https://github.com/Shansit007/Prisoners-Dilemma-Game.git
cd PrisonersDilemmaTournament/code
```

### 2. Install dependencies(optional)

```bash
pip install numpy
```

### 3. Run the simulation

```bash
python prisonersDilemma.py
```

### 4. View results

* Output will be saved in `results.txt`

---

## 🤖 Strategy Design & Behavioral Intelligence

Each strategy represents a **distinct behavioral pattern**, mimicking real-world human decision-making:

* **Tit-for-Tat** → Reciprocity & fairness
* **Grim Trigger** → Zero-tolerance / strict punishment
* **Detective** → Analytical testing + adaptive behavior
* **Simpleton** → Reactive emotional adjustment
* **Always Cooperate** → Blind trust
* **Always Defect** → Pure selfishness
* **Joss** → Opportunistic exploitation
* **FTFT** → Forgiveness & tolerance

These strategies collectively demonstrate how **emotional intelligence traits like trust, revenge, forgiveness, and adaptability** can be encoded into algorithmic logic.

---

## 🧠 Key Concepts

* Game Theory
* Multi-Agent Systems
* Iterated Decision Making
* Strategy Optimization
* Behavioral Modeling
* **Emotional Intelligence in AI Systems**
* Trust & Cooperation Dynamics

---

## ➕ Adding Your Own Strategy

Create a new `.py` file inside `exampleStrats/`:

```python
def strategy(history, memory):
    # history: past interactions
    # memory: internal state (can model emotions/logic)
    return 1, None
```

This flexibility allows you to design strategies that simulate:

* Forgiveness thresholds
* Trust decay
* Risk-taking behavior
* Emotional retaliation patterns

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
* **Balanced behavior (trust + punishment) yields optimal results**
* Emotional intelligence-inspired strategies outperform rigid ones

---

## 🚀 Applications

* Artificial Intelligence & Multi-Agent Systems
* Behavioral Economics
* Negotiation & Decision Systems
* Reinforcement Learning Concepts
* Social Simulation Models
* **Human-AI Interaction Modeling**

---

## 👨‍💻 Author

**Shansit Suman**
B.Tech CSE (AI/ML), VIT Bhopal

---
