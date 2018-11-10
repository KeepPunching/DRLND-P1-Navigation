Deep Reinforcement Learning algorithm has been used to solve the banana collection environment. 

An agent has been trained to navigate and collect bananas in a large, square world. A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

0 - move forward.
1 - move backward.
2 - turn left.
3 - turn right.
The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.

Details of learning algorithm are as follows:
1) An implementation of Deep Q-Network has been created. Fully connected feedforward network is used as a function approximator to estimate
Q-value function. The neural network contains fully connected input, output and one hidden layer (called local network).
2) A memory buffer is used to save the experience tuple of agent (state,action,reward, next state).
3) A copy of the neural network is maintained (called target network) which provides target Q values to learn for local network at every timestep.
4) Every few iterations target network is updated with a copy of the local network weights. A parameter tau is used  to decide the fraction of 
local network parameter copied on to target network parameters.
5) The agent follows an epsilon greedy action selection policy, which means action is selected using Q values from local network with a probability
of 1 - epsilon and selected randomly with a probability of epsilon.
6) epsilon value is decayed every time step to change the exploration-exploitation balance of the algorithm. Higher the epsilon value, more
is the exploration and vice versa.
7) Agent's experience tuple (state, action, reward, next state) is saved in the memory buffer.
7) local network is trained every time step. A sample batch
