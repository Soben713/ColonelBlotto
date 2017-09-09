# ColonelBlotto
An implementation of zero-sum *Colonel Blotto* game with general payoff functions.

Definition of the game from [Wikipedia](https://en.wikipedia.org/wiki/Blotto_game):

> A *Blotto* game, *Colonel Blotto* game, or *divide-a-dollar* game is a type of two-person zero-sum game in which the players are tasked to simultaneously distribute limited resources over several objects (or battlefields). In the classic version of the game, the player devoting the most resources to a battlefield wins that battlefield, and the gain (or payoff) is then equal to the total number of battlefields won.

It was shown by Ahmadinejad et al. [] and [] that the zero-sum version of the game, even for general payoff functions could be solved in polynomial time. This code is an implementation of the algorithm given in []. The payoff function `payoff_a(k, x, y)` returns the payoff of the first player in the `k`-th battlefield if the players put `x` and `y` troops in it respectively. By default, the player who puts more troops in a battlefield gets a payoff of `+1` for that battlefield. You can override the payoff function to be anything.

## Installation
The code is written in JuMP/Julia. See [here for its installation guide](http://jump.readthedocs.io/en/latest/installation.html).

## Citation
You can cite either of the following versions of the paper.
* [arXiv:1612.04029](https://arxiv.org/abs/1612.04029)
* [AAAI'17 Proceedings](https://aaai.org/ocs/index.php/AAAI/AAAI17/paper/view/14980)
