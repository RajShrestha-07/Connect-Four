# Connect Four

Connect Four is a small web game. Drop discs into a 7-column, 6-row board and try to get four in a row (across, up and down, or diagonal) before the computer does. It keeps count of your wins, losses and draws, highlights the winning four, and alternates who starts each game.

Live demo: https://YOUR-USERNAME.github.io/Connect-Four/

Built with: HTML, CSS and JavaScript.

What this project shows: The computer looks ahead about five moves using minimax with alpha-beta pruning. Minimax tries each move for both players and picks the one with the best outcome, and alpha-beta pruning skips branches that can't beat a move it already found, which makes the search much faster. Connect Four has too many possible games to check them all (unlike tic tac toe), so when the search runs out of depth the code estimates how good a position is. It scores lines of two or three discs and gives a small bonus for the centre column. The board is stored as a grid of rows and columns, and the win check looks in four directions from every disc.

What I'm learning from it: I'm studying how the `search` function uses alpha and beta to skip moves, how `evalBoard` scores a position when the search stops, and how `findWin` checks the four directions.
