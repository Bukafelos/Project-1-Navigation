# My-DRL-Project-1
[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

# Project 1: Navigation

### Introduction

For this project, I will train an agent to navigate (and collect bananas!) in a large, square world.  

![Trained Agent][image1]

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, the trained agent must get an average score of +13 over 100 consecutive episodes.

### Instructions

To set up your python environment to run the code in this repository, follow the instructions below.

Create (and activate) a new environment with Python 3.6.

Linux or Mac:
conda create --name drlnd python=3.6
source activate drlnd
Windows:
conda create --name drlnd python=3.6 
activate drlnd
Follow the instructions in this repository to perform a minimal install of OpenAI gym.

Install the box2d environment group by following the instructions here.
Clone the repository (if you haven't already!), and navigate to the python/ folder. Then, install several dependencies.

git clone https://github.com/udacity/Value-based-methods.git
cd Value-based-methods/python
pip install .
Create an IPython kernel for the drlnd environment.
python -m ipykernel install --user --name drlnd --display-name "drlnd"
Before running code in a notebook, change the kernel to match the drlnd environment by using the drop-down Kernel menu.
![image](https://user-images.githubusercontent.com/66205537/159739047-c0aa423c-8882-450d-a006-09211cae4eb0.png)

 

### File Descriptions

- My_Model.py defines the DQN model architecture
- My_DQN_Agent.py defines how the agent takes actions based on the policy and learns based on feedback from the environment
- Navigation.ipynb runs the environemt and trains the agent. This is the main code to solve the environment
- My_Weights.pth contains the weights for the final DQN
