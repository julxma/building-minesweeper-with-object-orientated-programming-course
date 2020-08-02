Let's object-oriented programming to build a classic and nostalgic Minesweeper game in Python!

*Image result for minesweeper gif

If you need a reminder of the rules of Minesweeper, here are the rules we are going to implement our version of Minesweeper by:

1) Players will select tiles from a 10x10 grid. If a mine is clicked then the game is over. For the purposes of our game, we will have 10 mines.

2) Each non-mine tile is labelled with a number if it is adjacent (all 8 neighbors) to a mine, in which case, the number shown will be the number of mines adjacent to that tile.
    - If there are no mines adjacent, there will be a blank tile (no number) shown.

3) If a tile is clicked, then there are three possibilties:
    1. The tile has no adjacent mines: The (blank) tile and its neighbors all show. If any of the neighboring tiles are also blank, i.e. have no adjacent mines, then the neighboring tiles and their neighbors also have to be shown.
            Note: please reference the animation if this isn't clear. You will have to use recursion to complete this.
    2. The tile has adjacent mines: The tile just shows with its number of neighboring mines.
    3. The tile is a mine: The game is over.

4) Players also have the option to flag where they think mines are located with the letter "F".

Here are a couple examples of how your output should look:

Capture

After the first move "55", then the board looks like this:

Capture(2)

A little further down the game, I have made some more moves, and I know a flag is at "36". If I want to place a flag there, it would look like this:

Capture(3)

Notice the "F" at column 3, row 6.

Here are some guiding questions to help get us start thinking about how to implement this game:

- How do we use object-oriented programming to implement this game?
- What are the expected inputs of this game?
- What inputs are considered invalid?
- What class(es) are needed for this program? Think about what are the objects (in a literal sense) exist in the Minesweeper game.

Remember that it is good practice to make our code as modular when possible!