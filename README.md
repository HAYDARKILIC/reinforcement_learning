# Reinforcement Learning

** Haydar Kilic, Artificial Intelligence Engineering **


---

## 📖 Source Textbook

The Jupyter notebooks in this repository contain Python implementations of the theoretical content in Reinforcement Learning Class.

---

## 📂 Contents

| Notebook | Topic | Algorithms |
|----------|-------|------------|
| [`RL_Lecture1_MDP_EN.ipynb`](RL_Lecture1_MDP_EN.ipynb) | Markov Decision Processes | Value Iteration, Policy Iteration |
| [`RL_Lecture2_ValuePrediction_EN.ipynb`](RL_Lecture2_ValuePrediction_EN.ipynb) | Value Prediction Problems | TD(0), Monte Carlo, TD(λ), LSTD |
| [`RL_Lecture3_Control_EN.ipynb`](RL_Lecture3_Control_EN.ipynb) | Control Algorithms | Q-Learning, SARSA, Actor-Critic, REINFORCE, UCB |

---

## 🗂 Notebook Details

### 📓 Chapter 1 — Markov Decision Processes
`RL_Lecture1_MDP_EN.ipynb`

- MDP definition: state space, action space, transition kernel, reward function
- Value functions and Bellman equations
- **Value Iteration** — Bellman optimality operator $T^*$, geometric convergence guarantee
- **Policy Iteration** — policy evaluation + improvement loop
- 📦 Application 1: GridWorld (4×4 stochastic grid)
- 📦 Application 2: Inventory Control (Example 1.1 — Poisson demand, (s,S) policy)
- 📦 Application 3: Gambler's Problem (Example 1.2 — varying win probabilities)

### 📓 Chapter 2 — Value Prediction Problems
`RL_Lecture2_ValuePrediction_EN.ipynb`

- **Tabular TD(0)** (Algorithm 1) — bootstrapping, convergence analysis for different learning rates
- **Every-Visit Monte Carlo** (Algorithm 2) — backward return computation, comparison with TD(0)
- **TD(λ)** — eligibility traces, sweep over λ ∈ [0,1]
- **Linear Function Approximation** — TD(0) in large/continuous state spaces
- **LSTD(0)** (Algorithm 7) — least-squares solution, single-pass convergence
- Comprehensive RMSE-based comparison of all methods

### 📓 Chapter 3 — Control Algorithms
`RL_Lecture3_Control_EN.ipynb`

- **Multi-Armed Bandits & UCB1** (Algorithm 5) — exploration-exploitation trade-off, Thompson Sampling
- **Q-Learning** (Algorithm 12) — off-policy TD control (Watkins 1989)
- **SARSA** — on-policy TD control, head-to-head comparison with Q-Learning
- **Actor-Critic** — softmax policy + TD critic
- **REINFORCE** — policy gradient (Williams 1992), with and without baseline
- Multi-run statistical comparison of all control algorithms

---

## 🚀 Installation and Usage

### 1. Install Dependencies

```bash
pip install -r requirements.txt
```

### 2. Launch Jupyter

```bash
jupyter notebook
```

Then open the desired `.ipynb` file in your browser.

### 3. Recommended Order

```
RL_Lecture1_MDP_EN.ipynb  →  RL_Lecture2_ValuePrediction_EN.ipynb  →  RL_Lecture3_Control_EN.ipynb
```

Each notebook is **self-contained** — no dependency on previous notebooks.

---

## ⚙️ Requirements

```
numpy >= 1.24
matplotlib >= 3.7
scipy >= 1.10
jupyter >= 1.0
notebook >= 7.0
```

Python 3.9+ is recommended.

## 📖 Kaynak Kitap

Szepesvári, C. (2022). Algorithms for reinforcement learning. Springer nature.

---

