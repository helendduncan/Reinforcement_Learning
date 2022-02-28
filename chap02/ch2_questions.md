## Chapter 2 selected questions

![Graph showing the returns for two methods on a ten-armed test bed as a function of number of steps. An optimistic greedy method with Q1 = 5 is shown in blue, with increasing percentage of number of optimal actions with steps. The method appears to plateau at approximately 80%. A sharp peak is observed at around 10 steps. Also shown in a realistic epsilon-greedy method with Q1 = 0, epsilon=0.1 which increases slower than the optimistic greedy method, reaching a maximum of around 70% optimal actions chosen](../images/opti_greedy.png)
### Q 2.6
This graph shows the percentage of optimal actions taken as a function of the number of steps over a ten-armed test bed. 
If have an initialisation value of 5 (which is higher than most values expected from any of the 10 initial distributions, then the agent will search all ten arms) and the estimate Qn will be updated with a smaller estimate than the initial value. As this is a greedy method the agent will pick another, and another from the initialised set until all ten have been sampled. Then it will focus on what it believes to be the otpimal choice, this is slightly better than starting off with Q1=0 as all points are sampled at least once. The 'optimal' run is then picked exclusively until the Qn is calculated below one of the other estimates from one of the other pulls.

![Graph showing the average reward as a function of number of steps for an upper confidence bound method and an epsilon greedy method. Both show a gradual increase from 0 to 500 steps before begining to plateau with a reward of 1.1 and 1.2 for the epsilon greedy and the upper confidence bound method respectively. The upper confidence band data shows a spike at step 11](../images/ucb.png)

### Q 2.8
The spike in the UCB data at step 11 corresponds to the time when all initial states have been sampled once and the agent starts picking greedily. It will pick greedily until the value of ln(t) is greater than Nt(a)
