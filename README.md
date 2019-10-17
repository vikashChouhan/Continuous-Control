# Contiunous Control

This project is doen to build an agent that can control a double-jointed arm towards some given locations.

## Environment Details


In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

>**The environment will be considered solved if agent is able to get a reward of +30.**

## Requirements

* Matplotlib
* Numpy
* python 3
* pytorch (Instructions: https://pytorch.org/)
* unityagent (Instructions: https://github.com/Unity-Technologies/ml-agents)
* Reacher Unity Environment ([Linux](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)),([OSX](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)),
([Win64](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)),([Win32](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip))


## Steps to Run

1. Download the environment from above links and unzip it into the directory of the project. Rename the downloaded folder to 'reacher' and make sure that it contains 'Reacher.exe' 
2. Use jupyter notebook to run the Report.ipynb notebook using `jupyter notebook report.ipynb`
3. Jupyter notebook contains detailed steps. To train the agent run the cells in order. 
4. A graph of the scores during training will be displayed after training. 



**agent.py**: This file contains the documented definition of the DDPG. It builds up the 4 networks; Actor's target and local network and the critics target and local network. 

**model.py**: This file defines the two model achitecture.

**replay_buffer**: This file is used to implement an experience store for experience replay. 
