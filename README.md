1. Project Overview:
This project is a web-based implementation of the popular puzzle game "2048." The objective of the game is to move and combine numbered tiles on a 4x4 grid to reach the tile numbered 2048. The player moves tiles using the arrow keys, and the game ends when no more valid moves are possible. It includes a scoring system, a start/restart button, and messages displaying win or loss states. The game’s interface is designed with simple visuals and smooth interactions, emphasizing a user-friendly experience.

2. Technologies Used:
a. HTML (Hypertext Markup Language):
  The page structure is created using HTML elements, including:
    <!DOCTYPE>, <html>, <head>, <meta>, <title>, <link>, <script>, <body>, <header>, <main>, and <footer>.
    A <table> element is used to represent the 4x4 game grid.
    <button> elements for the "Start" and "Restart" functionality.
    <p> tags to display score and game status messages.
b. CSS (Cascading Style Sheets):
  The visual design and layout are handled using CSS, incorporating:
    Flexbox and Grid Layouts: For centering the game elements and structuring the 4x4 grid.
    Responsive Design: Ensuring the game layout adapts to different screen sizes and resolutions.
    Custom Styling for Tiles: Different colors for each numbered tile (e.g., 2, 4, 8, 16, etc.), background colors, and text styles are applied.
    Animations and Transitions: Smooth transitions for tile movements, hover effects for buttons, and fade-in/out effects for win/loss messages.
c. SASS (Syntactically Awesome Stylesheets):
  SASS is used to organize and enhance CSS styles:
    Nested Selectors: To apply styles for specific states (e.g., .field-cell--2, .field-cell--4).
    Variables and Mixins: Used to create reusable values (e.g., for tile colors and sizes).
d. JavaScript (ES6+):
  Event Listeners & DOM Manipulation: Handles interactions with the game board, including starting/restarting the game, moving tiles, and updating the score.
    Game State Management: Using a Game class to track game progress, score, and status.
    Game Logic: Functions like moveLeft(), moveRight(), moveUp(), and moveDown() to handle the movement and merging of tiles based on the arrow keys pressed by the user.
    Score Calculation: The game tracks the score based on tile merges and updates it dynamically.
    Keyboard Events: Players interact with the game using the arrow keys to control the movement of the tiles.
e. Mutation Observer:
  A MutationObserver is used to track changes in the game grid after each move. It observes the grid and triggers the game logic to check if a move is possible or if the game has ended.

3. Features:
Game Field (Grid):
  A 4x4 grid is dynamically populated with numbered tiles, each with its own color corresponding to its value (e.g., 2, 4, 8, 16, etc.).
  Tiles combine when moved into each other, and the grid is updated accordingly.

Score Display:
  The current score is displayed at the top of the page and is updated as tiles combine.

Start/Restart Button:
  The button toggles between "Start" and "Restart." When clicked, it initializes the game or resets it to start a new round.

Win and Lose Messages:
  Win: Displayed when the player reaches the 2048 tile.
  Lose: Displayed when no valid moves remain, indicating the game is over.
  Start Message: Displayed initially, prompting the user to start the game.

Tile Movement:
  Tiles can be moved and combined in four directions: left, right, up, and down, using the arrow keys.
  As the tiles move, their numbers and colors change according to the rules of the game.

Game Logic:
  The game keeps track of the state, moves, and score using the Game class, which encapsulates the logic of the game, including checking for valid moves, tile merging, and game over conditions.

Dynamic Tile Creation:
  When a move is made, new tiles are created and added to the grid. Their positions and values are dynamically updated.

4. User Interaction:
  Arrow Keys: Players move tiles using the arrow keys (ArrowLeft, ArrowRight, ArrowUp, ArrowDown).
  Start/Restart Button: The game can be started or restarted by clicking the button.
  Responsive Feedback: The game provides immediate feedback to the user, such as updating the score and displaying messages when the game is won or lost.

5. Game Flow:
  The user clicks "Start" to begin the game.
  The game grid initializes with two random tiles.
  The user moves the tiles using the arrow keys, merging matching tiles.
  The score updates as tiles combine.
  The game continues until the player reaches the 2048 tile (win) or there are no more valid moves (lose).
  The user can restart the game at any time by clicking the "Restart" button.

6. Link to preview: