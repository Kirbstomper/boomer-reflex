# Boomer-Reflex

Inspired by games like Frozen Synapse and Toribash (and on some level mystery dugeon games), people have long argued that fighting games are inacessable at large due to complicated inputs, something that I think has been fixed by games that provide simple input methods such as rising thunder, grandblue fantasy, and smash. Simple design via something like divekick and footsies. But some people still view the genre as having reaction time as just a ridiculous barrier to entry. Lets change that and have fun doing it

# Framedata
Most fighting games run their game logic and visually at 60 "Frames Per Second" (FPS will be used to refer to this, not "first person shooter") In a fighting game when you press a button to use a move it takes a certain amount of frames to execute from start to finish. A move have 3 distint parts

Startup - The part of the animation where the move is not actually hitting an opponent yet. Think of it like winding up a punch

Active - This is the part of a move that actually hits the opponent. Think of it like the punch being extended

Recovery - While startup was winding the punch, this is your arm coming back after a punch. or resting after taking an action,

Each of these parts has an amount of frames associated with it, totallying out to the framecount for a move. 


In addition to moves having frame data for coming out, they also have framedata for what happens on hit such as how many frames someone is in hitstun, this is what allows combos to be possible. You use a move that provides enough hitstun that you can hit them again while they are not able to do anything.

# Gameplay

The idea here is that players can select an action (moving their character, pressing a button, or using a special move) and have it executed at the same time to update the gamestate frame by frame. If a player is in recovery they will not be able to act out of it, so commit wisely.

If a player is hit, both players will be reset to starting position, with the character who took damage losing health.

A player will be able to move left, right, and crouch to block low
A player will also be able to jump
A player will have 3 buttons to use (light, medium, heavy)
A player will have 1 button as a character action (Fireball, DP, Rekka, etc) We keep it simple.

Hit your oponent, don't get hit



