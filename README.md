# autonomous-delivery-agent
Delivery Agent Simulation
Multi-search algorithm pathfinding simulation using Pygame visualization. This project demonstrates a range of AI search algorithms for package delivery in different terrain environments.

Features
????️ Map Types
Small Map (5x5): Simple grid with basic obstacles

Medium Map (10x10): Advanced terrain patterns and obstacles

Large Map (15x15): Advanced maze-like layout

Dynamic Map: Moving obstacles that change locations

???? Search Algorithms
BFS (Breadth-First Search): Shortest path in terms of steps

UCS (Uniform Cost Search): Minimum-cost path

A* (A-Star Search): Most efficient with heuristic guidance

Replan: Adaptive algorithm for dynamic environment

???? Visualization
Real-time path animation

Color-coded terrain types

Dynamic obstacle movement

Cost display on each cell

Step-by-step execution tracking

Installation
Prerequisites
Python 3.7+

Pygame library

Usage
Running the Simulation
Run the main script

Select option 1 for PyGame visualization

Select map type (1-4):

1: Small map

2: Medium map

3: Large map

4: Dynamic map

Select algorithm (1-4):

1: BFS

2: UCS

3: A*

4: Replan

Controls During Animation
ESC: Quit simulation

Close Window: Quit application

Animation runs automatically with configurable delays

Algorithm Comparison
BFS (Breadth-First Search)
Pros: Guarantees shortest path by steps

Cons: Does not consider terrain cost

Best for: Grids without cost considerations

UCS (Uniform Cost Search)
Pros: Finds lowest-cost path

Cons: Slower than BFS

Best for: Cost-sensitive applications

A* (A-Star Search)
Pros: Most efficient, searches cost + heuristic

Cons: Requires admissible heuristic

Best for: Most practical applications

Replan (Hill Climbing)
Pros: Resilient to changing environment

Cons: Can fail to find optimum solution

Best for: Dynamic obstacle scenarios

DeliveryAgent/
├── Grid Class          # In charge of terrain and obstacles
├── Cell Class          # Attributes of grid cell
├── DeliveryAgent Class # Handling search algorithms
├── PygameVisualizer    # Visualization tool
└── Map Creators        # Pre-defined map schemes

Key Classes
Grid: Game world with terrain and obstacles responsibility

set_terrain(): Set cell terrain type

set_obstacle(): Add permanent/dynamic obstacles

update_dynamic_obstacles(): Dynamic obstacle update

DeliveryAgent: Pathfinding algorithm implementation

bfs(): Breadth-first search implementation

uniform_cost_search(): Cost-based search algorithm implementation

a_star_search(): Heuristic search implementation

hill_climbing_replan(): Adaptive search algorithm implementation

PygameVisualizer: Handling graphics and animation

draw_grid(): Draw the game world

animate_path(): Animate agent movement

Future Enhancements
Future development potential:

Multiple agents with interactions

More search algorithms (IDA, D Lite)

Improved dynamic obstacle processing

Performance benchmarking suite

Save/load map configurations

License
This is a learning project. Feel free to edit and expand for learning AI pathfinding concepts.

Contributing
Suggestions and enhancements welcome! Areas of focus:

Algorithm efficiency

Visualization improvements

Other map types

Performance optimisation

