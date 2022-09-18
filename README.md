# Snake-Game

## Overview

### Snake

Snake, the game that after so many years is still a classic from many people childhoods around the world. This game simulates a snake eating a fruit and getting longer everytime it eats one.

Technologies used:
1. HTML
2. CSS
3. JAVASCRIPT

## User Stories

As an user, I want the ability to...

-Start the game moving the keyboard arrows.
-Watch the snake getting longer everytime it collides with the fruit.
-See the score increase everytime the snake eats the fruit.
-See an announcement that the game is over.

## Wireframes / Screenchots
![IMG_0458](https://user-images.githubusercontent.com/77081100/190926274-def3ee8d-0cf2-41cc-9c45-40c560f68968.jpg)

![IMG_0458](https://user-images.githubusercontent.com/77081100/190926274-def3ee8d-0cf2-41cc-9c45-40c560f68968.jpg)


## Entity Relationship Diagrams (ERDs)

Snake: {
   x: 10(subject to change)
   y: 10(subject to change)
   height: 15(subject to change)
   width: 15(subject to change)
   color: green
   alive: true
   render: function () {
   ctx.fillStyle = this.color
   ctx.fillRect(this.x, this.y, this.width, this.height)
   }
}

Fruit: {
    x: 200(subject to change)
    y:100(subject to change)
    height: 10(subject to change)
    width: 10(subject to change)
    color: red
    alive: true
    render: function () {
   ctx.fillStyle = this.color
   ctx.fillRect(this.x, this.y, this.width, this.height)
    }
}

function - gameloop - holds the entire logic that runs the game
function - detectHit - used to see if items have collided with one another
function - movementHandler - used to move the snake around, should be attached to arrow keys.
