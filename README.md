# Game-using-python
Implementation of chess in python language in which 2 players can play this game. Using "R" key we can undo this game and "Q" the game ends in between. There is 2 Classes in code.
1. One is GameState() which will store the positions of the pieces. 
    a. It has changePosition() function which will change the position of the pieces as per request. 
    undoSteps() will undo to the previous state. 
    b. availablePositions() will give all the possible moves a piece can move at that position. 
       availablePositions() will call respective functions of pieces like bishopAvailablePositions(),              queenAvailablePositions(), etc. Pawn can move in forward direction and in left or right only if              opposite color piece is there. For rook, we create directions=((-1,0),(0,-1),(1,0),(0,1)) where each        set() represents the direction that piece can move. Similar we use different logic for other pieces          as well.
2. Another Class is Steps() which is used as a data structure to store initial and final positions of rows      and columns as well as unique number(unique ID), attacking piece and piece captured.

To get input from user, pygame is used. Whenever user clicks on game window, we get the position, where we clicked, using mouse.get_pos(). Some graphics is also used to make the game more enjoyable.
