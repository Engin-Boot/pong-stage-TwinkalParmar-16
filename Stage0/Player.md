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

### Scenario: varify the user
- Given: Has clicked to SignIn or SignUp. 
- When: Enter userName and Password and clcik to submit.
- Then: Compare the username and password with the database.

### Scenario: authorized user
- Given: Has username and password. 
- When: When username and password matches with database.
- Then: Allow user to play the game and navigate to the next page.

### Scenario: unauthorized user
- Given: Has username and password. 
- When: When username and password does not match with database.
- Then: Will not allow user to play the game and 
        dsiplay create account or reset password.


