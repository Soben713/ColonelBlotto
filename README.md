# An Algorithm to Find Colonel Blotto Game's Best Strategies
An implementation of zero-sum *Colonel Blotto* game with general payoff functions.

Definition of the game from [Wikipedia](https://en.wikipedia.org/wiki/Blotto_game):

> A *Blotto* game, *Colonel Blotto* game, or *divide-a-dollar* game is a type of two-person zero-sum game in which the players are tasked to simultaneously distribute limited resources over several objects (or battlefields). In the classic version of the game, the player devoting the most resources to a battlefield wins that battlefield, and the gain (or payoff) is then equal to the total number of battlefields won.

It was shown by [Ahmadinejad et al.](https://arxiv.org/abs/1603.00119) (AAAI'16) and [Behnezhad et al.](https://arxiv.org/abs/1612.04029) (AAAI'17) that the zero-sum version of the game, even for general payoff functions could be solved in polynomial time. This code is an implementation of the algorithm given by [Behnezhad et al.](https://arxiv.org/abs/1612.04029)

The payoff function `payoff_a(k, x, y)` returns the payoff of the first player in the `k`th battlefield if the players put `x` and `y` troops in it respectively. By default, the player who puts more troops in a battlefield gets a payoff of `+1` for that battlefield. You can override the payoff function to be anything.

## Installation
The code is written in JuMP/Julia. See [here for its installation guide](http://jump.readthedocs.io/en/latest/installation.html).

## Citation
You can cite the conference version of the paper:

```
@inproceedings{DBLP:conf/aaai/BehnezhadDDHS17,
  author    = {Soheil Behnezhad and
               Sina Dehghani and
               Mahsa Derakhshan and
               MohammadTaghi Hajiaghayi and
               Saeed Seddighin},
  title     = {Faster and Simpler Algorithm for Optimal Strategies of Blotto Game},
  booktitle = {Proceedings of the Thirty-First {AAAI} Conference on Artificial Intelligence,
               February 4-9, 2017, San Francisco, California, {USA.}},
  pages     = {369--375},
  year      = {2017},
  crossref  = {DBLP:conf/aaai/2017},
  url       = {http://aaai.org/ocs/index.php/AAAI/AAAI17/paper/view/14980},
  timestamp = {Mon, 06 Mar 2017 11:36:24 +0100},
  biburl    = {http://dblp.dagstuhl.de/rec/bib/conf/aaai/BehnezhadDDHS17},
  bibsource = {dblp computer science bibliography, http://dblp.org}
}
```
You can also find the paper on [arXiv:1612.04029](https://arxiv.org/abs/1612.04029).
