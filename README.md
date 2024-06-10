# Game-Playing---Adversarial-Search
Python implementation of Adversarial Search for Tic-Tac-Toe, using MiniMax and Alpha Beta Pruning.

## Introduction

This repository contains implementations and experiments with various AI techniques for game playing and optimization. The focus is on two primary tasks:

1. **Tic-Tac-Toe with Minimax and Alpha-Beta Pruning**:
   - Implementing the Minimax algorithm for optimal move selection in Tic-Tac-Toe.
   - Enhancing the Minimax algorithm using Alpha-Beta Pruning for efficiency.
   - Developing parallelized and heuristic-based versions of Alpha-Beta Pruning.
   - Creating a modified Tic-Tac-Toe game with a "weak" AI player featuring randomized decision-making.

## Question 1: Tic-Tac-Toe with Minimax and Alpha-Beta Pruning

### Implementation Overview

The goal was to implement the Minimax algorithm for Tic-Tac-Toe and enhance it using Alpha-Beta Pruning. Additional explorations included parallelization and heuristic-based optimizations. A modified version of Tic-Tac-Toe with a "weak" AI player was also created.

### Implementation Details

1. **Minimax Algorithm**: The Minimax algorithm finds the optimal move by evaluating all possible moves recursively.

2. **Alpha-Beta Pruning**: Alpha-Beta Pruning was integrated to reduce the search space by discarding subgraphs that do not lead to an optimal move. This optimization significantly decreased the number of nodes evaluated during the search process.

3. **Parallelized Alpha-Beta Pruning**: A parallelized version of Alpha-Beta Pruning was implemented using two threads, dividing the search space into maximizing and minimizing subtrees. This parallelization aimed to improve the algorithm's performance by leveraging multi-threading capabilities.

4. **Enhanced Heuristic**: An enhanced heuristic was developed to prioritize more promising branches of the search tree during non-terminal state evaluation. This heuristic-based approach further reduced the search space by guiding the selection of moves and pruning less desirable branches.

5. **Modified Tic-Tac-Toe Gameplay**: A modified version of Tic-Tac-Toe was created where the AI player followed randomized decision-making, avoiding both the best and worst decisions. A heuristic was incorporated to assess the desirability of game states, enhancing the AI's gameplay experience.

### Results and Evaluation

1. **Minimax Algorithm Evaluation**: The average number of nodes evaluated without Alpha-Beta Pruning was compared to that with Alpha-Beta Pruning over three runs. The results demonstrated a significant reduction in node evaluations with Alpha-Beta Pruning, showcasing its effectiveness in optimizing the search process.
   
2. **Parallelized Alpha-Beta Pruning**: A comparison between the parallelized and sequential versions of Alpha-Beta Pruning was conducted based on node evaluations and time taken. The parallelized version exhibited improved performance, showcasing the benefits of multi-threading in optimizing search algorithms.
   
3. **Enhanced Alpha-Beta Pruning**: The enhanced Alpha-Beta Pruning with the heuristic-based approach showcased further reduction in node evaluations compared to standard Alpha-Beta Pruning. This highlighted the efficacy of incorporating heuristics in guiding search decisions.
   
4. **Modified Tic-Tac-Toe Gameplay**: The modified Tic-Tac-Toe game with a "weak" AI player demonstrated randomized decision-making and heuristic-based desirability assessment. This approach introduced variability and strategic depth to the gameplay, enhancing the player experience.

### References

1. [GeeksforGeeks - Finding Optimal Move in Tic-Tac-Toe using Minimax Algorithm in Game Theory](https://www.geeksforgeeks.org/finding-optimal-move-in-tic-tac-toe-using-minimax-algorithm-in-game-theory/)
2. Research Papers on Alpha-Beta Pruning and Heuristic Optimization in Game Playing AI.

## Contributions

- Ahmed Kamal :)
