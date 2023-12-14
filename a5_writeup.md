# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

I think Depth-First Search is faster than Breadth-First Search because DFS solved the puzzles in less iterations. 337 for DFS vs 556 for BFS on the harder board. They were equally efficient in the easier board. DFS may run into a dead end while BFS is more likely to find the solution.

2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?


DFS explores deeper levels, while BFS finds the quickest path possible to get to the answer. Maybe for an alternative you could try to use lists. It definitely wouldn't be as efficient as DFS or BFS but I think that you could use lists to get to the answer at some point.

3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

You can use these ways of searching for many different puzzle games. I think BFS would be more efficient for ones that are not complicated, and have a straight path to the answer. I think MineSweeper is a good example of a game that BFS would be efficient at. DFS would be better for puzzle games that can have many different ways of getting to the final answer.


