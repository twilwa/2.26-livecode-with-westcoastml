# Design

## Context
Building on top of the initial canvas renderer, we are adding the core Tetris game rules within the single `tetris.html` file.

## Goals / Non-Goals

**Goals:**
- Implement all 7 standard tetrominoes (I, J, L, O, S, T, Z).
- Provide basic keyboard controls (Arrows/WASD) for movement and rotation.
- Manage grid state (merging pieces, clearing lines).
- Display a simple score.

**Non-Goals:**
- Complex SRS kicks (wall kicks) are out of scope for this basic iteration to keep logic simple, basic rotation will suffice.
- Advanced features like "Hold" piece or "Ghost" piece are deferred for later to keep the scope tight, although standard UI elements can be added if time permits. Let's focus on a working base game first.

## Decisions

### Decision 1: Matrix Representation
- The board is a 2D array of integers. 0 represents empty, non-zero represents colors/types.
- Pieces will be generated from predefined 2D matrices.

### Decision 2: Collision Detection
- A generalized `collide(grid, piece)` function will check if the piece's matrix overlaps with any non-zero elements in the grid or exceeds boundaries.

### Decision 3: Game Loop and Timing
- Continue using `requestAnimationFrame`. We will introduce a drop interval that decreases as the score/level increases.
