# Space Invaders Final Project for "How to code: Simple Data"

I completed the <a href="https://courses.edx.org/certificates/6cab91bc64474e0885eb4a72eb9c0b29">"How to code: simple data"</a> online course. For the final project, I created a space invaders game using racket, a teaching language based on lisp. Given lisp's lack of loops, I created the entire program using recursive functions.

The game runs by manipulating data. Different components are advanced according to their speeds and added or deleted from linked lists according to other events in the game (eg. collisions and key presses). Since racket lists are immutable, a new list was created each time with the addition or absence of components. This made it easy to test the logic of the game.

A big-bang function keeps the game going, repeatedly calling an update function that creates new data for the next frame. On each tick of the big bang, new images of your tank, missiles and invaders are rendered to the screen, giving the effect of movement.

If a missile collides with an invader, both the invader and missile are deleted from their respective linked lists and disappear from the screen. If a missile is fired (with spacebar), a new missile is added to the list of missiles and is therefore rendered to the screen. It is deleted again once it passes through the top of the screen, to avoid the game running out of memory.

Overall this course was excellent and mind expanding, it has definitely sparked my curiosity to learn more about functional programming in the future.

<img align="center" src="https://staceycarter-scholarship-application.netlify.com/spaceInvaders.gif" height=400px />

# Run the game
To run the space invaders project:
* Download the rkt file. 
* Open file in drRacket. 
* To run the game, type (main G0) into the console to set the initial state.

