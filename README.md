# Acrobot-v1 RL Comparison

A small reinforcement learning research project that compares **Q-learning** and **SARSA** on OpenAI Gymnasium's classic control environment **Acrobot-v1** using a simple discretized state-value table.

The project is implemented as a single Jupyter notebook (`main.ipynb`) that trains both algorithms, plots learning curves, and generates GIFs of the learned policies.

---

## 🚀 What this project does

- Implements **Q-learning** and **SARSA** agents for the `Acrobot-v1` environment.
- Uses **state discretization** to convert continuous observations into a discrete state space.
- Compares learning performance via **learning curves** (returns over episodes).
- Generates **policy visualization GIFs** showing the agent controlling the Acrobot.

---

## ✅ Why this project is useful

- ✅ Great reference for understanding how tabular RL algorithms behave on continuous environments.
- ✅ Easy-to-follow structure: configuration, training, evaluation, and visualization all in one notebook.
- ✅ Ready-made comparison of **on-policy (SARSA)** vs **off-policy (Q-learning)** behavior.

---

## 🧰 Getting started

### 1) Clone the repo

```bash
git clone <your-repo-url> "Acrobot-v1"
cd "Acrobot-v1"
```

### 2) Create and activate a Python virtual environment (recommended)

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3) Install dependencies

There is no `requirements.txt` in this repo, but the notebook depends on:

- `gymnasium` (Gymnasium v1 environment suite)
- `numpy`
- `matplotlib`
- `imageio`
- `Pillow`

Install the required packages:

```bash
pip install gymnasium numpy matplotlib imageio Pillow
```

### 4) Run the notebook

Start Jupyter and open `main.ipynb`:

```bash
jupyter notebook main.ipynb
```

Then run all cells in order. The notebook will:

1. Tune hyperparameters (learning rate, exploration rate) for both SARSA and Q-learning
2. Train each algorithm for multiple random seeds
3. Plot learning curves with confidence intervals
4. Generate GIFs of the learned policies (`sarsa_acrobot.gif`, `qlearning_acrobot.gif`)

---

## 📁 Important files

- `main.ipynb` – Core implementation (training loop, evaluation, plotting, GIF export)
- `sarsa_acrobot.gif` – Example output (SARSA policy rollout)
- `qlearning_acrobot.gif` – Example output (Q-learning policy rollout)

---

## 🆘 Where to get help

If you run into issues:

- Check that you’re using a compatible Python version (the included `.venv` uses Python 3.9.x).
- Ensure `gymnasium` is installed and working (some environments may require additional system dependencies).

For general Gymnasium help, see the official docs:

- https://gymnasium.farama.org/

---

## 🤝 Contributing

This project does not currently include a formal `CONTRIBUTING.md`, but contributions are welcome.

If you want to contribute:

1. Fork the repo
2. Create a feature branch
3. Open a pull request with a short description of what changed

---

## 🧑‍💻 Maintainers

- Maintained by the repository owner.

> ⚠️ Note: This repo does not include an explicit license file. Add a `LICENSE` if you intend to share or publish it publicly.
