# Pacman Game README

## Overview

This repository contains Python code for a Pacman game simulation. The goal of the game is for Pacman to eat all the tokens on the board without being caught by the ghosts. The game board is represented as a matrix, and various objects are denoted by specific numerical codes.

## Game Objects

- **99**: Wall
- **88**: Player eaten by a ghost
- **77**: Player (Pacman)
- **21/20**: Red ghost with/without a pill
- **31/30**: Blue ghost with/without a pill
- **41/40**: Yellow ghost with/without a pill
- **51/50**: Green ghost with/without a pill
- **11**: Normal slot with a pill
- **10**: Empty slot

## Input Representation

The input describing the initial state of the game is a matrix (game) of size NxM, where each entry represents the initial state of the objects. The game can end either in success (all tokens eaten) or failure (Pacman caught by a ghost).

## Player Actions

You have four player actions:
- **R**: Shift to the right
- **D**: Move down
- **L**: Shift to the left
- **U**: Move up

After each player action, the ghosts move according to specified rules.

## Ghost Movement Rules

- Each ghost moves in one of the four directions (up, down, right, or left).
- Order of movement: player, red ghost, blue ghost, yellow ghost, green ghost.
- Ghosts move towards the player based on Manhattan distance.
- If two directions are equally close, priority is given to right, down, left, and finally up.
- A ghost cannot stay in place unless it has no valid slot to move to.
- A ghost cannot move to a slot occupied by another ghost or a wall.

## Code Structure

1. **ex1.py:** File where main work is done. 
2. **ex1_check.py:** Shell script containing functions to test the problem-solving code. 
3. **Search.py:** Contains search algorithms and the node class.
4. **utils.py** Reference files remain unchanged.

## Getting Started

1. Clone the repository: `git clone https://github.com/yourusername/pacman-game.git`
2. Navigate to the project folder: `cd pacman-game`
3. Modify the `py1.Ex` file to implement the required functions.
4. Run the test script: `./py.check_1ex`

Feel free to explore the code files for a deeper understanding of the implementation details. Good luck with your Pacman adventure!
