Pong Game – Python Turtle Graphics Implementation

This project is a complete recreation of the classic Pong arcade game using Python’s Turtle Graphics module. The game includes two paddles, a bouncing ball, collision detection, scoring logic, and adjustable game speed.
The goal was to build a fully interactive, object-oriented game from scratch while understanding real-time movement, event handling, and class-based game architecture.

The project consists of four components: Paddle, Ball, Scoreboard, and the main game loop that ties everything together.

Key Features
1. Player-Controlled Paddles

Two paddles are created using a custom Paddle class.
Controls:

Right Paddle: ‘p’ = up, ‘l’ = down

Left Paddle: ‘w’ = up, ‘s’ = down
The paddles move vertically in response to keyboard events and stay aligned within the game screen.
(Direction logic handled in paddle.py)

2. Bouncing Ball with Increasing Speed

The Ball class handles:

Movement in both X and Y directions

Wall collisions (top/bottom bouncing)

Paddle collisions (reversing direction + speed boost)

Resetting the ball after a missed hit
(Logic handled in ball.py)

The ball gradually speeds up each time it hits a paddle, increasing difficulty.

3. Score Tracking System

A Scoreboard class displays and updates scores in real time.

Left player score increments when right paddle misses

Right player score increments when left paddle misses

Score is displayed at the top of the screen
(Logic handled in scoreboard.py)

4. Real-Time Game Loop

The main game file controls the entire flow:

Screen setup (size, color, tracer settings)

Listening for keyboard controls

Updating the ball position each frame

Collision detection for walls and paddles

Scoring and ball reset when a player misses
(Main loop handled in pong_game.py)

Game Flow

Game starts with ball moving diagonally.

Players move paddles to keep the ball in play.

Ball bounces off walls and paddles.

If a paddle misses the ball, the opponent scores.

Ball resets to the center and restarts.

Game continues indefinitely until the window is closed.

Conclusion

This project demonstrates core game development concepts using Python, including:

Object-oriented programming

Collision detection

Keyboard event handling

Real-time animation loops

State management and scoring

It’s a fun and interactive project that showcases how simple graphics and logic can recreate a classic arcade experience.
