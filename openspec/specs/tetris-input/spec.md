# tetris-input Specification

## Purpose
TBD - created by archiving change tetris-game-completion. Update Purpose after archive.
## Requirements
### Requirement: Keyboard Controls

The system MUST respond to user keyboard input to control the active piece.

#### Scenario: Moving Left/Right
- **WHEN** the Left or Right arrow key is pressed
- **THEN** the piece MUST move 1 unit in that direction, if there is no collision.

#### Scenario: Rotating
- **WHEN** the Up arrow key (or designated rotate key) is pressed
- **THEN** the piece MUST rotate 90 degrees, adjusting position if necessary to avoid collision (basic kick).

#### Scenario: Dropping
- **WHEN** the Down arrow key is pressed
- **THEN** the piece MUST move down 1 unit immediately, resetting the drop counter.

