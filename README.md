# hcs-f20-ml
Additions: Took the existing tic-tac-toe and went off running. 
- Added a hard-coded 4x4 game, the same as 3x3 but with a larger grid.
- Added a general nxn game, where n is some positive integer. This simulates a general grid of numbers on which the model can play against. The time to run noticeably increases with n, of course, especially for n > 5. 
    - Interestingly, the strategy applied in the workshop seems to be less effective as n increases, with winrate decreasing, holding all else equal. Perhaps a higher learning_rate and more trials are required to properly train a model in larger games.
- Future improvements: Build on nxn code to simulate multiplayer tic-tac-toe with p players. Instead of the current code which only has conditions -1 (draw) 1 (loss) and 2 (win), could extend to -1 (draw) and integers i in the range 1-p (each representing i winning).
    - Requires some adjustments to TicTacToe class, specification of hard-coded Opponent (extra attribute).
