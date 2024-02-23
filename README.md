# Yashi-Game

__SAT-based__ approach for solving the __Yashi Game__. Final project for the _Knowledge Representation and Learning_ course at _UniPd_.

## Game Rules:

An instance of the Yashi game is specified by a n x n integer grid, on which p nodes are placed.  
A solution of the game consists in drawing horizontal and vertical segments, satisfying the following conditions:
- No two segments cross each other
- The segments form a tree (they form a graph without cycles)

## Solutions:

Given an instance of the Yashi Game, some constraints are defined in order to determine if a solution exists. The [PySAT](https://pysathq.github.io/) library was used to define the formulas and to access the solvers.  
A __SAT solver__ (_Minisat22_) was used to identify a solution for the game, a __MaxSAT solver__ (_based on the Fu&Malik MaxSAT algorithm_) was used to find the __minimum-length solution__.  

.

![Plots of a Yashi Game solution](https://github.com/federicochiarello/Yashi-Game/blob/master/img/yashi_solutions.png)
