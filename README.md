# DRLND-P1-Navigation
This repo contains code for using deep reinforcement learning to train an agent on banana collection environment. The agent navigates in a large square world and collect bananas. A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

0 - move forward.
1 - move backward.
2 - turn left.
3 - turn right.

The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.

1) The code for agent is provided in dqn_agent.py. 
2) The code for neural used for learning Q function is provided in model.py. 
3) The code used for loading the environment and training the agent is embedded in python notebook Navigation.ipynb. 
4) Trained network parameters are saved in checkpoint.pth

Steps to follow for setting up envirnonment:

1) Set up Python Environment: Please follow the instructions in the [DRLND GitHub repository] (https://github.com/udacity/deep-reinforcement-learning#dependencies) to set up your Python environment. 
2) Download the Unity Environment: You need only select the environment that matches your operating system:

Linux: click here (https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
Mac OSX: click here (https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
Windows (32-bit): click here (https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
Windows (64-bit): click here (https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

Then, place the file in the folder where Navigation.ipynb is placed and unzip (or decompress) the file.

3) Load Jupyter Notebook Navigation.ipynb and run code cells inside to see results.
