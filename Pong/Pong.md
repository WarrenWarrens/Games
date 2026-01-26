# PONG

## How To Run:
#### Unzip & run file

## How To Play:
#### Use W & S keys to move up or down

## Features

#### Player & CPU move smoothly, collide with border walls 
and upon balls impact with the paddle or walls, a sound plays, 
paddles change colours and speeds up. 
As a score is earned, the UI updates. The ball randomly shoots in either left or right direction

There is no Menu or Game Over state currently present, i apologize

There is also no Bonus feature added, once again, i apologize 

## AI Description

#### The AI constantly keeps track of the balls position, 
and uses it as tracking to ensure the paddle hits the ball.
We calculate the distance between the paddle & the ball, then
check to see if the absolute value (done to avoid division by 0)
of the distance is greater than the speed of the paddle.
If so, we move by the distance / abs(distance)
if not, we just move by the distance.
Then we adjust the position.y value off the distance we calculated & ensure
the paddle remains in range of play with the clamp function. 
