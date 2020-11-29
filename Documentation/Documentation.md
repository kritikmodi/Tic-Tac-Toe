### HOW TO BUILD THE TIC-TAC-TOE GAME USING PYTHON :
>The game is playable directly on the terminal, Python GUIs are not used for building this game.

To build the **tic-tac-toe** game, you essentially require _3 components_ :

* A game board.
* A function to take input from the user meanwhile flipping the player from O to X and X to O during each turn.
* A function to check whether any player won or tie after each turn.

The workflow or the _program-flow_ should go like this :

* Display the board.
* Ask the user to select any empty postion with the current token(X or O).
* Fill that position with the current token(X or O).
* Display the resulting board.
* Check whether it's a win or tie.
* Display appropriate message if there's a win or tie.
    > It's a win if any row, column or diagonal is filled with the same token(X or O). It's a tie if all the slots are filled but there's no win.
* Flip the token(X to O or O to X) and loop the entire process again if there's neither a win nor a tie.

### FUNCTIONS BREAKDOWN :

Following are the functions used to build this game in the Python code provided :

* **`play_game()`** : This function is called as soon as the program is executed. It calls all the other functions for successful execution of the game, namely `display_board()`, `handle_turn()`, `check_if_game_over()` and `flip_player()`.

* **`display_board()`** : This function displays the current board during each turn or iteration.

* **`handle_turn()`** : This function takes the input from the user(the position on the board where he wants to place his token(X or O)), checks whether it's valid and available and then allots the respective board position with the current token(X or O).

* **`check_if_game_over()`** : This function checks whether the game is over or not by checking for a win or a tie using the functions `check_for_winner()` and `check_for_tie()`.

* **`check_for_winner()`** : This function checks whether it's a win after each turn or iteration by using the functions `check_rows()`, `check_columns()` and `check_diagonals()`. It's a win if any row, column or diagonal has the same token(X or O) throughout. 

* **`check_rows()`** : This function checks if any of the 3 rows has the same token(X or O) throughout and returns the result accordingly.

* **`check_columns()`** : This function checks if any of the 3 columns has the same token(X or O) throughout and returns the result accordingly.

* **`check_diagonals()`** : This function checks if any of the 2 diagonals has the same token(X or O) throughout and returns the result accordingly.

* **`check_for_tie()`** : This function checks whether there's a tie after each turn or iteration and returns the result accordingly. It is a tie if all the slots are filled but there's no win.

* **`flip_player()`** : This function flips the player or token, that is, X to O and O to X after each turn or iteration of the game.

##### NOTE :

* Details of the variables and loops are provided as comments in the code itself along with the logic associated with each function.

* In the code, `player` refers to the token, that is, X or O.

* You only need any Python environment to run this code.
