# Snake-Game

This is a simple implementation of the classic Snake Game in C++ using the console.
The game features a snake that the player controls using arrow keys to collect food and grow longer. 
The goal is to achieve the highest score without colliding with the borders or the snake's own tail.

## Features
- Responsive arrow key controls.
- Dynamic difficulty modes (easy and difficult).
- Score tracking.
- Game-over screen.

## How to Play

1. Clone the repository to your local machine.

2. Compile the code using a C++ compiler.

3. Execute the compiled executable to start the game.

4. Use arrow keys (up, down, left, right) to control the snake.
   - Up Arrow: Move Up
   - Down Arrow: Move Down
   - Left Arrow: Move Left
   - Right Arrow: Move Right

5. Press `1` to play in difficult mode or `2` to play in easy mode.
   - Difficult Mode: Faster snake movement (30ms delay).
   - Easy Mode: Slower snake movement (100ms delay).

6. The game will continue until you collide with the borders or the snake's own tail.

## Code Overview

### Initialization
- The game initializes with the snake positioned in the center, and a randomly placed food item.
- The score starts at zero.

### Drawing
- The game screen is drawn using the console, with the snake represented by "O", food by "*", and tail segments by "&".
- The score is displayed at the bottom of the screen.

### Input
- Arrow keys are used to control the direction of the snake.
- Input is handled using `_kbhit()` and `_getch()` functions.

### Logic
- The logic of the game involves updating the positions of the snake and checking for collisions.
- Tail segments are updated to follow the head.
- Collisions with borders, the snake's own tail, and food are checked.

### Difficulty Modes
- The game has two difficulty modes: difficult and easy.
- The sleep duration between frames is adjusted based on the selected mode.

## Enjoy the Game! 🐍
