# Deep_Reinforcement_Learning_Collaboration_Competition

**The Environment**

This project works on the Tennis environment, In this environment. Two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play.

![tennis](media/15895058471430/tennis.png)


The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping.

**Solving the Environment**

The task is episodic, and in order to solve the environment, the agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,

After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores. This yields a single score for each episode.

The environment is considered solved, when the average (over 100 episodes) of those scores is at least +0.5.

**Getting Started**

Follow the instructions below to explore the environment to learn how to use the Python API to control the agent(s).

Download the environment from one of the links below. You need only select the environment that matches your operating system:

* Linux: click [here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
* Mac OSX: click [here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
* Windows (32-bit): click [here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
* Windows (64-bit): click [here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)

Place the downloaded file(s) in the folder you cloned this repo to and unzip (or decompress) the file.

Create a Python environment for this project. I recommend using `conda` or `venv`.

Activate that environment and install dependencies below:

`pip install -r requirements.txt`

**How to run the code and train agents**

1. Run jupyter notebook and open `Tennis.ipynb`.
2. Remember to change the environment path `env = UnityEnvironment(file_name="...")` to your specification.
3. Sections 1 to 3 set you up and ready for the the environment.
4. Run the cells in Section 4 to train the agent. 
5. You can change the hyperparameters in `maddpg_agent.py` to train your own agents.
