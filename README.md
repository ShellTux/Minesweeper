# Minesweeper Game

![A won expert game of KMines, a free and open-source variant of Minesweeper](https://upload.wikimedia.org/wikipedia/commons/1/1b/Kmines_Expert_Game_with_Numbers_1-8.png)

This is a command-line based implementation of the popular Minesweeper game in
various Programming Languages.

## Installation

Clone the repository:

```zsh
git clone https://github.com/ShellTux/minesweeper.git
```

Navigate to the directory:

```zsh
cd minesweeper
```

Navigate to a specific `language`:

```zsh
cd c
```

Compile the program: `make`

```zsh
make
```

## Game Rules

- The objective of the game is to uncover all the cells on the board that do not contain a mine.
- The player can `uncover` a cell by pressing `space`
- If a mine is `uncovered`, the `game is over`.
- If a cell does `not contain a mine`,
it will display a number indicating the number of neighboring cells that contain mines.
- The player can flag a cell by pressing `f`
- This is useful for marking cells that the player suspects contain mines.
- The game is won when all non-mine cells are uncovered.

<!-- ## Customization -->

<!-- The game can be customized by modifying the constants defined in game.h: -->

<!--     BOARD_SIZE: the size of the board (number of rows and columns) -->
<!--     NUM_MINES: the number of mines on the board -->

## Implementation

### Languages

- [x] C
- [ ] Pascal
- [ ] Python
- [ ] Rust
- [ ] Haskell ?

### C

- [x] Movement (w,  a,    s,    d)
- [ ] Movement (up, left, down, right arrows)
- [x] Press `space` to open a cell
  - [x] When the `revealed` cell is a `bomb`, then `game over`.
- [x] Open recursively empty neighboring cells
- [x] The `first cell` to be opened is __not__ a bomb
- [x] Press `f` to flag a cell
- [x] Print Table after an operation
  - [x] Print Number of bombs planted
  - [x] Print amount of opened cells
  - [x] Print amount of flagged cells
- [x] Win when exactly `all bombs have been flagged` and
`all non-bombs have been opened`.

## Acknowledgements

This game was inspired by the classic Minesweeper game by Microsoft.
License

This project is licensed under the MIT License. See the LICENSE file for details.