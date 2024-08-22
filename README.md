# Robot Path Planning Simulation

## Description

This project implements a robot path planning simulation using CoppeliaSim (V-REP) software. It demonstrates the use of Dijkstra's algorithm and Breadth-First Search (BFS) for path planning, along with obstacle avoidance capabilities. The simulation features an interactive UI for controlling the robot and setting parameters.

## Features

- Path planning using Dijkstra's algorithm and BFS
- Interactive obstacle generation
- Real-time obstacle avoidance
- Customizable start and end points
- Visualized path drawing
- Adjustable robot speed and sensor parameters

## Requirements

- CoppeliaSim (V-REP) software
- Python 3.x
- NumPy library

## Installation

1. Clone this repository to your local machine.
2. Ensure you have CoppeliaSim installed.
3. Install the required Python libraries:

## Usage

1. Open the CoppeliaSim scene file (not provided in the code snippet).
2. Run the simulation in CoppeliaSim.
3. Use the interactive UI to:

- Set the obstacle percentage
- Define start and end points
- Choose between Dijkstra's algorithm and BFS
- Initiate the path planning and robot movement

## Code Structure

- `sysCall_init()`: Initializes the simulation, sets up the environment, and creates the UI.
- `_graph()`: Defines the Graph class for creating and managing the navigation graph.
- `run_dijkstra()` and `run_bfs()`: Implement Dijkstra's algorithm and BFS respectively.
- `move_towards_path()`: Controls the robot's movement along the planned path.
- `avoid_obstacle()`: Implements the obstacle avoidance algorithm.
- Various UI callback functions for handling user interactions.

## Key Components

1. **Graph Generation**: Creates a graph representation of the environment, including randomly generated obstacles.
2. **Path Planning Algorithms**:

- Dijkstra's algorithm for finding the shortest path
- BFS for exploring all possible paths

3. **Robot Control**: Functions to move the robot along the planned path and avoid obstacles.
4. **Sensor Integration**: Uses proximity sensors for obstacle detection.
5. **Visualization**: Draws the robot's path and highlights obstacles in the simulation.

## Customization

You can modify various parameters in the code to adjust the simulation:

- `x_scale` and `y_scale`: Change the size of the simulation area
- `velocity`: Adjust the robot's movement speed
- `node_radius`: Modify the size of path nodes
- `random_percent`: Change the density of randomly generated obstacles

## Contributing

Contributions to improve the simulation or add new features are welcome. Please feel free to fork the repository and submit pull requests.

## License

[This Project is Open Sourced]

## Acknowledgments

- CoppeliaSim (V-REP) for providing the simulation environment
- Contributors and maintainers of the NumPy library
