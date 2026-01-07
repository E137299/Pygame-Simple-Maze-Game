Pygame: Simple Maze Game 

## Program Requirements

### 1. Setup

* Create a new Python file called `maze_game.py`
* Import the following modules:

  ```python
  import pygame
  import sys
  ```
* Initialize Pygame and create a window (suggested size: **800 x 600**)

---

### 2. Player Class

Create a class called `Player` that:

* Inherits from `pygame.sprite.Sprite`
* Creates a visible rectangle (square or circle)
* Stores a movement speed
* Can move using the **arrow keys** or **WASD**

**Player Requirements**

* Has an `image` and `rect`
* Starts at a visible position
* Moves smoothly when keys are pressed
* Stops moving if it collides with a wall

---

### 3. Wall Class

Create a class called `Wall` that:

* Inherits from `pygame.sprite.Sprite`
* Creates a rectangular wall of any size
* Uses a solid color (gray or black recommended)

**Wall Requirements**

* Has an `image` and `rect`
* Position and size are passed into the constructor

---

### 4. Sprite Groups

Create the following sprite groups:

* `all_sprites`
* `walls`

Add:

* The player to `all_sprites`
* Every wall to both `walls` and `all_sprites`

---

### 5. Maze Layout

Create a simple maze using multiple wall objects.

**Maze Requirements**

* At least **10 walls**
* Walls form a path the player must move through
* Walls should block the player from moving freely

*Hint:* Hard-code wall positions using `(x, y, width, height)` values.

---

### 6. Collision Detection

* Prevent the player from moving through walls
* Use **sprite collision detection**
* If the player hits a wall, their movement should stop or be undone

---

### 7. Game Loop

Your game loop must:

* Handle events (quit event)
* Get keyboard input
* Update player movement
* Check for collisions
* Draw everything to the screen
* Use `pygame.display.flip()` or `update()`
* Run at a steady frame rate using a clock

---



## Rubric

| Category                           | Points  |
| ---------------------------------- | ------- |
| Player class implemented correctly | 20      |
| Wall class implemented correctly   | 20      |
| Maze layout & wall placement       | 20      |
| Collision detection works          | 20      |
| Game loop & controls               | 10      |
| Code style & comments              | 10      |
| **Total**                          | **100** |


