# Tasks

## 1. Core Logic and State

- [x] 1.1 Define constants for colors and matrices for all 7 standard pieces (I, J, L, O, S, T, Z).
- [x] 1.2 Implement `collide(grid, piece)` function to check bounds and existing blocks.
- [x] 1.3 Implement `merge(grid, piece)` to copy piece data into the main grid.
- [x] 1.4 Implement `playerReset()` to generate a new random piece and handle Game Over.
- [x] 1.5 Implement `gridSweep()` to find, clear filled lines, and update score.

## 2. Movement and Input

- [x] 2.1 Implement `playerDrop()` to move the piece down manually and handle locking/resetting.
- [x] 2.2 Implement `playerMove(offset)` to move horizontally with collision checks.
- [x] 2.3 Implement `rotate(matrix, dir)` for piece rotation.
- [x] 2.4 Implement `playerRotate(dir)` with basic wall kick logic.
- [x] 2.5 Add `document.addEventListener('keydown')` for arrow keys/WASD.

## 3. UI and Polish

- [x] 3.1 Add HTML/CSS for a score display element.
- [x] 3.2 Implement `updateScore()` to refresh the UI text.
- [x] 3.3 Update the main `update()` loop to integrate score and new piece logic.
