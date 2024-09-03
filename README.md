Demo of the Project:
https://drive.google.com/file/d/1CkwH7ysWAnmX2EBG0e2M6miFZp5h6No6/view?usp=sharing

Turn Based Chess Like Game
This is a turn-based game similar to chess, played on a 5x5 grid. There are two players, each controlling a team of 5 characters: 3 Pawns and 2 Heroes. The server is built with Node.js, and WebSocket is used for real-time communication. The client interface uses plain HTML, CSS, and JavaScript.

Characters and Moves:
Pawns (P1, P2, P3):
  Move one block in any direction: Left, Right, Forward, or Backward.
  Move commands: L (Left), R (Right), F (Forward), B (Backward).

Hero1 (H1):
  Moves two blocks straight in any direction.
  Can defeat any opponent's character in its path.
  Move commands: L (Left), R (Right), F (Forward), B (Backward).

Hero2 (H2):
  Moves two blocks diagonally in any direction.
  Can defeat any opponent's character in its path.
  Move commands: FL (Forward-Left), FR (Forward-Right), BL (Backward-Left), BR (Backward-Right).

Game Flow:
  Setup: Players place their characters on their starting rows.
  Turns: Players take turns moving one character per turn.
  Combat: If a character moves to a space with an opponent's character, that character is removed from the game.
  Winning: The game ends when one player has eliminated all of the opponent's characters.

Setup Instructions and Prerequisites:
Node.js must be installed.

Installation:
 **1. Clone the repository:** git clone https://github.com/your-username/chess-like-game.git
  **2. Go into the Directory:** cd chess-like-game
  **3. Install dependencies:** npm install

Running the Project:
  1. Start the server:
     node server.js
  2. Open the game in a browser:
     Go to http://localhost:8080 to play the game.

Playing the Game:
  1. Click a character to select it.
  2. Click a move direction to move the character.
  3. Move history and captured characters will be shown below the game board.

Project Structure:
  1. server.js: Handles the game logic, WebSocket communication, and game state on the server side.
  2. public/index.html: The main HTML file for the game interface.
  3. public/script.js: Handles game interactions and communication with the server.
  4. public/style.css: (Optional) For custom styles.
