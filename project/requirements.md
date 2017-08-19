##Unnamed Strategy Game

Johnathan Kimbro, Kristen Wright

_Requirements_

1.	User Interface
	*	Menu Sections  
		Game must provide a startup/setup menu to access saves and create new games.  
		Game must utilize menus for selection of moves within the environment

	*	Game Board  
		Game must generate and simulate a functional "game board".  
		Game board must be scrollable and interactive.

2. 	Data Source
	*	Game data must be stored and saveable to pull data and generate new or preexisting games
	*	Game data will be saved in loadable class-based xml formats.
	*	Game data will be sourced for each play.


3. 	Logic Engine
	*	Game contains a series of rules regarding gameplay as well as automated actions.
		*	Every turn, the logic engine compounds player's new army count and resource count
		*	Game board is procedurally generated using logic boundaries
			*	each board ranges from Small (20x20), Medium(35x20), Large(50x20), Massive(80x20)
			*	Game board structure:  
>Mountain	20%  
>Plains		30%  
>Forest		30%  
>Rocky		20%  
>Water		Generated & Chained Randomly

Game provides resource collection & economy to require players to strategize their gameplay

---

Game development is structured into four interlocking Modules; modules are stackable, meaning each module will provide a new functionality to the overall game

**Module 1: Construction**  

	*	Basic menus, discover new areas, build & collect resources, save game
	*	Create memory management system and data storage (cloud based or pc based)

**Module 2: Battle/Easy Mode**  

	*	Rudimentary hardcoded "computer" enemy, to be used as "easy mode."
	*	Enemy is static and player builds up to defeat it

**Module 3: Enemy AI**  

	*	Adaptive AI for normal-hard-extreme modes that starts at the same level as you.
	*	AI enemy builds up resources and challenges player.

**Module 4: Multiplayer Mode**  

	*	Address testing concerns
	*	Create mode where multiple players can play against each other