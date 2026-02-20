---

# ME5406 Project – Part 1

Reinforcement Learning with Q-Learning, SARSA, First Visit Monte Carlo and DQN

## Overview

This project implements reinforcement learning algorithms using:

* Python
* PyTorch
* Gymnasium
* NumPy
* Matplotlib
* Jupyter Notebook

---

# Installation Instructions

## I. Clone or Download the Project

Make sure the notebook file is in your working directory:

```
part_1_project_ME5406_FINAL.ipynb
```

---

## II. Create a Virtual Environment (Recommended)

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

## III. Install Required Packages

Run:

```bash
pip install matplotlib numpy torch pillow ipython pyyaml ipykernel
```

Or create a `requirements.txt` file:

```
matplotlib
numpy
torch
pillow
ipython
pyyaml
ipykernel
```

Then install:

```bash
pip install -r requirements.txt
```

---

# How to Run the Code

## Option 1: Run with Jupyter Notebook (Recommended)
1. (Optional: Install kernel for a new python environment) Run the following to install the kernel to `.local/share/jupyter/kernels/`
```bash
python -m ipykernel install --user --name <NAME>
```
2. Run  
```bash
jupyter lab part_1_project_ME5406_FINAL.ipynb
```
3. If a new kernel was insatalled, choose it when running jupyter.


Then:
1. Click **"Run All"**
2. Or run cells sequentially from top to bottom
---


## Torch Installation Problems

If needed, install from official PyTorch website:
[https://pytorch.org/get-started/locally/](https://pytorch.org/get-started/locally/)

---
