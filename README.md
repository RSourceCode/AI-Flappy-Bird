# 🐦 Flappy AI Bird

An AI-powered version of the classic *Flappy Bird* game built using **Python**, **Pygame**, and **NEAT (NeuroEvolution of Augmenting Topologies)**. The AI learns how to play the game through evolution over generations without hardcoding any rules.

---

## 🚀 Features

* **AI-controlled birds** that learn to navigate pipes using neural networks.
* Implements **NEAT algorithm** to evolve the birds' decision-making over time.
* Real-time **fitness scoring** and **visualization**.
* Built entirely with **Python** and **Pygame**.
* Train once and watch multiple AI birds fly intelligently.

---

## 🧠 Tech Stack

* **Python 3**
* **Pygame** (for game development and rendering)
* **NEAT-Python** (for evolving neural networks)

---

## 📁 Project Structure

```
Flappy-AI-Bird/
│
├── imgs/                    # Folder containing game assets
│   ├── bird1.png
│   ├── bird2.png
│   ├── bird3.png
│   ├── pipe.png
│   ├── base.png
│   └── bg.png
│
├── config-feedforward.txt   # NEAT configuration file
├── flappy_ai.py             # Main game + AI logic
└── README.md                # Project documentation
```

---

## 🧬 How It Works

* Each bird is represented by a **neural network**.
* Inputs to the neural network:

  * Bird's current vertical position.
  * Distance between bird and top of next pipe.
  * Distance between bird and bottom of next pipe.
* Output:

  * A value determining whether to **jump** or not.
* The **NEAT algorithm** adjusts the weights and structure of the networks across generations to improve performance.

---

## ▶️ Running the Project

### 1. Install Dependencies

```bash
pip install pygame neat-python
```

### 2. Run the Game

```bash
python flappy_ai.py
```

Make sure the `imgs/` folder and `config-feedforward.txt` are in the same directory as your script.

---

## 🧾 NEAT Configuration

The file `config-feedforward.txt` contains the parameters for evolving the neural networks such as:

* Population size
* Mutation rate
* Number of inputs/outputs
* Network structure constraints

Adjust it for experimentation and performance tuning.
