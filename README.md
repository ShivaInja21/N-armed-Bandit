# N‑Armed Bandit Simulator 🎰

This repository implements a classical **N‑Armed Bandit** problem using the **ε‑greedy strategy** (and optionally other algorithms) in Python via a Jupyter Notebook. The agent learns to maximize long-term rewards by balancing **exploration** and **exploitation** over multiple independent bandit "arms" with unknown payoff distributions.

---

## 📌 Features

- Configurable number of arms (`n_arms`) and trials (`n_steps`)
- Implemented **ε‑greedy algorithm** with tunable ε
- Collects and visualizes:
  - Cumulative reward over time
  - Optimal action percentage per time step
  - Optional comparison between greedy and exploratory policies
- Supports multiple independent runs to evaluate statistical performance
- Simple, educational implementation ideal for learning reinforcement learning basics

---



## 📖 Overview of the Notebook

- **Initialization**: Defines true payoff values (`q*(a)`) via sampled normal distributions.
- **ε‑greedy strategy**:
  - With probability ε, choose a random arm (explore)
  - Otherwise, choose the currently estimated best arm (exploit)
- **Simulation loop**:
  - For each time step:
    - Choose an arm
    - Receive reward (sampled from that arm’s distribution)
    - Update estimated averages \(Q(a)\)
  - Tracks running reward and optimal action statistics
- **Visualization**:
  - Plots average reward vs. time
  - (Optional) plots % of optimal actions vs. time

---

## 📊 What You’ll Learn

- Core concepts of the multi‑armed bandit problem
- Trade-off between exploration (trying new options) vs. exploitation (using known good options)
- How ε impacts learning performance over time
- Techniques for aggregating results across multiple simulation runs

---

## 🧩 Extensions & Experimentation

Consider expanding the project by:

- Varying ε (e.g., 0, 0.01, 0.1, 0.2) and comparing results
- Implementing other strategies like **softmax**, **UCB**, or **Thompson Sampling**
- Adding non-stationarity (i.e., changing arm reward distributions over time)
- Packaging simulation results for quantitative comparison

---

Developed by **ShivaInja21**
