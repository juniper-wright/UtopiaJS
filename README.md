UtopiaJS
========

JavaScript version of the Utopian Engine

Version 3.0 of the [Utopian Engine](https://github.com/phoenixfyre/UtopianEngine) was supposed to feature the following:

* Porting the Engine to JavaScript, running as an SPA.
* Improved JavaScript handling - the ability to affect UtopianEngine state variables

I decided that the two projects are dissimilar enough (100% Java -> 100% JavaScript!) to warrant a separate repository.

So, like Version 2.0 of the Utopian Engine, UtopiaJS will feature the following:

A text adventure game engine, written in Java.

Version 2.0 of the Utopian Engine features:

* A fully-fledged built-in Scripting Language, named UtopiaScript. At this time, the UtopiaScript functions are:
	* Print - Print a string to the player's console
	* Println - Same as Print, but with a trailing endline
	* Pause - Pauses the game's operation until the player presses enter
	* Description - Prints out a predefined description for the room the user is in
	* RequireItem - Require that the player possess one or more of an item to continue
	* AddItem - Give the player one or more of an item
	* TakeItem - Take one or more of an item from the player
	* RoomState - Change the state of any room to one of a predefined list of states for that room
	* GoTo x y- Send the player to any room in the game
	* Go x/y - Send the player to x rooms horizontally, and y rooms vertically (can be negative)
	* Score - Modify the user's score
	* LoadGame - LOAD A NEW GAME. Basically, I put this in for episodic gaming. More on this later.
	* QuitGame - Ends the game. Used to denote winning or losing, or just quitting. The Engine does not discriminate.
	* Inventory - Prints the user's inventory.
* JAVASCRIPT! Yes, the Utopian Engine supports JavaScript, and makes the user's input available to JavaScript for dynamic event-handling. With a bit of finagling, it is possible to make an RPG. Since the entire Engine will be in JavaScript, this will be MUCH more robust.
* Two-dimensional array of Rooms, each of which can be completely independent of one another, or modify one another
* Each Room has a list of Roomstates - when certain actions happen, developers can script the rooms to change, subtly or otherwise. Basically everything changes about the room when its state changes.

In addition to the features in the Utopian Engine v2.0, UtopiaJS will feature:

* The ability to upload games, and the server will keep a record of recent/popular games.
* The ability to author games directly from your browser.
