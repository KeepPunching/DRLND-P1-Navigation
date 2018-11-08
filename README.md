# DRLND-P1-Navigation
This repo contains code for using deep reinforcement learning to train an agent on banana collection environment. The agent navigates in a large square world and collect bananas. A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

0 - move forward.
1 - move backward.
2 - turn left.
3 - turn right.

The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.

The code for agent is provided in dqn_agent.py. The code for neural used for learning Q function is provided in model.py. The code used for loading the environment and training the agent is embedded in python notebook Navigation.ipynb 
