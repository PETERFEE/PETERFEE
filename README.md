ML Game Trainer: Advanced AI Learning Platform
A cutting-edge platform for training AI agents to master classic video games using Deep Q-Learning.

<p align="center">
<img src="assets/Screenshot 2025-07-10 184134.png" alt="ML Game Trainer Introduction" width="600"/>
</p>

Overview
ML Game Trainer is designed to demonstrate machine learning in action. It provides an interactive environment where AI agents, powered by neural networks, learn to play a variety of classic games autonomously. This platform supports real-time visualization of training progress and offers adjustable controls to monitor the AI's learning process.

Key Features
Multiple Classic Games: Train AI on 7 iconic games: Snake, Pong, Flappy Bird, Tetris, Galaga, Dino Run, and Pac-Man.

Deep Q-Learning (DQN): Utilizes advanced AI algorithms to enable intelligent gameplay.

Real-time Visualization: Observe AI training with live plots and interactive game windows.

Adjustable Game Speed: Control the training speed to analyze learning dynamics.

Model Persistence: Trained models are automatically saved and loaded for continued training and evaluation.

Game Highlights
Snake Game
The AI learns optimal pathfinding to collect food in a classic Snake environment.

<p align="center">
<img src="assets/Screenshot 2025-07-10 104109.png" alt="Snake Game Training Progress" width="700"/>
</p>

Tetris
AI agents learn to stack blocks and clear lines, adapting to changing board layouts.

<p align="center">
<img src="assets/Screenshot 2025-07-10 193327.png" alt="Tetris Game Training Progress" width="700"/>
</p>

Pac-Man
The AI navigates the maze and interacts with ghosts that exhibit different behaviors (aggressive, conditional, and random).

<p align="center">
<img src="assets/Screenshot 2025-07-10 192428.png" alt="Pac-Man Game Training Progress" width="700"/>
</p>

Flappy Bird
Training an AI to navigate the bird through pipes with continuous flight mechanics.

<p align="center">
<img src="assets/Screenshot 2025-07-10 193434.png" alt="Flappy Bird Training Progress" width="700"/>
</p>

Pong
A two-player Pong game where the AI controls one paddle, utilizing an improved reward structure for efficient learning.

<p align="center">
<img src="assets/Screenshot 2025-07-10 001642.png" alt="Pong Game Training Progress" width="700"/>
</p>

Installation
This project requires Python 3.7+ and several libraries.

pip install pygame torch numpy matplotlib tkinter

Usage
Run the application:

python main.py

Select a game from the UI.

Adjust the game speed using the AI Controls window.

Watch the AI train in real-time.

Trained models are saved automatically in the model/ directory.

Architecture
main.py: Entry point for the application and game selection.

ui_windows.py: Manages the Tkinter UI for game controls and selection.

game_runner.py: Coordinates the game loop and AI training process.

agent_core.py: Implements the neural network agent.

game_interface.py: Base class for all game implementations.

utils.py: Contains utility functions for file paths and resources.

Requirements
Python 3.7+

Pygame

PyTorch

NumPy

Matplotlib

Tkinter
