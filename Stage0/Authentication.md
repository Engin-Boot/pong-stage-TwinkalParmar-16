# Authentication
  Allow the player to play the game.
  

## Feature

### Variables
- Username
- Password

### Methods
- SignIn()
- SignUp()
- VarifyUser()
- resetPassword()

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

