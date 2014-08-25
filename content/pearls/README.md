Pearls
======

Game Rules
----------

Pearls is a brilliantly simple game. We start with 3 rows of pearls:

    O O O
    O O O O
    O O O O O

Two players take turns. On their turn, a player can take as many pearls as they
want (minimum 1) from a *single* row.

A player wins by forcing the opponent to take the last pearl left. An example
game where player 1 wins:

    O O O
    O O O O
    O O O O O
    Player 1 takes all pearls in row 3
    O O O
    O O O O

    Player 2 takes all pearls in row 2
    O O O


    Player 1 takes 2 pearls in row 1
    O


    Player 2 must take the last pearl.

An example where player 2 wins:

    O O O
    O O O O
    O O O O O
    Player 1 takes all pearls from row 1

    O O O O
    O O O O O
    Player 2 takes 2 from row 2

    O O
    O O O O O
    Player 1 takes 2 from row 2


    O O O O O
    Player 2 takes 4 from row 3


    O
    Player 1 must take the last pearl.


Data Representation in Python
-----------------------------

We can create very simple (but rather ugly) code by storing the number of
pearls in each row in one variable per row:
    
    row_1 = 3
    row_2 = 4
    row_3 = 5

and subtracting values from each variable as necessary.

One nicer representation could be using a Python dictionary to map rows to
numbers of pearls left:

    pearls_per_row = {1: 3, 2: 4, 3: 5}

and referencing remaining pearls using just the row number: `pearls[1] -= 2`.

Arguably the 'nicest' representation for pearls per row is just using a simple
list:

    pearls_per_row = [3, 4, 5]

Now, we have a really simple mapping between row number and number of pearls in
the row:

    pearls_per_row[row_num] -= num_to_remove

As such, we have code that looks remarkably similar to the code we create when
using a dictionary, but the data structure used is much more straightforward.

Checkpoints
-----------

### Week 2
Lesson: game rules

Implement the game engine: ability to start a game, take turns, affect the game
state by choosing a move, etc.

### Week 3
Lesson: user input and effective interfacing

Create the command line interface: print out the game board, prompt users for
turns, give nice feedback (is that move legal (allowed)? did someone just win?
can you determine a win BEFORE someone takes the last pearl?

### Week 4
Lesson: turtle

Use turtle to create a simple graphical depiction of the game state. Redraw the
pearls when someone makes a move. Maybe print out who's turn it is on the
turtle canvas?

*Extension:* implement the whole game using TKinter. No command line interface!


### Week 5
Lesson: no lesson! We're not giving you the answer!

Write a program to play this game. There exists an algorithm to beat a human
opponent almost all the time. Can you work it out? (note: Google is a
programmer's best friend.)
