How to use:
Run pychess.py with Python 3
All the instructions you need to play the game are included in the help section, which is printed upon running it!
All edge cases are covered, and the rules are as described in the help section. I put all my documentation in the help section so that you can read it while playing the game.

The chess engine is a simple minimax algorithm with pruning that searches through the moves, where board positions are ranked in order of the sum of the chess pieces' values. (Pawn=1,Bishop=Knight=3,Rook=5,Queen=9,King=Infinity)

The help section reads as follows:

PYCHESS:
    Welcome to Pychess, created by Ryan Burgert
    on planet Earth, Milky Way Galaxy, 2018.

    In this game, you play a chess game against an AI.
    There are a few differences in the rules between
    normal chess and the chess in this game, though.
        1. En-Passant and Castling are not allowed
        2. You are allowed to put yourself in check 
        3. There are no stalemates
        4. Pawns always promote to queens
        5. In order to win the game, you 
           must capture your opponent's king
        6. You always play white

    Special commands:
        1. "HELP" - brings up this menu
        2. "AUTO" - lets the AI make one move for you
        3. "L1"   - sets the AI to level 1
        4. "L2"   - sets the AI to level 2
        5. "L3"   - sets the AI to level 3
        6. "L4"   - sets the AI to level 4
        7. "L?"   - display current AI level
        8. "abcd", where a, b, c, and d are digits 
            between 1 and 8, inclusively - 
            Moves a piece from square (a,b) to square (c,d), 
            where coordinates (x,y) represent the positions
            of each square on the board. 
            EXAMPLE: To move your king's pawn two forward on 
            the first turn, you would enter "5254"
        9. The up/down arrow keys let you scroll
            through commands, for the sake of 
            convenience.
        10. "FLIP" - Flips the board visually.
            You still play white, though.
            This is useful for comparing 
            pychess to other chess engines.
        11. "SAVE *" - Saves the current game state to path *
            EXAMPLE: "SAVE test.txt"
        12. "LOAD *" - Loads the current game state from path *
            EXAMPLE: "LOAD test.txt"
        13. "EXIT" - Exits the game

    Other Notes: 
        • Commands are not case sensitive
        • Saved games include the ai level, and the sequence of
            moves since the beginning of the game. In other words,
            the UNDO command will work immediately after loading a game.
        • Immediately after you make a move, the chess board with
            that move (before your opponent makes their move)
            will be displayed in yellow
        • Your terminal must be capable of rendering unicode
            chess characters to display this game properly.
        • The AUTO command will make a move for you using the same
            AI level as your opponent AI, which will move immediately
            afterwards. This prevents cheating, as this function 
            is really meant to see how the AI thinks when playing 
            against itself.
