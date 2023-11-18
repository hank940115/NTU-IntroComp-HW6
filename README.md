# [Tic-Tac-Toe Game](https://en.wikipedia.org/wiki/Tic-tac-toe)

You are tasked with designing a simple Tic-Tac-Toe game. The game rules are as follows:

Tic-Tac-Toe is played on a 3x3 grid, where two players take turns marking 'X' and 'O' on the grid. The objective is to form a line of three identical marks.

When one player wins, the game ends, and that player is declared the winner. If all the cells are filled, and no player wins, the game is declared a draw.

## The submission format
```
  [Name of your repo]/
          |
          |── python/
          |    ├── main.py
          |    ├── args.py
          |    ├── test.py
          |    └── ...
          |
          └── git/
               ├── [student_id]-0.png
               ├── [student_id]-1.png
               └── ...
```

## Execute

* What Tas will run
```
python main.py --input_dir input_dir_path --output_dir output_dir_path
```




#### This program takes two parameters:  *input_folder* and *output_folder*. 

## Input


It reads multiple input files from the input_folder, each containing a series of player moves. Each move is represented by a pair of integers, row and col, indicating the player's position on the board (X makes the first move). 

Input :
```
1 1
1 2
2 2
1 3
2 3
```

## Output

Your program should simulate the entire game based on these moves and, upon game completion, write the final board state 
**( By self.print_board() function )** and the game result *(“Player X wins!”, “Player O wins!”, or “It's a draw!”)* into the corresponding file in the output_folder (with the same file name). 
Please use the provided TicTacToe class to implement this functionality, as it already includes the logic for the Tic-Tac-Toe game.


**1. The final board state**  : use ```self.print_board()``` function

**2. The game result:**

* X wins : please write "Player X wins!" (uppercase X)

* O wins : please write "Player O wins!" (uppercase O)

* Draw : please write "It's a draw!"


output : 
```
X | O |  
---------
O | X |  
---------
  |   | X
---------
Player X wins!
```

#### The output has to be in the format we require.
You can make sure whether your format is correct by using the command.
```
python test.py --output_folder your_answer_path/ --answer_folder testanswer/
```

# Note
1. Ensure that your program can handle invalid inputs (e.g., moves outside the board's boundaries or occupied positions) by ignoring them.

Example: 

Input: 
```
2 1
5 2
1 1
2 3
1 2
3 3
1 3
```

output : 
```
O | O | O
---------
X |   | X
---------
  |   | X
---------
Player O wins!
```

2. Please note that your program should be able to process multiple input files and generate the corresponding outputs for each file, and the output file names need to be the same as the input file names.

3. In each game, there will always be a winner or a draw as the final outcome. If the result is already determined, there is no need to consider further input.


Example: 

Input: 
```
1 1
1 2
2 2
2 1
3 3
2 3
3 2
```
output : 
```
X | O |  
---------
O | X |  
---------
  |   | X
---------
Player X wins!
```
# What you have to do

Fill in the program where we have requested in ```main.py``` and ```args.py```, and do not modify other parts.
