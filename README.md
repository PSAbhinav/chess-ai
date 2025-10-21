Chess
A simple chess game implemented in Python using the Pygame library.
It features a basic AI that calculates the optimal move by peeking DEPTH moves ahead. The AI assesses positions and scores only.

<!-- (Optionally replace this video link with your own preview or remove it) -->
Introduction
This is a basic implementation of a chess game with a graphical user interface. The game allows two players to make moves on a standard chessboard. Additionally, there is an AI opponent that uses negamax algorithm and alpha-beta pruning for move selection.

Features
Graphical User Interface:

The game features a user-friendly graphical interface developed using the Pygame library.

Two-player Mode:

Play against a friend in human vs. human gameplay. Enjoy the classic chess experience with two human players.

AI Opponent:

Challenge yourself against an AI opponent equipped with the negamax algorithm and alpha-beta pruning. The AI has options to make valid moves, providing a single-player chess experience.

Checkmate, Stalemate, and Legal Moves:

The game checks for conditions such as checkmate, stalemate, and legal moves, ensuring a fair and rule-compliant gameplay experience.

Advanced Chess Mechanics:

Supports advanced chess mechanics, including pawn promotion, en passant, and castling for a more strategic and engaging experience.

Undo and Reset Board:

Press Z for undo, R for reset.

Variety of Chess Boards:

Enjoy playing on different chess board colors, adding a personalized touch to your gaming experience.

Immersive Sounds and Images:

Enhance your gaming experience with multiple piece move or capture sounds.

En Passant
In chess, the en passant rule allows a pawn to capture an opponent's pawn that has moved two squares forward from its starting position. The capturing pawn moves to the square immediately beyond the captured pawn.

Optionally add your own images here to illustrate the rule.

Pawn Promotion
In chess, pawn promotion occurs when a pawn reaches the eighth rank. The pawn can be promoted to any other chess piece (except a king).

Optionally add your own images here to illustrate pawn promotion.

How to Play
Clone the repository to your local machine:

bash
git clone https://github.com/PSAbhinav/chess-ai.git
cd chess-ai
Install the required dependencies:

bash
pip install pygame
Run the main.py script to start the game:

bash
python main.py
Using Visual Studio Code:

Open Visual Studio Code.

Click on "File" → "Open Folder" and select the cloned directory.

Open the integrated terminal in Visual Studio Code.

Run the following command to start the game:

bash
python main.py
Controls
The controls for the chess game are designed to be intuitive and user-friendly.

Selecting a Piece:

Click on the chess piece you want to move. The selected piece will be highlighted to indicate that it's ready for a move.

If AI is thinking, you can click on an AI piece to see all possible moves.

Moving a Piece:

After selecting a piece, the legal moves for that piece will be highlighted on the chessboard.

Click on one of the highlighted squares to move the selected piece to that position.

All chess rules, including legal moves, capturing, pawn promotion, en passant, and castling, are handled automatically.

Settings for AI
Human vs Human Gameplay
If you want to play a game where both players are human, open the main.py file and set:

python
SET_WHITE_AS_BOT = False
SET_BLACK_AS_BOT = False
To flip the board for black, go to engine.py and set:

python
self.playerWantsToPlayAsBlack = False
AI Gameplay
If you want to play a game with the AI, open the main.py file and set:

python
SET_WHITE_AS_BOT = True
SET_BLACK_AS_BOT = False
To flip the board for black, go to engine.py and set:

python
self.playerWantsToPlayAsBlack = False
DEPTH
The DEPTH setting determines how many moves ahead the AI will consider during its search for the best move. A higher depth generally results in a stronger AI, but it also requires more computational resources.

For best performance, keep DEPTH at 4 or below.

If you'd like to change the depth, open the chessAi.py file and edit:

python
DEPTH = 3
Acknowledgments
Special thanks to the Pygame library for providing a straightforward and effective means to develop graphical applications in Python.

Contributions and Feedback:
This project is open to contributions from the community. If you have ideas, want to report issues, or suggest improvements, feel free to contribute on GitHub. Your input is valuable in enhancing the overall quality and functionality of this chess engine.

Project maintained by PSAbhinav.
