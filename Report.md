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
The report clearly describes the learning algorithm, along with the chosen hyperparameters. It also describes the model architectures for any neural networks.

## Plot of Rewards
A plot of rewards per episode is included to illustrate that the agent is able to receive an average reward (over 100 episodes) of at least +13. The submission reports the number of episodes needed to solve the environment. Environment solved in 425 episodes!	Average Score: 16.02  
![image](https://user-images.githubusercontent.com/65574771/210248306-c0a52107-8bc2-44bf-a2e8-e1c66f931741.png)


## Ideas for Future Work
The submission has concrete future ideas for improving the agent's performance.  

Solve the environment in fewer than 1800 episodes!  
Write a blog post explaining the project and your implementation!  
Implement a double DQN, a dueling DQN, and/or prioritized experience replay!  
For an extra challenge after passing this project, try to train an agent from raw pixels! Check out (Optional) Challenge: Learning from Pixels in the classroom for more details.  
