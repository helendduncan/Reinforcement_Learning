## Chapter 3 selected questions

### Q 3.7
###### Why is the robot trying to escape a maze not improving?

The reward is +1 for exiting the maze. That's it. There's no incentive to exit quickly and so a run that takes 1000 moves is considered as successful as one that takes 100. One way to fix this would be to add a penalty for each move, perhaps -0.01, now there is incentive to exit the maze quickly and runs which do so will have a greater final reward than those which don't.

### Q 3.8
###### If $\gamma$= 0.5, and R1 - R5 = -1, 2, 6, 3, 2 respectivley, what are G0 - G5?

Using equation 3.9 and the definition that GT = 0 (hence G5 = 0) and working backwards...
$G_{t} = R_{t+1} + \gamma G_{t+1}$

$G_{5} = 0$

$G_{4} = R_{5} + \gamma G_{5}$
$G_{4} = 2 + 0.5 (0)$
$G_{4} = 2$

$G_{3} = 3 + 0.5 (2)$
$G_{3} = 4$

$G_{2} = 6 + 0.5 (4)$
$G_{2} = 8$

$G_{1} = 2 + 0.5 (8)$
$G_{1} = 6$

$G_{0} = -1 + 0.5 (6)$
$G_{0} = 2$
