# Dice_Battle

A game theory simulation based on mixed strategies, uses linear and dynamic programming in order to solve the game. Built with Python and Dash by Plotly.

Two players meet in a game of dice. The goal is to be the first to reach at least N points (usually N = 100). On each turn, we choose to roll between 1 and D six-sided dice (for example, D = 10). The number of points scored is 1 if at least one of the dice falls on 1, otherwise it is the sum of the dice. We are going to study two variations of this game:

* sequential variant: the players take turns (the first player therefore has an advantage).

* simultaneous variant: players play each round simultaneously. In this case if both players reach N points or more in the same round, it is the player who exceeds the N points the most who wins; if both players get the same score, then they are tied.

The goal of the project is to determine an optimal game strategy (and to test this strategy against others). We say that a player has a payout equal to 1 if he wins the game, a payout equal to 0 if the game is a draw, a payout equal to -1 if he loses. So it is in particular a zero sum game.

The coded version in this work is the simultaneous version, it uses Gurobi as a linear solver.

<iframe width="852" height="480" src="https://www.youtube.com/embed/1BZs011gLbU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
