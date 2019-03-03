# Distributed Scrabble

The system implements a simplified version of the classic Scrabble game in which 2 or more players
play over a 20x20 grid to form words that can only be either horizontal (from left to right) or vertical
(from top to bottom).

The basic drill of the game will be explained with an example using 3 players:

  1) Active player’s turn: Player 1 begins, players 2 and 3 wait. During his turn, player 1 can place
  any of the English characters in any free cell on the board. He then chooses if he wants to get
  credit for either the horizonal or vertical word formed and submits his move.

  2) Voting for getting credit: After player 1 submits his move, players 2 and 3 vote to determine
  if the word that player 1 is claiming is a valid word. If all players vote “yes”, player 1’s score
  increases according to the length of the word. If any player votes “no” no credit is given but
  the player’s 1 move is kept on the board. After voting, player 1’s turn ends and player 2
  repeats the process from step 1.

  3) Ending the game: During each turn, the active player can alternatively “Pass” to indicate that
  he has no valid move. The game will end when all 3 players pass in sequence and the player
  with the highest score wins the game.
