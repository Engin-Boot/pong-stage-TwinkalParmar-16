# Interaction Sequences

## Startup Sequence

Authentication Module

## Movement Initiation

- Toggle Module
- Player Module
- Customization Module
- Exceptional Module

## One score

Toggle Module.

# Interations

1. Start 
## Authentication Module
   After varifying the player control will go to style module[if needed]/ player module.
   ### Methods
   - signIn(){
     <br/> Enter username and password
     <br/>authenticateUser()
    }
   - signUp(){
     <br/> Enter username and password
     <br/>authenticateUser()
   }
   - authenticateUser(){
   <br/> Matches with database
   <br/> Go to next activity
   }

2. Module Interacrion
## Player Module
   When player hits the ball then control will go to Toggle Module.
   And if some exceptional(restart/quit/close) event happens then control will transfer to Exceptional Event Module.
   
   ### Abstract Methods
   - missed()
   - notMissed()
   - moveUp()
   - moveDown()

   ### Player1 
   Inherits Player
   ### Impelentation of abstract Methods from Player class
   -  moveUp(){
    <br/> use up key
   }
   -  moveDown(){
    <br/> use down key
    }
   - notMissed(){
    <br/> call player1.changeTheDirection() from Toggle module.
    <br/> call player1.transferControl() from Toggle module.
   }
   - missed(){
   <br/> call player1.updateScore() from Toggle module. 
    <br/> call player1.checkWinner() from Toggle module
   }

   ### Player2 
   Inherits Player
   ### Impelentation of abstract Methods from Player class
   -  moveUp(){
    <br/> use 'W' key
   }
   -  moveDown(){
    <br/> use 'D' key
    }
   - notMissed(){
    <br/> call player2.changeTheDirection() from Toggle module.
    <br/> call player2.transferControl() from Toggle module.
   }
   - missed(){
   <br/> call player2.updateScore() from Toggle module. 
   <br/> call player2.checkWinner() from Toggle module
   }
  
 
## Customization Module
   After getting authorization it will have a option for customization to style the display.
   Both players can call the fucnctions from the customization module.
   player1.method_name or player2.method_name
   
   
## Exceptional Events
   - close(){
    <br/>  Save the current state.
    <br/> exit()
   }
   -reset(){
   <br/>player1.score=0
   <br/>player2.score=0
   }
   - declareWinner(){
    <br/>  if(player1.score > player2.score)
    <br/>  then
    <br/> Display Winner is player1.name
    <br/> if(player2.score > player1.score)
    <br/> then
    <br/> Display Winner is player2.name
    <br/> else
    <br/> Display Tie
   }
   - quit(){
   <br/> player1.reset()
   <br/> player2.reset()
   <br/> exit()
   }
   - sessioExpeired(){
   <br/> after fixed time period
   <br/>Show session Experied
   <br/> quit()
   }

   
    
 
   
   

  
   

