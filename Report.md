# Udacity-Navigation-Project

For this project, I have train an agent to navigate (and collect bananas!) in a large, square world.  
The "Navigation-Project" is the first project in Udacitys Deep Reinforcement Learning Nanodegree under Value Based Methods section.


## Trained Agent

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction. Given this information, the agent has learned how to best select actions. Four discrete actions are available, corresponding to:  

`0` - move forward.  
`1` - move backward.  
`2` - turn left.  
`3` - turn right.  

The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

## Learning Algorithm
For the learning algorithm, the solution was developed using Deep Q-Network which is using a deep nural network as a function approximator for the Q-function.
The network archetecture has three linear layers with relu activation function. The first layer input is equal to the state size and the unit size is 64, the following layers have equal size units except for the output layer which is equal to the action size. As for the episode decay i set it to a value of 0.99. The algorithm terminates when the reward value >= 16. 
The following parameter values are specified for the agent:  

BUFFER_SIZE = int(1e5)  # replay buffer size  
BATCH_SIZE = 64         # minibatch size  
GAMMA = 0.99            # discount factor  
TAU = 1e-3              # for soft update of target parameters  
LR = 5e-4               # learning rate   
UPDATE_EVERY = 4        # how often to update the network  

## Plot of Rewards
A plot of rewards per episode is included to illustrate that the agent is able to receive an average reward (over 100 episodes) of at least +13. The submission reports the number of episodes needed to solve the environment. 
The Environment was solved in 425 episodes!	With an average Score of 16.02.  
![image](https://user-images.githubusercontent.com/65574771/210248306-c0a52107-8bc2-44bf-a2e8-e1c66f931741.png)


## Ideas for Future Work
- Implement a double DQN, a dueling DQN, and/or prioritized experience replay!  
- To train an agent from raw pixels!
