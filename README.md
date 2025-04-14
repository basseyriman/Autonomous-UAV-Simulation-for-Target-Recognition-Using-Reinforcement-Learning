# 🚁 Autonomous UAV Simulation for Target Recognition Using Reinforcement Learning

## 👨‍💻 Author: Bassey Riman  
**Student ID:** Q2034066  
**Email:** Q2034066@live.tees.ac.uk

---

## 📌 Project Overview

This project explores the simulation of Unmanned Aerial Vehicles (UAVs) for autonomous **target recognition** using **Reinforcement Learning (RL)** techniques—specifically 
**Q-learning**. The UAV navigates a dynamic environment populated with obstacles and a simulated target, learning to make optimal movement decisions to identify targets through trial-and-error learning.

The simulation models real-world surveillance challenges, highlighting how UAVs powered by intelligent RL algorithms can enhance **military intelligence gathering** and **autonomous navigation** capabilities.

---

## 🎯 Key Features

- UAV agent driven by **Q-learning RL algorithm**
- Realistic environment with obstacles and target object
- Intelligent target detection and navigation
- Simulated aerial visuals and military drone representation
- Interactive visualization and training analytics

---

## 📽️ External Media Assets

- **Military Drone Agent:**  
  ![Drone](https://www.pngall.com/military-drone-png/download/50108)

- **Simulated Sky Environment:**  
  [Pexels Sky Video](https://www.pexels.com/video/thick-fogs-covering-the-mountain-valley-4763084/)

- **Target (Spaceship) Image:**  
  ![Spaceship](https://www.pngkey.com/detail/u2e6q8t4t4r5u2a9_star-wars-rpg-nave-star-wars-star-trek/)

---

## 🛠 Installation Requirements

Ensure your environment is properly set up with the following dependencies:

```bash
pip install --upgrade pygame
pip install imageio
pip install imageio[ffmpeg]
pip install matplotlib

---
🧠 Libraries Used
import pygame
import random
import math
import time
import numpy as np
import imageio
import matplotlib.pyplot as plt

---
📐 Reinforcement Learning Setup
State & Action Definitions
STATE_SPACE_SIZE = 4
ACTION_SPACE_SIZE = 4
Q_TABLE = np.zeros((STATE_SPACE_SIZE, ACTION_SPACE_SIZE))

---
Reward Strategy
REWARD_TARGET_IDENTIFIED = 200
REWARD_MOVEMENT = 50
PENALTY_COLLISION = -50
PENALTY_TIME = -20
REWARD_DISTANCE_TO_TARGET = 100

---
Direction Mapping
DIRECTION_MAPPING = {'UP': 0, 'DOWN': 1, 'LEFT': 2, 'RIGHT': 3}

---
🧩 Key Functions
get_state(): Derives the current state based on UAV and target positions.

select_action(state): Uses ε-greedy policy to select an action.

update_q_table(state, action, reward, next_state): Applies Q-learning to update the agent’s knowledge.

obstacle_collision(x, y): Detects collision with obstacles.

📊 Visualization
The project uses Matplotlib and Pygame for real-time simulation and performance visualization, such as:

UAV movements over time

State transitions

Rewards and penalties log

Training progress and Q-table updates

💡 Use Cases & Impact
Military Surveillance Simulation

Autonomous Navigation Research

RL Algorithm Application

Obstacle Avoidance Testing

This project provides a testbed for future enhancement in drone-based RL applications for reconnaissance, search-and-rescue, and military intelligence.

📂 Project Structure
.
├── uav_simulation.py
├── assets/
│   ├── drone.png
│   ├── spaceship.png
│   └── background_sky.mp4
├── output/
│   └── training_video.mp4
├── README.md
└── requirements.txt

---
🚀 Getting Started
To run the project:

Clone this repository
git clone https://github.com/yourusername/uav-rl-simulation.git

Install dependencies
pip install -r requirements.txt

Run the simulation
python uav_simulation.py

🧠 Future Improvements
Implement Deep Q-Networks (DQN) for continuous state-action spaces

Add multi-agent scenarios for cooperative/competitive behavior

Integrate with ROS/Gazebo for real-world drone emulation

Add GUI interface for user interaction

📜 License
MIT License - Feel free to use and contribute!

🙏 Acknowledgments
Pygame Community: https://www.pygame.org/contribute.html

Open-source media from PNGAll, Pexels, and PNGKey

Teesside University for academic support

🔗 Contact
For questions or collaborations, contact:
📧 Q2034066@live.tees.ac.uk
