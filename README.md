# AI_A2_23F-0573-6E_Q6
PATH FINDER FOR INFORMED SEARCHES.

Dynamic Pathfinding Agent
A Tkinter GUI based dynamic pathfinding agent in Python. The agent demonstrates A* and Greedy Best-First Search (GBFS) algorithms with Manhattan and Euclidean heuristics, capable of navigating through static and dynamic obstacles in real-time.
This project is ideal for learning AI search strategies, heuristics, and adaptive pathfinding visualization.
Features
•	Interactive grid with start and goal points
•	Manual wall placement or random maze generation
•	Dynamic obstacles during path execution
•	Real-time path animation
•	Metrics: Nodes Visited, Path Cost, Execution Time
•	Choice of Algorithm: A* or GBFS
•	Choice of Heuristic: Manhattan or Euclidean
Algorithms Implemented
 A* Search
•	Uses f = g + h (path cost + heuristic)
•	Guarantees optimal path with admissible heuristics
•	Works best with Manhattan in 4-directional grids
•	Slight differences appear with Euclidean heuristic due to diagonal distance calculations
 Greedy Best-First Search (GBFS)
•	Uses only heuristic (h) to guide search
•	Faster in simple grids but may not guarantee optimal paths in complex mazes
•	Dynamic obstacles may force recalculations and suboptimal paths
 Heuristics
Heuristic	Formula	Best For
Manhattan	|dx| + |dy|	4-directional grids
Euclidean	√(dx² + dy²)	Continuous movement

 Controls
Action	Method
Place walls	Left-click & drag
Erase walls	Right-click & drag
Set Start	Select "Start" mode → Click
Set Goal	Select "Goal" mode → Click
Find Path	Click "Find Path" or press Space
Random Maze	Click "Random Maze" or press M
Clear Walls	Click "Clear Walls" or press C
Reset Grid	Click "Reset" or press R
New Seed	Click "New Seed"
Fullscreen	Press F11

 Metrics Display
•	Nodes Visited – Total expanded nodes
•	Path Cost – Length of final path
•	Execution Time – Time taken in milliseconds
•	Status – Current state (Searching, Path Found, etc.)
 Color Legend
Element	Color	Meaning
Start	 Green	Source 'S'
Goal	 Red	Destination 'G'
Wall	 Dark Gray	Obstacle
Frontier	 Yellow	In queue
Visited	 Light Blue	Explored
Path	 Bright Green	Solution
Agent	 Pink	Current position

 Notes
•	4-directional movement only (up, down, left, right)
•	Each move costs exactly 1.0
•	Dynamic obstacles spawn with 15% probability during agent movement
•	Replanning happens automatically if path is blocked

