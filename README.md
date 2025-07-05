# vehicle_routing
Vehicle Routing Problem Solver with Genetic Algorithms
# Overview
This project provides an advanced solution for the Vehicle Routing Problem (VRP) using Genetic Algorithms. By leveraging the DEAP library for evolutionary computation, the solution optimizes routing for logistics challenges. Initially, the DEAP library was explored through a maze solver before being applied to the VRP, demonstrating the adaptability of the approach.

## Features
**Genetic Algorithms**: Utilizes DEAP for evolutionary computation to find optimal routes.
**Maze Solver Exploration**: Initial experiments with genetic algorithms on maze solving before applying them to VRP.
**Standard Logistics Problem Solving**: Addresses both production and distribution logistics problems.
**Fitness Evaluation**: Implements a custom fitness evaluation function to enhance route efficiency and optimization.
**Visualization**: Uses Matplotlib to visualize routing solutions, aiding in effective data communication and decision-making.
## Installation
To set up the project, follow these instructions:

```
git clone https://github.com/username/repository.git
cd repository
pip install -r requirements.txt
```
### Usage
Run the VRP solver with:
`
python main.py --input data/input_file.json --output results/output_file.json
`
Example Input Data
data/input_file.json

```json

{
  "depot": [0, 0],
  "locations": [[1, 2], [3, 4], ...],
  "demands": [0, 1, 2, ...]
}
```
Example Output Data
results/output_file.json

```json
{
  "routes": [[0, 1, 2, 0], ...]
}
```
### Algorithms
**Genetic Algorithms**: Deployed through the DEAP library, involving crossover, mutation, and selection strategies tailored for routing optimization.
**Fitness Function**: Custom-designed to evaluate route efficiency based on distance, time, and constraints.
### Code Structure
**main.py**: Main entry point for running the solver.
**solver.py**: Contains genetic algorithm implementations and optimization logic.
**fitness.py**: Defines the fitness evaluation function for VRP.
**visualization.py**: Handles visualization of routing solutions with Matplotlib.

### Testing
To ensure the functionality and performance of the solution, run:

`
pytest tests/
`
### Contributing
Interested in contributing? Please refer to CONTRIBUTING.md for guidelines on how to contribute to the project.

#### License
This project is licensed under the MIT License. See LICENSE for details.

### References
DEAP Library: [DEAP Documentation](https://deap.readthedocs.io/en/master/)
Vehicle Routing Problem: [VRP Overview](https://en.wikipedia.org/wiki/Vehicle_routing_problem)
