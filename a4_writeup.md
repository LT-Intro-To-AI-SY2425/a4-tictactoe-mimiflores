# Assignment 4 - Writeup

In assignment 4 we created a basic tic tac toe game so that we could learn object oriented programming. Respond to the following questions.

## Reflection Questions

1. What was the most difficult part to tic-tac-toe?
The hardest part to tic-tac-toe was figuring out how to check every time for all the possible combinations of wins after a move. I was doing it in a really long way and I thought of using a loop to check through each instance, but I found a more pythonic way using chatgpt using return any(all(self.board[pos] == player for pos in combo) for combo in winning_combinations) to check for all of the combinations using only one line. 
2. Explain how you would add a computer player to the game.
A computer could be added by randomizing the moves for the second player (O) every time. The user can be player one using the X's and for every move of the second player, the computer can randomly choose a spot on the board (checking each time to make sure it is available and generating another number within the range to try another) to place their move. 
3. If you add a computer player, explain (doesn't have to be super technical) how you might get the computer player to play the best move every time. *Note - I am not grading this for a correct answer, I just want to know your thoughts on how you might accomplish it.
I think the best way to do this would be to use the possible combinations of wins and see which spots are taken by the computer's O's. Then the next move could be placed in one of the spots of the possible win combination with the most spots taken up by its pieces. I think this would be hard to do as it would involve a lot of loops and logical thinking but I think it is definitely possible to use this method. 