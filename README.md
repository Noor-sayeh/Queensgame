# N-Queens Solver GUI with Hill Climbing and Simulated Annealing

This project is a **Java Swing-based application** that visually demonstrates solutions to the **N-Queens problem** using two optimization algorithms: **Hill Climbing** and **Simulated Annealing**. Users can create chessboards of various sizes (4x4 to 8x8) and observe how queens are placed on the board to satisfy the N-Queens constraints.

---

## Features

1. **Interactive Chessboard Creation**:  
   Users can select a board size from the dropdown and generate a corresponding chessboard.

2. **Visualization of Algorithms**:  
   - **Hill Climbing**: Iteratively improves the queen positions until a solution is found or a local maximum is reached.  
   - **Simulated Annealing**: Uses probabilistic decision-making to escape local maxima and search for a global solution.

3. **Real-time Updates**:  
   The GUI dynamically updates the board as queens are placed during algorithm execution.

4. **Error Handling**:  
   Prompts users with appropriate messages if actions are performed incorrectly, such as running algorithms without creating a board.

---

## Code Overview

### Main Components

1. **Settings Panel**:  
   Includes options for board size selection, and buttons for board creation and algorithm execution.

2. **Chessboard Panel**:  
   Displays a visual representation of the chessboard with queens placed.

3. **Algorithms**:
   - **Hill Climbing**:
     - Tries to minimize the heuristic function by moving queens to better positions.
     - Includes random restarts to escape local maxima.
   - **Simulated Annealing**:
     - Probabilistically accepts worse states to explore the solution space and avoid local maxima.

4. **Utility Functions**:
   - `calHeuristic(int[] queens)`: Calculates the heuristic value based on queen conflicts.
   - `generateRandomQueens()`: Generates a random queen placement for restarts.
   - `nxtstat(int[] queens)`: Generates a random neighboring state for simulated annealing.

