# Exceptional Events
  Contains the events, which occurs during the execution of a program/game, that disrupts the normal flow of the game/program.
  Also inherits the Player module.
  

## Feature

### Functions
- close()
- quit()
- reset()

## Acceptance Criteria

### Scenario: close the game
- Given: Game is running. 
- When: Click close button.
- Then: Store the current state of the program and exit the game.

### Scenario: quit the game
- Given: Game is running. 
- When: Click quit button.
- Then: Reset the scores and exit the game.

### Scenario: reset the game
- Given: Game is running. 
- When: Click reset button.
- Then: Set the scores of both the player to zero and restart the game.

