I kept playing with my idea of a card game for a MU* and the MU* portion of it. 

Single player mode is mostly puzzle solving. The puzzles are challenges using a predetermined board state.

The game itself is about Tinkers controlling a magic breadboard to try and win by dealing damage directly to their opponent.

Tinkers are protected by several shields, which act as logic gates! (NOT, AND, OR, etc) Whys that? Because the Gadgets they build are stacks. Stacks have three states - PEEK, PUSH, POP.

Stacks get peeked at at some point during the turn. Whatever the peek effect is happens. Pushing happens when the card is added to the stack. Popping when its removed. 

Cards have Durabilities that go down every time they're peeked at. When it reaches 0, the card pops off the stack into the discard pile.

Cards can have empty spaces, if a space is empty then whatever is already on the stack stays.

You can empty a stack to make a shield. The cards in the stack influence this somehow, but I'm not certain how. It has to do with the NOT/AND/OR mechanics. It could be fun if you have to initially populate the shields yourself at the start of the game. 

Tinkers have a list of commands they can do at the start of the turn. Its a small list chosen at the start of the match, from a larger list. The default large list is very useful and versatile, but you can quest for more specific and powerful commands to add to your collection.

- - -

# "Screenshots"

## Field

Roughly what I think the field might look like. `0` is the player. `[ ]` are the stacks. `+` are the gates. The `|` lanes indicate what gates influence what Gadgets.

```
     0

[ ] [ ] [ ]
 +   +   +
 |   |   |
 |   |   |
 |   |   |
 +   +   +
[ ] [ ] [ ]

     0
```

## Cards

Definitely what I think cards are like, aside from the effects. The number on the top right is the durability. When something with a blank space is played onto a stack, it does *not* overwrite whatever is in that slot.

```
Boingle (3)

PEEK  Gain 1 Durability
POP   Tinker +1 Health
PUSH  Tinker +1 Health
```

```
Dingle (5)

PEEK  Tinker +1 Health
POP   
PUSH  
```

then if you play Dingle on top of Boingle

```
DingleBoingle (5)

PEEK  Tinker +1 Health
POP   Tinker +1 Health
PUSH  Tinker +1 Health
```
