## Final project for CS246 Fall 2016 by Simran Kaur and Fatima Taj

Quadris is a Latinization of the game of Tetris. Unlike Tetris, Quadris is not real-time. It gives the user as much time as needed to drop a block. 

This project uses many OOP principles such as polymorphism, encapsulation, inheritance, and abstraction. The design uses abstract base classes to organize components such as levels and blocks. The Factory Method design pattern has also been implemented to generate different blocks at different levels.

<img src="http://i67.tinypic.com/2zg6q1x.jpg" alt="quadris_screenshot" style="width:355px;height:591px;">

Build game by typing 'make'

Run game by typing ./quadris followed by command line options

# Command Line Options:
* -scriptfile file: generates block based on file
* -startlevel x: starts game on level x
* -seed x: sets seed as x
* -text: runs game in text mode only

Example: 
./quadris -text -scriptfile blocks.txt

# Commands:
* left: moves block one unit left
* right: moves block one unit right
* down: moves block one unit down
* clockwise: rotates block 90 degrees clockwise
* counterclockwise: rotates block 90 degrees anticlockwise
* drop: drops current block
* levelup: increases the difficulty level of the game by one 
* leveldown: decreases the diffculty level of the game by one
* norandom file: relevant only during levels 3 and 4, this command makes these levels non-random, instead taking input from the sequence file
* random: relevant only during levels 3 and 4, this command restores randomness in these levels
* sequence file: executes the sequence of commands found in file
* restart: clears the board and starts a new game

# Levels:
* 0: Takes blocks from sequence.txt or file specified on command line
* 1: Z and S blocks produced with probability 1/12 each, all other blocks produced with probability 1/6
* 2: All blocks produced with equal probability
* 3: Z and S blocks produced with probability 2/9, all other blocks produced with probability 1/9. Blocks are also considered "heavy" meaning each move is followed by a downward shift of one cell.
* 4: Same as level 3, but star block is dropped if a row is not cleared in 5 moves



