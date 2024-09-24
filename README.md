# **Skittter-Snacks**
Skitter Snacks is a game jam project about a jumping spider attempting to steal doritos from ants. Created for the online "2022 PIGSQUAD Summer Slow Jam", over 12 days, with a focus on "Stealth" gameplay mechanics. I worked alongside 4 other talented developers for this project. 

![Title_Screen](https://github.com/user-attachments/assets/95587d44-83e6-4471-852f-18cd7ef0836a)


## Game Mechanics
The core gameplay loop of Skitter Snacks involves the player spider ducking and weaving between the ant's patrol paths while attempting to steal the doritos spread around the map. The player spider has a unique ability; being able to jump across the map by holding space bar. This enables them to avoid the ant's gaze and run away when spotted. Several key game mechanics are required to enable this game loop to function:

- AI system that chases the player when they are within line of sight.
- Unique "Jump" ability of the Player Spider to allow them to remove themselves from line of sight of the enemy Ant AI.
- Phermones released from the doritos that enable the player to spot the Doritos on the map and steal them.
- Dynamic audio track that updates as the player is continuously spotted by enemy Ants, until they begin their chase.

![Starting_Bottle](https://github.com/user-attachments/assets/4f04ba42-804b-45ae-a868-0328cc927378)

## My Contributions
I primarily worked upon the AI system for Skitter Snacks, as well as UI implementation, Audio Manager and several other gameplay mechanics. 

### AI
- State Machine design and implementation, to allow the AI to chase the player and return to patrolling when finished.
- Line of Sight system, allowing player to be spotted only within a specific view cone of the AI.
- Phermones system to inform other nearby ants of the player's position, to try and catch the player offguard.
- Navmesh implementation allowed the ants to move across most surfaces using NavLinks, so the chase can continue.

### UI
- Implemented global UI manager to allow for UI to update as more doritos are eaten and to update player's spotting indicator in the bottom right corner.
- Implemented billboarded sprites that update based on state of the AI.
  - Red:    AI has spotted the player and is actively chasing them
  - Orange: AI has spotted the player, but not yet chasing them
  - White:  AI has not spotted player and is currently patrolling as usual

### Audio 
- Implemeted Audio Manager to enable dynamic music control based on gameplay triggers.

## Links
- Link to the project on itch.io: https://bunnyufo.itch.io/skitter-snacks (I am Aculater58 in the credits, Web Build can potentially break the game, would recommend playing the build locally instead) 
- Link to the Gamejam Entry: https://itch.io/jam/ssjstealth/rate/1627291 
- Link to EXE download: https://drive.google.com/drive/folders/14eaOc_5DD9jxakztT3VzHbz7hy25LKin?usp=share_link.
  
The controls for the game are: Moving - WASD, Hold spacebar to jump (Line indicates where you jump to). 
