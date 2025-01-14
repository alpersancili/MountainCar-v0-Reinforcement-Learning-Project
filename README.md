# MountainCar-v0-Reinforcement-Learning-Project
This project implements Q-learning, a fundamental reinforcement learning algorithm, to solve the classic MountainCar-v0 environment provided by the gymnasium library. The goal of the agent is to drive an underpowered car up a steep hill by building momentum through strategic actions.

🔍 Overview
Problem Statement
The agent starts at the bottom of a valley and must reach the flag at the top of the right hill. However, the car's engine is too weak to climb the hill directly, requiring the agent to leverage momentum by moving back and forth.

Approach
The solution involves:
Discretizing the continuous state space into bins for position and velocity.
Implementing the Q-learning algorithm to iteratively learn an optimal policy.
Using an epsilon-greedy strategy to balance exploration and exploitation during training.

📁 Project Structure
mountain_car_q.py: Main script implementing the Q-learning algorithm and training/testing the agent.

Q-Learning Implementation:
Discretizes the state space into 20 bins each for position and velocity.
Updates Q-values based on rewards and future state predictions.

Epsilon-Greedy Exploration:
Gradually decays the exploration rate (epsilon) to encourage exploitation in later episodes.

Visualization:
Plots the moving average of rewards over 100 episodes to track learning progress.

Save & Load Functionality:
Saves the Q-table to a file for reuse in testing mode.

📊 Results
The training process aims to maximize cumulative rewards by learning an optimal policy. The reward graph (mountain_car.png) illustrates the agent's performance improvement over time.

https://github.com/user-attachments/assets/afa728ac-f645-4cab-ba35-6af18e2a84c8



