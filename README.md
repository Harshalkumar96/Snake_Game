# Snake_Game

# 🐍 Snake Game – Python Turtle Graphics

A classic Snake game built using Python’s built-in `turtle` module. This game allows users to control a growing snake, eat food, and avoid collisions — with both the wall and itself.

---

## 🎮 Game Features

- Responsive controls using arrow keys
- Real-time scoring system
- Randomized food placement
- Collision detection (with food, walls, and tail)
- "Game Over" screen on collision

---

## 📁 Project Structure


snake_game/
│
├── main.py         # Main script to run the game
├── snake.py        # Snake class: controls snake creation, movement, growth
├── food.py         # Food class: handles random food generation
├── scoreboard.py   # Scoreboard class: manages score display and game over


🚀 How to Run
✅ Requirements
Python 3.x (recommended 3.7+)

No external libraries required (uses built-in turtle and random)

▶️ Run Instructions
Clone or download this repository

Open a terminal in the project directory

Run the game with:
python main.py


🧠 Code Walkthrough
main.py
Sets up the game screen (600x600, black background)
Initializes game objects:
-- Snake – player-controlled object
-- Food – randomly placed item the snake eats
-- Scoreboard – displays current score

Handles game loop:
-- Moves the snake forward continuously
-- Detects collisions with food, walls, or the snake’s own body
-- Ends the game if a collision occurs



snake.py
Snake class manages the snake’s:
-- Initial creation with 3 square segments
-- Movement logic (segments follow head)
-- Growth mechanism (on eating food)
-- Directional control (up, down, left, right)
Movement Note: The snake moves in discrete steps of 20 pixels. Direction changes are restricted to avoid 180° turns.



food.py
-- Inherits from Turtle
-- Creates small blue circles as food
-- Randomly repositions food within game bounds on collision with the snake


scoreboard.py
-- Inherits from Turtle
-- Displays score at the top center of the screen
-- Updates score every time food is eaten
-- Displays "GAME OVER" message on collision with wall or tail

