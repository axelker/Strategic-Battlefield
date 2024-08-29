# Strategic Battlefield
Strategic Battlefield is a tactical game where players navigate a grid-based map containing combatants, obstacles, and various elements such as bombs and mines. The objective is to strategically position your units and utilize the elements on the battlefield to defeat your opponent.
This project is part of a design methods module that aims to apply and enhance object-oriented programming skills and the use of various design patterns, including Logger, Composite, Adapter, proxy and Strategy

## Functionalities
The game board is a configurable grid defined in the Constante class. It consists of two maps:

A map containing different combatants with their coordinates as keys.
A map containing various board elements (Bombs, Mines, Walls, Pellets) with their coordinates as keys.
### Each combatant has distinct characteristics:

- Tank (T): Deals heavy damage but has a short-range weapon and costly movements. Shield activation is prioritized due to its low cost.
- Elite (E): Has light, low-cost movements with a long-range, high-damage weapon. However, using the shield is expensive.
- Soldier (S): Balances between the Tank and Elite, with moderate attributes.
- RandomCombatant (R): Has randomly assigned attributes for all characteristics.
Each combatant also has a specific view that represents their state and actions on the grid.

### Board elements include:

- Bomb (B)
- Mine (M)
- Wall (*)
- Empty spaces
- Pellet (p)
### Game Strategies:

Combatants can choose between a random strategy or a more calculated approach using a refined strategy.
The board uses a semi-random strategy (strategyPlateauAlea) to place combatants and elements, prioritizing empty spaces to avoid overcrowding with walls.

## Game Execution:
The game progresses with a "Next" button, allowing players to advance through each phase of the battle in a controlled and sequential manner.


## Run Instructions
To run the game, follow these steps:

### Using Apache Ant (if installed):
1. Open a terminal at the root of the project directory.
2. Execute the ant command, which will run the build.xml file. This command will:
- Create necessary directories.
- Generate Javadoc.
- Compile .class files and other necessary artifacts.

### Alternative Method:
- Run the script ./compilation.sh in the terminal.
This script will manually compile the necessary files to run the game.
