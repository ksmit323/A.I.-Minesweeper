# Minesweeper A.I. with Pygame

This is an AI program that plays the classic game of Minesweeper with a graphical interface implemented with Pygame. It uses a knowledge-based approach using propositional logic to identify and flag mines, and to reveal safe cells.

## Installation

To run the program, you'll need Python 3.7 or later installed on your computer, as well as Pygame. You can install Pygame by running:
```
pip install pygame
```
Once you have Python and Pygame installed, download the source code from the repository and navigate to the project directory in your terminal.
```
git clone https://github.com/ksmit323/A.I.-Minesweeper.git
cd A.I.-Minsweeper
```

## Usage
To start the game, run the **'runner.py'** file.
```
python runner.py
```
The game will display a graphical interface of the Minesweeper game board. The AI will then automatically begin playing, using propositional logic to identify safe cells and flag mines as it goes.

## Propositional Logic
The Minesweeper AI uses a knowledge-based approach using propositional logic to reason about the game board. The board is represented as a set of propositional variables, with each variable representing a cell on the board. The AI then uses rules of inference to deduce which cells are safe and which cells contain mines.

The AI uses several types of rules, including:

- **Single-cell rule**: If a cell is known to be a mine or a safe cell, then all other cells that are adjacent to it are affected by that knowledge.
- **Counting rule**: If the number of unknown cells adjacent to a cell equals the number of mines that must be in the adjacent cells, then those unknown cells must all contain mines.
- **Subset rule**: If a set of cells is known to contain a certain number of mines, and that number is equal to the number of mines that must be in a larger set of cells that contains the first set, then the larger set must contain all of the mines.
These rules are combined to create a knowledge base, which is used to make inferences about the game board.
