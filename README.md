# Lab 1.4: Eat it all!

## Overview

Today you will write a game where the player must eat all the food which appears—while avoiding an enemy which bounces around the screen!

### Part 1: Start wherever!

You will first learn how to make sprites appear regularly at random locations using the on game update every x ms and pick random from blocks.

1. Create a new MakeCode Arcade project called “Eat It All”.
2. From the Game drawer, add an on game update every 500 ms block to your project. Set the time 3000 ms (remember: 1000 milliseconds =1 second).
3. From the Sprite drawer, add a sprite of kind Food to the on game update every 3000 ms block. Name this sprite whatever you want and select any image you would like.
4. From the Sprite drawer, add a set sprite position block to your on game update block.
5. From the Math drawer, add a pick random 0 to 10 block to your project.
6. Connect it to the x entry in your set sprite position block.
7. In the pick random block, set the first number to 10 and the second number to 142.
8. Add a second pick random block to the y position in your set sprite position block. Set the numbers to 10 and 102.
9. Run your program.
 
*Where do the Food sprites appear?*

*What happens if you change the numbers in the pick random block?*

*Why do you think the numbers 10 and 142 were initially selected for the x position, and the numbers 10 and 102 for the y position?*

#### Part 2: Eat it all!

10. From the Sprite drawer, add a sprite of kind Player to your on start block. Name it whatever you want and select whatever image you want. Then add blocks so the Player:
- a. Starts in the middle of the screen
- b. Stays on the screen
- c. Moves with the buttons
11. From the Sprite drawer, add a sprite of kind Enemy. Name it whatever you want and select whatever image you want. Then add blocks so the Enemy:
- a. Starts in a random location
- b. Moves with a random velocity
- c. Bounces off the edges of the screen
12. Add an on sprite overlaps block to your game. Set it so it will run when a sprite of kind Player collides with an otherSprite of kind Enemy. Then add blocks so:
- a. The otherSprite (which is the Enemy sprite) moves to a new random location with a new random velocity.
- b. You can drag the red otherSprite block from the top of the on sprite overlaps block and connect it to mySprite space in the set sprite position block.
13. Add another on sprite overlaps block to your game. Set it so it will run when a sprite of kind Player collides with an otherSprite of kind Food. Then add blocks so:
- a. The otherSprite (which is the Food) sprite is deleted with some effect.


#### Part 3: Points! Lives!

So far, your game has a player, an enemy, and some food to eat. Now let’s add some scoring and lives.

1. Let’s make the player lose a life when they collide with the Enemy.

From the Info drawer, find the change life by -1 block and add it to the appropriate on sprite overlaps block. 

2. Now let’s increase the score when the player collides with some Food.

From the Info drawer, find the change score by 1 block and add it to the appropriate on sprite overlaps block. 

Run your program. What happens when you collide with some food or the enemy?

What happens when you collide with the enemy three separate times?


Bonuses

Here are some things you can add to your game which can make it more interesting and personal!

14. Make both the Player and Enemy relocate when they collide.
15. Have the player lose points if the Enemy collides with Food.
16. Play a sound when the Enemy and Player collide, and when the Player and Food collide.
17. Design your own sprites.
18. Add a background.
 
What else can you think of?
Rubric

Lab 1.4 criteria

Point values

Part 1

4 Total Points

on game update every 3000 ms block added

1 point

Food sprite created

1 point

Food sprites appear at random location

2 points

Part 2

4 Total Points

Player sprite created properly

1 point

Enemy sprite created properly

1 point

on sprite collides block for Player and Enemy created properly

1 point

on sprite collides block for Player and Food created properly

1 point

Part 3

2 Total Point

Score updated appropriately

1 point

Lives updated appropriately

1 point

Project total

10 total points


