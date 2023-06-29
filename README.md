# Chess Engine


## Summary 
Here is a Chess Engine where a user can play against the computer, the engine is made using pygames.

The engine incorporates all the valid moves of the game such as -
1. En Passant
2. Pawn Promotion
3. Chckmate and Stalemate
4. Castling
   
It also has features to highlight valid moves for a seleced piece, undo the last move, reset the game and move animation.

## Computer Moves
Used Greedy Algorithm to predict the best move out of all the valid moves. Here every piece is given a score according to its importance and both the players try to move the score in opposite directions.

The to compute the moves upto two stages and then make the the best move possible, I used MinMax algo to select a move that minimizes the best score of the opponent.

To calculate the MinMax score recursively upto a depth of chioce, I used NegaMax algo

However the engine was taking more time to make its move so to optimise the time taken, I used Alpha Beta Pruning, which made the program run faster.

## Requirements
Install pygame

`pip install pygame`

## Instructions 
1. Clone this repository.
   `git clone https://github.com/priyansh2612/ChessEngine.git`
2. Install the requirements

3. Run `Main.py`

* Press `z` to undo a move.
* Press `r` to reset the game.
