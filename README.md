A Computational Take on Statistics
========

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/brianspiering/statistics_a_computational_appoarch/master)

Historically, statistics has been analytic and theoretically driven.

This is an inverted approach - computational and empirically movtivated.

----

The goal is to leveage efficient compute and resampling techniques (e.g., bootstrapping and permutation tests) to build statistics from first principles. Use that new foundation to solve novel problems.

For example instead of a calculating the probability of dice rolling, let's build a simulator and see what happens:

```python
from random import choices

# Traditional die: A cube
n_sides = 6

# Roll a die
choices(population=list(range(1, n_sides+1)))

# Roll 2 dice
roll_2_dice = (lambda: choices(population=list(range(1, n_sides+1)),
                      k=2))
roll_2_dice()
```
