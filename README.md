# codeAndBeerBowlingKata
TDD Bowling Kata for Code and Beer Events


## Scoring ten-pin bowling
_adapted from [Uncle Bob's formulation](http://butunclebob.com/ArticleS.UncleBob.TheBowlingGameKata)_

![Example scoresheet](https://www.wpclipart.com/recreation/sports/bowling/bowling_scoresheet_example.png)

The game consists of 10 frames as shown above.
In each frame the player has two chances to roll the ball to knock down 10 pins.
The score for the frame is the total number of pins knocked down, plus bonuses for strikes and spares.

A spare (/) is when the player knocks down all 10 pins in two rolls.
The bonus for that frame is the number of pins knocked down by the next roll.
So in frame 2 above, the score is 10 (the total number knocked down) plus a bonus of 5 (the number of pins knocked down on the next roll) for a total of 15.

A strike (X) is when the player knocks down all 10 pins on their first roll.
The bonus for that frame is the number of pins knocked down by the next two rolls.
So in frame 1 above, the score is 10 (the number knocked down) plus bonuses of 9 and 1 (the number of pins knocked down on the two next rolls) for a total of 20. 

In the tenth frame, a player who rolls a spare or strike is allowed to roll the extra balls needed to complete the frame.
No more than three balls can be rolled in the tenth frame.


## The task

Write a `TenPinBowlingGame` class with two methods:
* `roll` is called each time the player rolls a ball; it takes the integer number of pins knocked down, and returns nothing.
* `score` is called at the end of the game and returns the total score.


## Remember Uncle Bob's [three rules](http://butunclebob.com/ArticleS.UncleBob.TheThreeRulesOfTdd)!
Thou shalt not

1. write any production code unless it is to make a failing unit test pass.
2. write any more of a unit test than is sufficient to fail; compilation failures are failures.
3. write any more production code than is sufficient to pass the one failing unit test.
