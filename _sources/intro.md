# Reinforcement Learning: An overview:

To start off with a cut and paste from [Wikipedia](https://en.wikipedia.org/wiki/Reinforcement_learning). Reinforcement learning is an area of machine learning, where intelligent agents should take actions in an environment in order to maximise the notion of a cumulative reward. To put this in the context of the NATS project - the intelligent agents are the things we are trying to train/generate, the environment will be the digital twin we make of the UK airspace, and the cumulative reward will be the continued separation of aircraft in the sky, while maintaining good fuel and time efficiency.

Sutton and Barto discuss the idea of reinforcement learning as a machine learning method that is focused on goal-directed learning from interaction. The idea is to "maximise a numerical reward signal" but without explicitly being told what actions to take, instead the agent/algorithm must explore a range of potential actions to discover which actions yield the greatest reward. As we will see in the [restaurant example](/chap02/restaurant_too.ipynb) example later on, one must balance the exploration and the exploitation phase. Another feature that reinforcement learning must deal with is the idea that there may be multi-step ways to maximise the numerical reward, that is to say that a 'low-scoring' action may need to be taken in order for a 'high-scoring' step to occur. Sutton and Barto contend that the trial-and-error search and the delayed-reward characteristics distinguish reinforcement learning from other machine learning methods (perhaps such as supervised and unsupervised learning). 

:::{note}
At the time of writing this I am new to reinforcement learning. Hopefully there aren't any glaring errors!
:::
