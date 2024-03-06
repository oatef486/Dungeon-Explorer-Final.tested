# Dungeon Explorer

**Code from the AMS Advanced Python course**

# Authors:

1- Omar Saleh -Matriculation number: 3120009
2- Jonathan Estephan -Matriculation number: 3119742
3- Ibrahim Khalil -Matriculation number: 3119779
4- Abdullah Aljamal -Matriculation number: 3107686

# game_logic.py

\*\* new classes added:
1- lightning
2- undead

\*\* variables:
1- fountain
2- all_coins_collected
3- shock

\*\*events:
1- "collect all coins to access the door"

\*\*functions:

1- move_command:
-In move_command function, we added the shock variable; which has the same functionaloty as the fireballs, but causes -2 damage(check in the update function)
-we added the all_coins_collected variable, so that the player must collect all coins to proceed further to the next level

2- get_objects:
-In get_objects function we added variables for lightning(l), undead(u), skeleton(s), fountain(n)

3- update:
-In update function we implemented the same functionality for the lightnings as for the fireballs
-we added 2 more for loops for the undeads and skeletons
-we also made the fountain, so that it is used for shelter by the player and the monsters can't go through it

- we also made the monsters unable to go through the doors, because that caused a bug sometimes, when a monster is on the same position as the door and the player walks into it too

4- start_level:
-In start_level function we added 4 new paramters for the lightnings, undeads, skeletons and fountains
-we assigned U for undead, S for skeleton and F for fountain

# graphics_engine.py

-we added a new function (print_instructions), which simply prints the instructions for the game once the code runs
-we added new soundtracks for when a level is passed, when the player dies and when all levels are cleared
-All new soundtracks are composed specifically for this project by a friend of ours

# levels.py

-we added 2 more levels making the total levels number 5, we used generate_maze.py file

\*\*we formatted all files using black

## Links:

- https://github.com/krother/ams_dungeon_explorer
- [Opengameart](https://opengameart.org/) - graphics and music for your own games

## we used chatgpt for some debugging issues we faced

## we got the lightning graphics from opengameart

## we faced an issue when we tried running the code on windows, that being the speed of the monsters might be too fast, to tackle this issue just add more waits in the update functions
