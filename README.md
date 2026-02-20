Here is a clean **README.md** you can copy directly into your project.

---

# ME5406 Project – Part 1

Reinforcement Learning with SARSA and Deep RL

## 📌 Overview

This project implements reinforcement learning algorithms (including SARSA and deep learning–based approaches) using:

* Python
* PyTorch
* Gymnasium
* NumPy
* Matplotlib
* Jupyter Notebook

The environment used includes:

* `FrozenLake-v1` from Gymnasium

---

# 🛠 Installation Instructions

## 1️⃣ Clone or Download the Project

Make sure the notebook file is in your working directory:

```
part_1_project_ME5406_FINAL.ipynb
```

---

## 2️⃣ Create a Virtual Environment (Recommended)

```bash
python -m venv venv
```

Activate it:

**Windows**

```bash
venv\Scripts\activate
```

**Mac/Linux**

```bash
source venv/bin/activate
```

---

## 3️⃣ Install Required Packages

Run:

```bash
pip install gymnasium matplotlib numpy torch pillow ipython
```

Or create a `requirements.txt` file:

```
gymnasium
matplotlib
numpy
torch
pillow
ipython
```

Then install:

```bash
pip install -r requirements.txt
```

---

# ▶️ How to Run the Code

## Option 1: Run with Jupyter Notebook (Recommended)

Start Jupyter:

```bash
jupyter notebook
```

Open:

```
part_1_project_ME5406_FINAL.ipynb
```

Then:

1. Click **"Run All"**
2. Or run cells sequentially from top to bottom

⚠️ It is important to run cells in order because:

* Functions are defined earlier
* Training depends on earlier imports and definitions

---

## 🧠 Project Structure

The notebook includes:

### 1️⃣ Imports

Libraries such as:

* PyTorch (neural networks and optimization)
* Gymnasium (environment simulation)
* NumPy (numerical operations)
* Matplotlib (visualization)

---

### 2️⃣ SARSA Implementation

Includes:

* `epsilon_greedy_action()`
* `sarsa()` training function
* `vis_sarsa()` visualization function

Example environment creation:

```python
env = gym.make('FrozenLake-v1', is_slippery=True, render_mode='rgb_array')
```

Training example:

```python
Q, rewards = sarsa(env)
```

Visualization:

```python
vis_sarsa(env, Q)
```

---

### 3️⃣ Deep Reinforcement Learning (PyTorch)

If included in later cells:

* Neural network model definitions
* Policy networks
* Optimization using `torch.optim`
* Action sampling using `Categorical` distribution

Make sure GPU is available if using CUDA (optional).

---

# 📊 Expected Output

* Console training logs:

  ```
  Episode 10000, Avg Reward: ...
  ```
* Reward plots
* Environment visualization (FrozenLake grid)
* Learned policy behavior

---

# ⚠️ Common Issues & Fixes

### 1. Environment Rendering Error

Make sure you use:

```python
render_mode='rgb_array'
```

---

### 2. Gymnasium Not Found

Install:

```bash
pip install gymnasium
```

---

### 3. Torch Installation Problems

If needed, install from official PyTorch website:
[https://pytorch.org/get-started/locally/](https://pytorch.org/get-started/locally/)

---

# 💻 Recommended Python Version

Python 3.9 – 3.11

Check version:

```bash
python --version
```

---

# 📈 Customization

You can modify:

* Learning rate (`alpha`)
* Discount factor (`gamma`)
* Exploration rate (`epsilon`)
* Number of episodes
* Environment parameters (`is_slippery=True/False`)

Example:

```python
Q, rewards = sarsa(env, episodes=50000, epsilon=0.2)
```

---
