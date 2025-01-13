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

numpy
matplotlib
Install them using:

bash
Copia codice
pip install numpy matplotlib
How to Run
Prepare the simulation input data in the input_data dictionary.
Run the script to generate a real-time visualization of the simulation.
Modify input_data or the code to customize the environment and parameters.
Key Input Data
Configuration
Room dimensions: Set the width and height of the room.
Background and wall colors: Define RGB values for the environment's appearance.
Heatmap: Enable or disable heatmap visualization.
Actors
Position: Initial coordinates of each actor.
Velocity: Initial velocity vector.
Radius: Size of the actor (used for collision detection).
Color: RGB color for visual representation.
Walls and Door
Walls: List of wall coordinates defining the room's boundaries.
Door: Location and size of the exit.
Example Input Data
A basic setup is already included in the script under input_data:

python
Copia codice
"config": {
    "width": 200.5,
    "height": 200.5,
    "scale": 10,
    "delay": 0,
    "bgColor": [0, 0, 0],
    "wallColor": [255, 255, 255],
    "heatmapEnabled": True
},
"room": {
    "walls": [
        [0.5, 0.5, 200, 0.5],
        [200, 0.5, 200, 200],
        ...
    ]
},
"actors": [
    {
        "pos": [50, 100],
        "velocity": [1.5, 1.5],
        "desiredSpeed": 1,
        "radius": 0.25,
        ...
    },
    ...
],
"door": {
    "x": 100,
    "y": 200,
    "width": 4
}
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
This project is inspired by the seminal work on escape panic dynamics:

Dirk Helbing, Illés Farkas, and Tamás Vicsek, Nature (2000).
