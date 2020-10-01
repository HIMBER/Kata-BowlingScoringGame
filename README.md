# BowlingScoringGame

## Classes

Start with a Game class, which has two methods: Roll and Score.  
The Roll method take the number of pins knocked down for a given game.  
The Score method is called at the end of the game and returns the score of the game.  

Next is the Frame class — and a Game has 10 frames.  
The Frame class has one function, Score, which returns the score for a given frame.  

However, in the case of a spare or strike, the Score function will need to look ahead to the next frame to score the current frame — we therefore have the reference for the frame object back onto itself, indicating that dependency. 

Next is the Roll class, and a Frame has 1 or 2 Rolls, except in the tenth frame, where it will have 2 or 3 rolls — as indicated by the sub-type Tenth Frame, which has one additional role (as indicated).

The Roll class has a private attribute of pins which holds the number of pins knocked down on a given roll. 
