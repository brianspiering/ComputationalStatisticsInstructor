Statistics: A Computational Approach
========

Historically statistics is analytic and theoretically driven.

This is an inverted approach - computational and empirically driven.

----

The goal is to lean on efficient compute and resampling techniques (e.g., bootstrapping and permutation tests) to build statistics from first principles to understand what is going on.

From that firm foundation, be able to solve novel problems.

For example instead of a calculating the probability of dice rolling, let's build a simulator and see what happens.

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