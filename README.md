# Maze Solver using Python `curses`

This project is a simple **maze solver visualization** built in Python using the `curses` library. It demonstrates **Breadth-First Search (BFS)** for finding the shortest path through a maze.

---

## Features

* Uses **Breadth-First Search (BFS)** to guarantee the shortest path.
* Maze is displayed in the terminal with **curses**.
* Real-time visualization of the pathfinding process.
* Path is marked with **red `X`** while walls and empty spaces are shown in **blue**.

---

##  Maze Representation

* The maze is represented as a **2D list** of characters:

  * `#` → Wall
  * `O` → Start position
  * `X` → End position
  * `E` → Extra marker (not used in solving)
  * Spaces (` `) → Walkable path

Example:

```python
maze = [
    ['#','O','#','#','#','#','#','#','#','#','#','#','#','#','#'],
    ['#','S',' ','#',' ',' ',' ','#',' ',' ',' ',' ','#',' ','#'],
    ...
]
```

---

## How It Works

1. **Find Start Position**: Locate the starting cell `O`.
2. **Breadth-First Search (BFS)**:

   * Explore all neighbors (up, down, left, right).
   * Skip already visited positions and walls `#`.
   * Keep track of the path taken.
3. **Visualization**:

   * Maze is redrawn each iteration.
   * Current path is shown in **red**.
4. **End Condition**: Stops when the end `X` is reached.

---

## Visualization

* **Blue (`#`, spaces, O, X)** → Maze layout
* **Red (`X`)** → Current BFS path under exploration

---

##  Running the Project

### Prerequisites

* Python 3.x
* curses
---

## Example Output (Terminal Visualization)

```
# O # # # # # # # # # # # # #
# S   #       #             #
... (maze updates as BFS runs)
```

The path will be dynamically highlighted in **red** as BFS explores.

---

## Future Improvements

* Add support for **DFS / A* Algorithm*\*.
* Allow **user input mazes** instead of fixed.
* Display **final path separately** after solving.

---

##  License

This project is open-source under the MIT License. Feel free to modify and improve it!
