# Tennis

This Kata is about implementing a simple tennis game scoring system. For this kata you will have to write a class that takes scoring of two players and can output a running score at any time.

1. A game is won by the first player to have won at least four points in total and at least two points more than the opponent.
2. The running score of each game is described in a manner peculiar to tennis: scores from zero to three points are described as “love”, “fifteen”, “thirty”, and “forty” respectively.
3. If at least three points have been scored by each player, and the scores are equal, the score is “deuce”.
4. If at least three points have been scored by each side and a player has one more point than his opponent, the score of the game is “advantage” for the player in the lead.

## Extra #1

If you haven’t yet, add the “Player 1 wins” and “Player 2 wins” cases.

## Extra #2

Add set scoring. A set is won if a player wins at least 6 games by a margin of 2.

## Extra #3

Add match scoring. A match is won if a player wins a predefined number of sets given by an extra argument, for example “best of 3” or “best of 5”.
