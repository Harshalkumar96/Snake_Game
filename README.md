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
│<br>
├── main.py         # Main script to run the game<br>
├── snake.py        # Snake class: controls snake creation, movement, growth<br>
├── food.py         # Food class: handles random food generation<br>
├── scoreboard.py   # Scoreboard class: manages score display and game over<br>


🚀 How to Run<br>
✅ Requirements<br>
Python 3.x (recommended 3.7+)

No external libraries required (uses built-in turtle and random)<br>

▶️ Run Instructions<br>
Clone or download this repository<br>

Open a terminal in the project directory<br>

Run the game with:<br>
python main.py<br>


🧠 Code Walkthrough<br>
main.py<br>
Sets up the game screen (600x600, black background)<br>
Initializes game objects:<br>
-- Snake – player-controlled object<br>
-- Food – randomly placed item the snake eats<br>
-- Scoreboard – displays current score<br>

Handles game loop:<br>
-- Moves the snake forward continuously<br>
-- Detects collisions with food, walls, or the snake’s own body<br>
-- Ends the game if a collision occurs<br>



snake.py<br>
Snake class manages the snake’s:<br>
-- Initial creation with 3 square segments<br>
-- Movement logic (segments follow head)<br>
-- Growth mechanism (on eating food)<br>
-- Directional control (up, down, left, right)<br>
Movement Note: The snake moves in discrete steps of 20 pixels. Direction changes are restricted to avoid 180° turns.<br>



food.py<br>
-- Inherits from Turtle<br>
-- Creates small blue circles as food<br>
-- Randomly repositions food within game bounds on collision with the snake<br>


scoreboard.py<br>
-- Inherits from Turtle<br>
-- Displays score at the top center of the screen<br>
-- Updates score every time food is eaten<br>
-- Displays "GAME OVER" message on collision with wall or tail<br>

-- Play Image<br>
![image](https://github.com/user-attachments/assets/1a35f369-f29e-4bda-8cc1-9245c0b49c58)
<br>
🛠️ Built With<br>
🐍 Python 3<br>
📦 Turtle Graphics (standard library)<br>
🎲 Random module<br>
⭐️ Like this project?<br>
Consider giving it a ⭐ on GitHub and feel free to fork and modify it!<br>
