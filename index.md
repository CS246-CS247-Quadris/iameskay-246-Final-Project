## Final project for CS246 Fall 2016 by Simran Kaur and Fatima Taj

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

<img src="http://tinypic.com/view.php?pic=2zg6q1x&s=9#.WEok9qIrIp8"></img>
