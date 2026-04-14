# 🐍 Snake Game

![Python](https://img.shields.io/badge/python-3.9%2B-blue.svg)
![Pygame](https://img.shields.io/badge/Pygame-2.6.1-red.svg)

![License](https://img.shields.io/badge/license-MIT-green.svg)  
![Contributions](https://img.shields.io/badge/contributions-welcome-orange.svg)  

<p align="center">
  <img src="img/Snake-game.gif" alt="Snake game exemple">
</p>


---

## 📝 Project Description 
This project is a **classic Snake game** built with Pygame.  
You can play manually, or let the snake move automatically with random actions.  

The game also provides detailed **distance calculations** to food and walls (in all 8 directions).  
These metrics are useful for **training AI agents**, and this codebase was used as the environment for multiple **Reinforcement Learning** projects:
[Snake AI - DT](https://github.com/Thibault-GAREL/AI_snake_decision_tree_version), [Snake AI - GA](https://github.com/Thibault-GAREL/AI_snake_genetic_version), [Snake AI - DQL](https://github.com/Thibault-GAREL/AI_snake_DQN_version) and [Snake AI - PPO](https://github.com/Thibault-GAREL/AI_snake_PPO_version).  

A complete **XAI (Explainable AI) report** was written across these projects, analyzing and explaining the decision-making of each agent. 📄

---

## ⚙️ Features
  🎮 Playable Snake game with smooth movement  

  🍎 Food spawning and snake growth  

  🟩 Detailed snake rendering (head, body, tail with unique visuals)  

  📏 Functions to compute distances to **walls** and **food** in all directions (N, S, E, W, NE, NW, SE, SW)  

  🤖 Option to toggle **player mode** or **random agent mode**  

  🖼️ Optional checkerboard display for debugging  

---

## ⚙️ How it works

  🕹️ Control the snake manually with the arrow keys (**UP, DOWN, LEFT, RIGHT**) or let the random agent play.  

  🍎 When the snake eats food, it grows by 1 segment and new food is generated.  

  💥 Collision with walls or itself ends the game.  

  📊 Extra functions calculate distances to walls and food, allowing the game to be used as an environment for AI.  

---

## 🗺️ Schema  
💡 The snake is represented as a list of `Snake` objects, while food is a simple `food` object.  
The environment provides **distance functions** that can be reused in AI or reinforcement learning projects.  

---

## 📂 Repository structure  
```bash
├── img/
│   └── example.png
│
├── snake.py
│
├── LICENSE
├── README.md
```

---

## 💻 Run it on Your PC  
Clone the repository and install dependencies:  
```bash
git clone https://github.com/Thibault-GAREL/snake_game.git
cd snake_game

python -m venv .venv # if you don't have a virtual environment
source .venv/bin/activate   # Linux / macOS
.venv\Scripts\activate      # Windows

pip install pygame

python main.py
```

---

## 📖 Inspiration / Sources  
Code created by me 😎, Thibault GAREL - [Github](https://github.com/Thibault-GAREL)