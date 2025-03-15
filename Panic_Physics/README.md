# Escape Panic Simulation

This project simulates escape panic dynamics, inspired by the paper *"Simulating dynamical features of escape panic"* by Dirk Helbing, Illés Farkas, and Tamás Vicsek. The simulation models multiple agents (actors) navigating through a room to exit via a door, considering physical and social interactions.

## Features

- **Agent Interaction**: Models physical and social forces between agents.
- **Wall Interaction**: Simulates interactions between agents and obstacles (walls).
- **Dynamic Goal Setting**: Guides agents towards the exit while avoiding collisions.
- **Visualization**: Displays real-time simulations using `matplotlib`.
- **Customizable Environment**: Adjustable room size, agent properties, and simulation parameters.


## Simulation Process

Environment Initialization:
The room, walls, door, and agents are created based on the input data.
Agent Updates:
Each agent computes forces from nearby agents, walls, and its goal.
The position and velocity are updated iteratively.
Goal Check:
Agents reaching the door are removed from the simulation.
Visualization:
The room, walls, and agents are plotted dynamically.
Results
The simulation outputs:

A real-time animation of the escape process.
Timing data for each agent reaching the goal.
Acknowledgments

This project is inspired by the work on escape panic dynamics:

Dirk Helbing, Illés Farkas, and Tamás Vicsek, Nature (2000).
