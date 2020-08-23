# Toggle
  Contains the events, when control transfer from one player to another one.
  Also this modules inherits the player module.

## Feature

### Functions
- updateScore()
- changeTheDirection()
- checkWinner()
- transferControl()

## Acceptance Criteria

### Scenario: update the score
- Given: Player1's turn. 
- When: Bar does not hit the ball.
- Then: Player2.score=Player2.score+1.

### Scenario: update the score
- Given: Player2's turn. 
- When: Bar does not hit the ball.
- Then: Player1.score=Player1.score+1.

### Scenario: change in the direction of bal
- Given: Player1/player's turn. 
- When: Bar hits the ball.
- Then: Change the direction of the ball on opponent side.

### Scenario: declare winner
#### -
- Given: Game is running. 
- When: player1.score==11 and player2.score<11.
- Then: Declare player one as winner.
#### -
- Given: Game is running. 
- When: player2.score==11 and player1.score<11.
- Then: Declare player two as winner.
#### -
- Given: Game is running. 
- When: player1.score==11 and player2.score=11.
- Then: Tie.

### Scenario: control transfer
- Given: Player1's turn. 
- When: Bar hits the ball.
- Then: player1.is_my_turn=false and player2.is_my_turn=true.

### Scenario: control transfer
- Given: Player2's turn. 
- When: Bar hits the ball.
- Then: player2.is_my_turn=false and player1.is_my_turn=true.

