Tic-Tac-Toe (Python Console Game)

This is a simple command-line Tic-Tac-Toe game implemented in Python.
Two players (X and O) take turns to choose positions on a 3×3 board (using numbers 0–8).
The game ends when a player wins or when the board is full (resulting in a draw).

 Features

Two-player console gameplay

Automatic win detection

Input validation (prevents invalid or duplicate moves)

Simple and easy-to-understand code

Shows the board after every move

How to Play

The game board is represented using positions 0 to 8:

0 | 1 | 2
-------
3 | 4 | 5
-------
6 | 7 | 8


On your turn, type a number from 0 to 8 where you want to place your mark (X or O).

 Game Logic

The winner() function checks all 8 possible winning combinations:

3 rows

3 columns

2 diagonals

The game alternates turns between X and O.

The game ends when:

A player wins

All cells are filled (draw)

Code Overview
Board Storage

The board is stored as a list of 9 elements:

b = [" "," "," "," "," "," "," "," "," "]

Display Function

Prints the board in a 3×3 format:

def show():
    print(b[0],"|",b[1],"|",b[2])
    print("-------")
    print(b[3],"|",b[4],"|",b[5])
    print("-------")
    print(b[6],"|",b[7],"|",b[8])

Win Checker

Evaluates all winning patterns:

def winner(p):
    ...

 Running the Game

Run the Python file:

python tic_tac_toe.py


You will be asked:

where do u wanna go (0-8) :


Enter a number and continue playing until the game ends.
Example Gameplay
X | O |  
-------
  | X |  
-------
  |   |  

where do u wanna go (0-8) :
