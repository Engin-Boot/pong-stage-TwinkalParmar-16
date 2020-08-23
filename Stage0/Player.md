# Player
  Contains functionalities or activities which a player can perform.
  This will also inherit the style module.
  
## Feature

### Variables
- name
- score
- is_my_turn
- am_i_a_winner
- if_missed

### Methods

#### Abstract Methods
- missed()
- notMissed()
- moveUp()
- mobeDown()

## Acceptance Criteria

### Scenario: player hits the ball
- Given: Bar hits the ball. 
- When: Player1/player2 turn .
- Then: Chnage the direction of the ball : is_my_turn=!is_my_turn.

### Scenario: player does not hit the ball
- Given: Bar missed the ball. 
- When: player1/player2 turn.
- Then: update the score of opponent player : score =score+1.

### Scenario: up movement
- Given: Player wants to move bar in uppward direction. 
- When: Press 'up'(player1) key or 'w' key(player2).
- Then: Move bar in upward direction.

### Scenario: down movement
- Given: Player wants to move bar in downward direction. 
- When: Press 'down'(player1) key or 's' key(player2).
- Then: Move bar in downward direction.

