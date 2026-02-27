# Proposal

## Why
Now that the basic rendering engine is working, we need to implement the core gameplay mechanics for the Tetris game to make it fully playable.

## What Changes
- Add all 7 standard tetromino shapes and colors.
- Implement user input for moving (left/right/down) and rotating (SRS basic rotation) pieces.
- Implement collision detection against the grid boundaries and placed pieces.
- Implement locking pieces into the grid when they hit the bottom.
- Implement clearing full lines and calculating score.
- Add Game Over state and restart functionality.

## Capabilities

### New Capabilities
- `tetris-game-logic`: Complete game state management (piece movement, collision, line clearing).
- `tetris-input`: Keyboard handling for player control.
- `tetris-scoring`: Track score, lines, and levels.

## Impact
- `tetris.html`: Expanding the existing JS to include full game logic.
