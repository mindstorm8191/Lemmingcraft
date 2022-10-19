# Lemmingcraft

The aim of this project is to create an animated kind of programming language that is fun to sit and watch it work. Each block on the grid can contain a creature that performs an action on the data it recieves, complete with animations showing it working. It's hard to say how many types of blocks we'll have by the end of this, but hopefully it'll all be fun!

### Current plans

This will be based loosely on an esoteric language called Befunge, be sure to check it out.

Program flow will be managed using carts. These will contain stacks that hold your data; many operations will deal with operations on that stack. Multiple carts can be used with your program; Programs can start with several carts, running carts can be duplicated, and new carts can be spawned from actions of your program.

### Planned commands

-   Add - Pops two numbers off the stack, then pushes the sum of both onto the stack
-   Sub - Pops 2 off the stack, then pushes (top-under) onto the stack
-   Mult - Multiplies the top 2 numbers on the stack
-   Div - Divides the top 2 numbers on the stack (top/under)
-   Mod - Takes the modular of top/under, pushing it to the stack
-   Dup - Copies the top value on the stack, placing a 2nd copy of it there
-   DupUnder - Pops the top value (a), then copies the value a slots down and puts it on top of stack
-   GetUnder - Pops the top value (a), then pops the value a slots down, putting it on top of stack
-   PutUnder - Pops 2 values (a & b), then goes a slots down and places b there. Anything above is pushed higher in the stack
-   Arrow - Changes the direction the cart is traveling
-   Comp - Checks if the top value is 0. If so, program flow will to left. If not, it will go right.
-   Gap - 'lazy block'. Allows program to continue on, not doing anything. This is particularly useful when building custom code with blocks
-   Mget - Pops the value from Fetches data from memory
-   Display - Displays a string of characters from the stack
-   Start - Where a cart is spawned from, when the program begins
-   End - Where a cart stops, indefinitely

### Things to do next

I don't have a lot currently available for this project, so there's a lot that needs to be done

-   Make some more sample programs to toy with. These will be needed to better decide what commands are needed in the language
-   Start making some artwork. Lemming characters will need to be animated to some degree; hopefully we can come up with some idle animations, along with actively working ones
-   Start on a rudimentary interpreter, that puts the artwork into a workable display of the user's program working. Then get this ironed out.
-   Figure out what needs to be done next
