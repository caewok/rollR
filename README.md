
# rollr

<!-- badges: start -->
<!-- badges: end -->

The goal of rollr is to provide a simple way to make complicated dice rolls using syntax inspired by tabletop roleplaying games.

## Installation

Not yet

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(rollr)

roll("3d6")
roll("2d20h1")
```

## Dice roll syntax

Features list taken from [Sidekick](https://github.com/ArtemGr/Sidekick)


- [ ] `/r 1d8 + 4d6` - Roll one octahedron and four hexahedrons.

- [ ] `/r 1d20+5 # Grog attacks` - Roll dice with a comment.

- [ ] `/r 2d6>=5` - Roll two hexahedrons and take only the ones that turned greater or equal to five (aka difficulty check). Prints the number of successes.

- [ ] `/r 4d6=5` - So can this guy roll five?

- [ ] `/r 3d10>=6f1` - oWoD roll: rolling *one* is a failure, rolling more failures than successes is a *botch*.

- [ ] `/r 1d10>=8f1f2` - Rolling *one* or *two* is a failure.

- [ ] `/r 4dF` - [Fudge/Fate dice](http://rpg.stackexchange.com/questions/1765/what-game-circumstance-uses-fudge-dice).

- [ ] `/r 3d6!` - Exploding dice.

- [ ] `/r 1d10!>9` - Explode nine and ten.

- [ ] `/r 1d20r1` - Roll twenty, reroll on one (because halflings are lucky).

- [ ] `/r 3d10!>=8` - nWoD roll: tens explode, eights and up are treated like a success.

- [ ] `/r 1d10t10` - If a ten is rolled then count it [twice](https://github.com/ArtemGr/Sidekick/issues/151).

- [ ] `/r 2d20k1` - Roll twice and keep the highest roll (D&D 5e advantage).

- [ ] `/r 2d20k1 + 2` - Roll twice and keep the highest roll, with a modifier (D&D 5e advantage).

- [ ] `/r 2d20kl1` - Roll twice and keep the lowest roll (D&D 5e disadvantage).

- [ ] `/r 4d6k3` - Roll four hexahedrons and keep the highest three (D&D 5e ability roll).

- [ ] `/r repeat (4d6k3, 6)` - Roll D&D 5e ability score six times (to generate a new character).

- [ ] `/r repeat (d6, 3, brief)` - In Nomine. 1, 1, 1.

- [ ] `/r repeat (1d20+1, 5, short sum)` - Sum the rolls.

- [ ] `/r ova (5)` - OVA. 6, 6, 1, 1, 1 = 12.


