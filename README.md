# Udacity-DRL-Continuous-Control
This repo is an implementation to the second project, called Navigation, in the [Deep Reinforcement Learning Nanodegree](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893)
<p align="center"><img src=reacher.gif></p>

## Project Description 
In this project, the goal of the agent is to maintain its position at the target location for as many time steps aspossible, where the agent is a double-jointed arm can move to target locations. The environment is considered solved, when the average (over 100 episodes) of average scores of twenty agents is at least +30.

### State Space
The state (observation) space contains 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm.

### Action space
Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

### Rewards
A Reward of +0.1 is provided for each step that the agent's hand is in the goal location.

### Project Environment
#### Step 1: Clone the [DRLND repo](https://github.com/udacity/deep-reinforcement-learning). Follow the instructions in the readme file to configure the python (3.6 was used in this project) environment.
#### Step 2: Download the Unity Environment according to your operating system (20 agents environment):
- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)

Then, place the file in the p2_continuous-control/ folder in the DRLND GitHub repository, and unzip (or decompress) the file.

#### Step 3: Run
In the terminal run the following command (make sure you are in the correct directory):
```shell
$ jupyter notebook
```
This will open jupyter notebook in the browser, in which you can add the files from this repository to be able to run the code implemented here. 
- Continuous_Control.ipynb contains the code that you should run to train the agents.
- model.py contains the Actor and Critic Networks.
- ddpg_agent.py contains the implementation of the agent step, act and learn, as well as the replay buffer.
- checkpoint files contain the trained models that can be loaded and used directly.
