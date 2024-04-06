# Megayahtzee
Over-complicated and extremely exaggerated version of one of my favorite dice games, Yahtzee, developed in Javascript. Rather than five 6-sided dice, you now play with seven 7-sided dice. There are new rolls to attempt to achieve in this version, can you score them all? 
Published on my site. You can play it online here: https://starke.gg/programming/games/megayahtzee

## Objective
Similar to traditional Yahtzee, the objective for Megayahtzee is to maximize your total score through trials of rolling/rerolling dice such that the values on the dice align with a particular set. Within Megayahtzee scoring, there are four possible rankings to achieve:

| Ranking | Points | Description |
| ----------- | ----------- | ----------|
| ★ | 1500 - 1749 | Demonstrates a solid grasp of game mechanics and strategy. |
| ★★ | 1750 - 1874 | Excellent, requires careful planning and risk management. |
| ★★★ | 1875 - 1999 | Perfect, displays incredible precision and strategic genius. |
| ★★★★ | 2000+ | Virtually impossible, unfathomable probability analysis. |

## Rules
You are given seven 7-sided dice. In each round, you may roll the dice up to 4 times. After each roll, you may select which dice you want to keep static (don't want to reroll) and reroll the other dice. Alternativly, you can opt to accept the score for a particular set. After four rolls, you must accept a score for a set (even if it that provides no points). Once you've accepted a score for a particular set, that score for that set is final and you can no longer select that set. The game ends after 34 rounds (since there are 34 sets) when the scores for all sets have been finalized.

## Scoring
### Basic Tallies (Upper Level)
| Set | Description | Points |
| ----------- | ----------- | ----------|
| Aces | Count and add only Aces | Sum of all Aces |
| Twos | Count and add only Twos. | Sum of all Twos |
| Threes | Count and add only Threes. | Sum of all Threes |
| Fours | Count and add only Fours. | Sum of all Fours |
| Fives |  Count and add only Fives. | Sum of all Fives |
| Sixes | Count and add only Sixes. | Sum of all Sixes |
| Sevens | Count and add only Sevens.| Sum of all Sevens |

If the total of all the points from this is equal to 112 points or greater, then a bonus of 75 points will be added to the player's score.

### Common Combos
| Set | Description | Points |
| ----------- | ----------- | ----------|
| 4 of a Kind | Four dice of the same number. | (8 × Dice in 4-of-a-Kind) + Extras of the same Number|
| 5 of a Kind | A set where there are 5 dice with the same value | (10 × Dice in 5-of-a-Kind) + Extras of the same Number|
| Full House | Three dice of the same number and two dice of the same (different) number. | 25 |
| Small Straight | Sequence of four consecutive numbers. | 30|
| Large Sraight | Sequence of five consecutive numbers.| 40 |

### Wildcard Scores
| Set | Description | Points |
| ----------- | ----------- | ----------|
| Whatever | Any arbitrary set of dice | Sum of all dice values|
| Oddball | Any arbitrary set of dice | Sum of all 'odd' dice values (1,3,5,7)|
| Even Steven | Any arbitrary set of dice | Sum of all 'even' dice values (2,4,6)|
| Prime Parade | Any arbitrary set of dice | Sum of all 'prime' dice values (2,3,5,7)|
| Binary Blast | Any arbitrary set of dice | Sum of all 'binary' dice values (1,2,4)|

### Complex Clusters
| Set | Description | Points |
| ----------- | ----------- | ----------|
| Triple Double | Three different pairs of dice. | 15 + (2 × Sum of each pair) |
| Double Triple | X | X|
| Full Full House | X | X|
| Straight Straight | X | X|
| Packed House | X | X|
| Larger Straight | X | X|
| 6 of a Kind | X | X|

### Super Special Rolls
| Set | Description | Points |
| ----------- | ----------- | ----------|
| Party Boat | X | X|
| Meteor Shower | X | X|
| Great Pyramids | X | X|
| Meaning of Life | X | X|
| Lucky Stevens | X | X|
| Seventh Wheeling | X | X|
| Comet in the Sky | X | X|
| Odd One Out | X | X|
| Largest Straight | X | X|
| MEGAYAHTZEE | A set where all seven dice is the same value | X|
