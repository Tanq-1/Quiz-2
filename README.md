# Master Gate Maze

Master Gate Maze is a browser-based maze game where the player navigates a grid, collects colored keys, and unlocks the master gate to reach the exit. Each maze is randomly generated, providing a unique maze every time they generate a new one.

## How to run

- Download the index.html file
  
  <img width="2557" height="1301" alt="image" src="https://github.com/user-attachments/assets/82f1bf95-e8fe-4639-9a0d-90d1a72c0163" />

- Right click on the file and choose "Open with"
  
  <img width="400" height="324" alt="image" src="https://github.com/user-attachments/assets/773569ec-0457-4858-a721-e050bbe36d2a" />

- Choose a browser you want to open the file with
  
  <img width="473" height="536" alt="image" src="https://github.com/user-attachments/assets/31bdc00a-9406-49ad-9dff-4e504fac7b11" />

- The game should appear like so
  
  <img width="940" height="752" alt="image" src="https://github.com/user-attachments/assets/bdb5d946-4d9c-4bbb-8908-dc851eb45b2b" />

## Game Objective

The main goal of the game is to move your player (white circle) from the starting position to the exit, while collecting all the colored keys if any are present. The exit is blocked by the master gate (gold double-square ▣) until all keys are collected. If no keys are generated, the master gate is not present and the exit is accessible immediately.

## How to Play

- Use the **arrow keys** or **WASD** keys to move your player up, down, left, or right.
- Move onto a cell containing a colored key to collect it. Collected keys are tracked in the HUD and marked with a ✅.
- The master gate unlocks (turns into the exit) once all keys are collected or if there are no keys.
- Step onto the exit cell to complete the maze.

## Controls

- **Arrow keys / W, A, S, D**: Move the player
- **Generate Maze**: Randomly generate a new maze with the selected number of keys
- **Toggle Path Overlay**: Display the shortest solution path, including the order to collect keys and their locations
- **Reset Player**: Reset the player position and collected keys without generating a new maze

## Game Interface

### Left Panel

- **Grid**: 20 × 20 maze displayed on the canvas
- **Controls**: Buttons for maze generation, path overlay toggle, and resetting the player
- **Key Selector**: Choose the number of keys to appear in the maze (0–11)
- **Legend**: Shows all key colors with corresponding dots

### Right Panel

- **Status**: Displays keys collected, number of moves, player position, and exit position
- **Solution (Solver Output)**: Shows the optimal key collection order and path if the path overlay is enabled
- **Notes**: Provides guidance on gameplay mechanics

## Extra Information

- **Master Gate**: Blocks the exit until all keys are collected. Represented as a gold double-square ▣.
- **Keys**: Randomly placed colored keys that must be collected to open the master gate. Each color corresponds to a unique key.
- **Exit Flashing**: The exit cell flashes with multiple colors for visual feedback.
- **Path Overlay**: Highlights the shortest route to complete the maze based on current player position and collected keys.

## Strategy Tips

- Just have fun and try solving the maze without using the help of the solver

## Technical Details

- The maze is generated using a **Depth-First Search (DFS)** algorithm to create randomized paths with optional cycles.
- The shortest path solution is calculated using **Breadth-First Search (BFS)** to ensure optimal key collection and exit access.

## Browser Requirements

- Modern browser (Chrome, Firefox, Edge, or Safari)
- JavaScript enabled
