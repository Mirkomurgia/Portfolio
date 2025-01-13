Escape Panic Simulation

This project is a simulation based on the paper "Simulating dynamical features of escape panic" by Dirk Helbing, Illés Farkas, and Tamás Vicsek. It models a scenario where multiple agents (actors) navigate through a room to exit via a door under specific physical and behavioral constraints.

Features

Agent Interaction: Simulates physical and social forces between agents.
Wall Interaction: Models interactions between agents and obstacles (walls).
Dynamic Goal Setting: Agents are directed towards an exit (door) while avoiding collisions.
Visualization: Displays the simulation in real-time using matplotlib.
Configurable Environment: Customizable room dimensions, agent properties, and simulation parameters.
Prerequisites
To run the simulation, ensure the following Python libraries are installed:

Simulation Process

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
