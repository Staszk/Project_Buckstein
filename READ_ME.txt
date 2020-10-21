//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
//  Project_Buckstein | Programmed and Designed by Parker Staszkiewicz, Anthony Pascone, and John Imgrund (c) 2018  				//
//      										     																				//
//  This game was created by three students at Champlain College pursuing the Game Programming major.  The game had   				//
//  to be completed within three weeks and had to utilize both online networking and an AI technique not discussed during   		//
//  the course.  The game uses the RakNet framework for networking, Utility AI, and an original pathfinding algorithm with  		//
//  a D&D-style rulest for movement.							    																//
//										   	                                                                                        //
//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

Project_Buckstein is a co-op tactical strategy game in the style of XCOM.  The object of the game is to work together with
another player to defeat the AI-controlled enemies.

CONTROLS:
* Left Mouse Button: 	Clicking a Player Unit will select it; once a Player Unit is selected, clicking an available tile will cause the 
	                	unit to move to that spot.
						If an Enemy Unit is highlighted to be shot, left clicking it will cause the selected Player Unit to shoot the 
						enemy.
* Right Mouse Button:	Deselects any currently selected Player Unit.
* E Key:				With a Player Unit Selected, E will both show the shoot radius of the selected unit as well as highlight 
						enemies within range.
* T Key:				Opens the chat window and focuses it, allowing players to communicate over network.
						Also closes the window, if it is not in focus and is open.

NOTABLE ISSUES:
* Due to an issue relating to reading packets from RakNet, the networking of Project_Buckstein has some major flaws. Generally,
for any pair of two computers, only one will ever work as the Host.  If you cannot connect on your first try, we recommend changing
who is hosting the game.

In the event that networking issues stops you from seeing how the game is played, you can revert to revision 142 on branch Dev in 
order to "play" a non-networked version of the game.