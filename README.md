# gol-js-cucumber
Game of Life in JavaScript

## Introduction
[From Wikipedia: https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life]

The Game of Life is a cellular automaton devised by the British mathematician John Horton Conway in 1970. It is a zero-player game, meaning that its evolution is determined by its initial state, requiring no further input. One interacts with the Game of Life by creating an initial configuration and observing how it evolves.

## Rules

The universe of the Game of Life is an infinite, two-dimensional orthogonal grid of square cells, each of which is in one of two possible states, live or dead. Every cell interacts with its eight neighbours, which are the cells that are horizontally, vertically, or diagonally adjacent. At each step in time, the following transitions occur:

* Any live cell with fewer than two live neighbours dies, as if by underpopulation.
* Any live cell with two or three live neighbours lives on to the next generation.
* Any live cell with more than three live neighbours dies, as if by overpopulation.
* Any dead cell with exactly three live neighbours becomes a live cell, as if by reproduction.

The initial pattern constitutes the seed of the system. The first generation is created by applying the above rules simultaneously to every cell in the seed, live or dead; births and deaths occur simultaneously, and the discrete moment at which this happens is sometimes called a tick. Each generation is a pure function of the preceding one. The rules continue to be applied repeatedly to create further generations.

## Examples

Here are two examples of seeds -- one that will remain static, and one that will evolve. In these examples, '.' represents a dead cell, and '*' represents a live cell.

### Block

This pattern will remain the same from tick to tick. In other words, it will never change. Based on the rules, can you figure out why?  

```
...      ...
.**  ==> .**
.**      .**
```

### Blinker

This pattern will oscillate between two states from tick to tick. Based on the rules, can you figure out why?

```
...      .*.       ...
***  ==> .*.  ==>  ***
...      .*.       ...
```


