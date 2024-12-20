Two-Player Pygame Chess
Description
This is a simple two-player chess game implemented using Python and Pygame. The game provides a basic chessboard setup, piece movement logic, and a user interface for two players to play chess on the same device. It highlights valid moves for selected pieces and tracks captured pieces during the game.

Features
Two-Player Gameplay: Supports a local two-player chess game.
Valid Move Indication: Highlights valid moves for the selected piece.
Captured Pieces Display: Shows captured pieces on the right side of the screen.
Turn-Based Logic: Alternates turns between White and Black players.
Game Over Detection: Ends the game when one player wins by capturing the opponent's King.
Restart Option: Allows restarting the game by pressing Enter after game completion.
Requirements
Python 3.x
Pygame library
Installation
Install Python 3 from Python's official site.

Install Pygame using pip:

bash
Copy code
pip install pygame
Ensure the assets folder contains the following images:

black queen.png, black king.png, black rook.png, black bishop.png, black knight.png, black pawn.png
white queen.png, white king.png, white rook.png, white bishop.png, white knight.png, white pawn.png
How to Run
Save the script as chess.py.
Place the required assets in an assets folder in the same directory as the script.
Run the script using Python:
bash
Copy code
python chess.py
How to Play
Player Turns: The game alternates turns between the White and Black players.
White starts first.
Selecting Pieces: Click on a piece to select it. Valid moves will be highlighted.
Moving Pieces: Click on a highlighted valid move to move the selected piece.
Capturing Pieces: If a piece lands on a square occupied by an opponent’s piece, the opponent's piece is captured.
Checkmate Detection: The game highlights the King if it is under attack.
Forfeiting the Game
Click on the FORFEIT button to forfeit the game.
Restarting the Game
After the game ends, press Enter to restart.
Code Overview
Game Initialization: Sets up the display, fonts, and initial variables for gameplay.
Piece Movement and Logic:
Functions such as check_pawn, check_rook, check_knight, etc., determine valid moves for each piece.
Drawing Functions:
draw_board(): Draws the chessboard and turn status.
draw_pieces(): Renders pieces on the board.
draw_valid(): Highlights valid moves.
draw_captured(): Displays captured pieces.
Game Loop: Handles the game’s main logic, including turn management and event handling.
Game Over: Ends the game when the King is captured and provides the option to restart.
Known Issues and Limitations
Piece Promotion: Pawn promotion is not implemented.
En Passant and Castling: Advanced chess rules like en passant and castling are not supported.
AI: No single-player or AI opponent is implemented.
Graphics: Basic visuals, with no animations for piece movement.
Future Enhancements
Implement AI for single-player mode.
Add support for advanced chess rules like castling, en passant, and pawn promotion.
Improve graphics and animations.
Add sound effects for moves and captures.
