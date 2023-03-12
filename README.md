Light's Out

The Three Components:

1. App
	- Primary component to do in the root div.
2. GameBoard (or just Board)
	- This will be/hold the grid of lights.
	- Game state will be held here.
	- Function here that gets passed to each child
		- When a cell is clicked, it's x, y get passed into this function which determines which nearby cells are affected, sets their values, then rerenders the whole board.
3. Light (Or cell)
	- This is an individual game piece the player will click on.
	- Props:
		- Lit or not; boolean
		- location in the grid: array of [x, y]