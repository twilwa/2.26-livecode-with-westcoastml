# tetris-rendering Specification

## Purpose
TBD - created by archiving change tetris-grid-renderer. Update Purpose after archive.
## Requirements
### Requirement: Render Grid and Active Piece

The system MUST render a standard 10x20 Tetris grid and one active, falling tetromino.

#### Scenario: Rendering the initial game state

- **WHEN** the game starts
- **THEN** an empty 10x20 grid should be drawn on the canvas
- **AND** a single tetromino (e.g., T-piece) should be drawn at the top-center of the grid.

