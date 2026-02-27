# tetris-game-logic

## ADDED Requirements

### Requirement: Tetromino Generation

The system MUST generate one of the 7 standard tetrominoes randomly when a new piece is needed.

#### Scenario: Spawning a piece
- **WHEN** the game starts or a piece locks into the grid
- **THEN** a new random piece MUST be placed at the top-center of the grid.

### Requirement: Collision Detection

The system MUST prevent pieces from moving through the walls, floor, or other locked pieces.

#### Scenario: Hitting the bottom
- **WHEN** a piece moves down and collides with the floor or a locked piece
- **THEN** the piece MUST lock into the grid and a new piece MUST spawn.

### Requirement: Line Clearing

The system MUST clear fully occupied rows.

#### Scenario: Clearing a line
- **WHEN** a row is completely filled with blocks
- **THEN** that row MUST be removed
- **AND** all rows above it MUST shift down by one.
- **AND** the score MUST increase.

### Requirement: Game Over

The system MUST end the game if a new piece cannot spawn without colliding.

#### Scenario: Stack reaches top
- **WHEN** a newly spawned piece immediately collides
- **THEN** the game MUST reset the grid and score.
