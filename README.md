ML Game Trainer: Advanced AI Learning Platform
A cutting-edge platform for training AI agents to master classic video games using Deep Q-Learning.

<p align="center">

</p>

<p align="center">
<a href="https://www.python.org" target="_blank">

</a>
<a href="https://pytorch.org/" target="_blank">

</a>
<a href="https://www.pygame.org/" target="_blank">
<img src="https://img.shields.io/badge/Pygame-FFD133?style=for-the-badge&logo=pygame&logoColor=white" alt="Pygame">
</a>
<a href="https://numpy.org/" target="_blank">
<img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy">
</a>
<a href="https://matplotlib.org/" target="_blank">
<img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white" alt="Matplotlib">
</a>
<a href="https://docs.python.org/3/library/tkinter.html" target="_blank">
<img src="https://img.shields.io/badge/Tkinter-4285F4?style=for-the-badge&logo=python&logoColor=white" alt="Tkinter">
</a>
</p>

Overview
ML Game Trainer is designed to demonstrate machine learning in action. It provides an interactive environment where AI agents, powered by neural networks, learn to play a variety of classic games autonomously. This platform supports real-time visualization of training progress and offers adjustable controls to monitor the AI's learning process, making complex AI concepts tangible and engaging.

Key Features
Multiple Classic Games: Train AI on 7 iconic games: Snake, Pong, Flappy Bird, Tetris, Galaga, Dino Run, and Pac-Man.

Deep Q-Learning (DQN): Utilizes advanced AI algorithms with both Convolutional Neural Networks (CNN) for image-based games and Linear networks for vector-based games to enable intelligent gameplay.

Real-time Visualization: Observe AI training with live plots of scores and records, alongside interactive game windows.

Adjustable Game Speed: Control the training speed (FPS) to analyze learning dynamics or speed up training.

Model Persistence: Trained models are automatically saved to the model/ directory and can be loaded for continued training or evaluation.

Game Highlights
Each game provides a unique challenge for the AI, showcasing different aspects of reinforcement learning.

Snake Game
The AI learns optimal pathfinding to collect food, demonstrating efficient navigation and strategic decision-making in a classic Snake environment.

<p align="center">

</p>

Tetris
AI agents learn to stack blocks and clear lines, adapting to changing board layouts and predicting future states for optimal placement.

<p align="center">
<img src="assets/Screenshot 2025-07-10 193327.png" alt="Tetris Game Training Progress" width="700"/>
</p>

Pac-Man
The AI navigates the maze, strategically collecting dots while interacting with three distinct ghost behaviors (aggressive, conditional, and random), and leveraging power pellets.

<p align="center">
<img src="assets/Screenshot 2025-07-10 192428.png" alt="Pac-Man Game Training Progress" width="700"/>
</p>

Flappy Bird
Training an AI to navigate the bird through an endless series of pipes, mastering continuous flight mechanics and timing.

<p align="center">
<img src="assets/Screenshot 2025-07-10 193434.png" alt="Flappy Bird Training Progress" width="700"/>
</p>

Pong
A two-player Pong game where the AI controls one paddle, utilizing an improved reward structure and state representation for efficient learning and competitive play.

<p align="center">
<img src="assets/Screenshot 2025-07-10 001642.png" alt="Pong Game Training Progress" width="700"/>
</p>

Installation
This project requires Python 3.7+ and several essential machine learning and game development libraries.

pip install pygame torch numpy matplotlib tkinter

Usage
Run the application:

python main.py

Select a game from the intuitive Tkinter UI.

Adjust the game speed (FPS) using the AI Controls window to observe the training at your preferred pace.

Watch the AI train in real-time, with live score updates and training progress plots.

Trained models are automatically saved to the model/ directory, allowing you to resume training or evaluate performance at any time.

Architecture
The platform's modular design ensures scalability and ease of understanding:

main.py: The primary application entry point, handling game selection and overall flow.

ui_windows.py: Manages the Tkinter UI for game selection, speed controls, and visualization toggles.

game_runner.py: Orchestrates the game loop, coordinates AI training, and manages real-time data flow.

agent_core.py: Implements the core Deep Q-Learning agent, including neural network definitions (linear and CNN) and training logic.

game_interface.py: Provides a base class and interface that all individual game implementations adhere to, ensuring consistency.

utils.py: Contains various utility functions, including resource path management and other helper methods.

Model Files
Trained models are persistently stored for future use, following a clear naming convention:
model/model_[GameName]_[linear/cnn].pth

Requirements
Python 3.7+

Pygame

PyTorch

NumPy

Matplotlib

Tkinter

Future Enhancements and Usage
This platform serves as a robust foundation for further exploration and development in reinforcement learning:

Advanced RL Algorithms: Integrate and experiment with more sophisticated reinforcement learning algorithms such as Proximal Policy Optimization (PPO), Advantage Actor-Critic (A2C), or Rainbow DQN.

New Game Environments: Expand the library of classic games or even integrate custom, more complex environments to challenge AI agents further.

Multi-Agent Learning: Implement scenarios where multiple AI agents interact within the same game, fostering collaborative or competitive learning.

Web-Based Interface: Develop a web-based front-end for the platform to make it more accessible and shareable, allowing users to train and observe AI agents directly in their browser.

Educational Tool: Utilize the platform as an interactive educational resource for teaching reinforcement learning, deep learning, and AI concepts to students and enthusiasts.

Research Platform: Serve as a flexible testbed for researchers to prototype new neural network architectures, experiment with hyperparameter tuning, and analyze AI learning dynamics in controlled environments.

Performance Benchmarking: Implement tools for comprehensive performance benchmarking of different AI models across various games.
