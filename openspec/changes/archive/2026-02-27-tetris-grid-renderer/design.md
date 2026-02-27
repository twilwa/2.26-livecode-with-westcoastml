# Design

## Context
We are starting to build a browser-based Tetris game. The first step is to establish the rendering foundation.

## Goals / Non-Goals

**Goals:**
- Render a 10x20 grid using HTML5 Canvas.
- Render a single active tetromino.
- Keep all code in a single HTML file for simplicity.

**Non-Goals:**
- Implementing game logic (e.g., collision detection, line clearing) is out of scope for this change.
- Handling user input is out of scope for this change.

## Decisions

### Decision 1: HTML5 Canvas API
We will use the vanilla Canvas API for rendering because it provides direct, performant pixel manipulation and is well-suited for grid-based games like Tetris without needing external libraries.

### Decision 2: Single File Structure
For this initial iteration, we will combine HTML, CSS, and JavaScript in `tetris.html` to minimize cognitive load and setup time.

### Decision 3: Data Structures
- The grid will be represented as a 2D array (10 columns, 20 rows).
- The active piece will be an object containing its coordinates (`x`, `y`) and its shape (a 2D array).
