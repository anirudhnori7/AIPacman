In this project, the Pacman agent will find paths through his maze world, both to reach a particular location and to collect food efficiently.

1) Finding a Fixed Food Dot using Depth First Search
Use following commands to test:
python pacman.py -l tinyMaze -p SearchAgent
python pacman.py -l mediumMaze -p SearchAgent
python pacman.py -l bigMaze -z .5 -p SearchAgent


2)Breadth First Search
Use following commands to test:
python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs
python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5

3)Varying the Cost Function
Use following commands to test:
python pacman.py -l mediumMaze -p SearchAgent -a fn=ucs
python pacman.py -l mediumDottedMaze -p StayEastSearchAgent
python pacman.py -l mediumScaryMaze -p StayWestSearchAgent

4)A* search
Use following commands to test:
python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic

5)Finding All the Corners
Use following commands to test:
python pacman.py -l tinyCorners -p SearchAgent -a fn=bfs,prob=CornersProblem
python pacman.py -l mediumCorners -p SearchAgent -a fn=bfs,prob=CornersProblem

6)Corners Problem: Heuristic
Use following commands to test:
python pacman.py -l mediumCorners -p AStarCornersAgent -z 0.5
-p SearchAgent -a fn=aStarSearch,prob=CornersProblem,heuristic=cornersHeuristic

7)Eating All The Dots
python pacman.py -l testSearch -p AStarFoodSearchAgent

8)Suboptimal Search
python pacman.py -l bigSearch -p ClosestDotSearchAgent -z .5 

