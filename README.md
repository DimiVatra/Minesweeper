# Minesweeper
Minesweeper for Arduino Mega, display LCD TFT 2.4''

Game Rule:
	After first click on a block, 9 mines will be randomly generated.
	The number appears at a opened block indicates how many bombs
	are in adjacent blocks. Try to open safe blocks. Flag blocks you think
	are with bombs. Put a "?" on the block you are not sure about.
	Lose Condition: Any block with bomb is opened.
	Win Condition: When all blocks without a bomb are opened.

Special game designs:
	1,On the left side of screen is a score panel, it shows how many blocks your
	flagged, and how many "mines" are left based on your flags.
	2,The timer will start to count your time after first click, and stops
	when you lose or win.
	3,The Core algorithm: "fast open", when opening a block, if it is a block
	with 0 bombs around, then it will automatically open the blocks around it.
	And if any of the opened 8 adjacent blocks have 0 mines around, then its
	adjacent blocks will recursively open as well.
	4,flag block and "?"block.
	5,All mine will be displayed when lose.

Game Control:
	At the welcome screen, touch to start a new game.
	Use the joystick to move cursor to select a block.
	Use the touch to open a block.
	Push down the pushbutton to:
	1, To flag a block.
	2, If it is already flagged, it will become a questionmarked block.
	3, If already questionmarked, it will back to original state.
	After win, or lose, also touch the screen to restart.
