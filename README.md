# Flappy Bird with NEAT Algorithm 
This project involves the creation of the classic Flappy Bird game using Pygame, enhanced with pixel-perfect collision detection and mask handling. Additionally, the project implements a machine learning model using the NEAT (NeuroEvolution of Augmenting Topologies) algorithm to train a neural network that plays Flappy Bird autonomously, aiming to achieve a perfect run.

# Features
Flappy Bird Game: A faithful recreation using Pygame.  
Pixel-Perfect Collision: Uses masks for precise collision detection.  
NEAT Integration: Trains a neural network to navigate the bird through the pipes.  

# Dependencies
pygame: Library for creating games.  
neat-python: Library for the NEAT algorithm.
# Game Components:
## Bird Class
Handles the bird's attributes, movements, and animations:  

jump(): Makes the bird jump.  
move(): Updates the bird's position and rotation.  
draw(win): Draws the bird on the game window with correct animations and rotations.  
get_mask(): Returns the mask for collision detection.  
## Pipe Class
Manages the pipes' positions, movements, and collision detection:  

set_height(): Sets random height for the pipes.  
move(): Moves the pipes leftwards.  
draw(win): Draws the pipes on the game window.  
collide(bird): Checks for collisions with the bird.  
## Base Class
Handles the moving ground:  

move(): Moves the ground to create an endless scrolling effect.  
draw(win): Draws the ground on the game window.  
## Main Game Loop
draw_window(win, birds, pipes, base, score): Draws all game components and updates the display.  
main(genomes, config): Core loop where the NEAT algorithm interacts with the game. Handles bird and pipe movements, collisions, scoring, and neural network decisions.  
## NEAT Algorithm
run(config_path): Sets up and runs the NEAT algorithm for a specified number of generations.  
main(genomes, config): Called by the NEAT algorithm to simulate the game and evaluate the fitness of neural networks. 

# Acknowledgments
Inspired by the original Flappy Bird.  
NEAT Algorithm: NEAT-Python Documentation  
