# Deep Reinforcement Learning Nanodegree - Continuous Control Project 2
#### Solution by Leschek Kopczynski

Second hands-on project of Udacity's Deep Reinforcement Learning Nanodegree. The Solution is presented in Jupyter Notebook wich is running in a conda virtual environment.
This repository contains material related to Udacity's
[Deep Reinforcement Learning Nanodegree](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893)
program. Content and text elements to setup the environment is borrowed from Udacity's 
[repository](https://github.com/udacity/deep-reinforcement-learning) and especially from
[Project 2](https://github.com/udacity/deep-reinforcement-learning/tree/master/p2_continuous-control).

As mentioned as a tip by the course leader the code is oriented by the solutions teached during the drl - nanodegree. 

## Dependencies

To set up your python environment to run the code in this repository, follow the instructions below.

1. First of all (if you haven't already) install [Anaconda](https://docs.anaconda.com/anaconda/install/) on your System.

2. Create (and activate) a new environment with Python 3.6.

	- __Linux__ or __Mac__: 
	```bash
	conda create --name drlnd python=3.6
	source activate drlnd
	```
	- __Windows__: 
	```bash
	conda create --name drlnd python=3.6 
	activate drlnd
	```
	
3. Follow the instructions in [this repository](https://github.com/openai/gym) to perform a minimal install of OpenAI gym.  
	- Next, install the **classic control** environment group by following the instructions [here](https://github.com/openai/gym#classic-control).
	- Then, install the **box2d** environment group by following the instructions [here](https://github.com/openai/gym#box2d).
	
4. Clone the repository (if you haven't already!), and navigate to the `python/` folder.  Then, install several dependencies.
```bash
cd python
pip install .
```
This will install the dependencies to the conda environment.

5. Create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `drlnd` environment.  
```bash
python -m ipykernel install --user --name drlnd --display-name "drlnd"
```

6. Start Jupyter Notebook Server from (project) root folder with:
```bash
python -m ipykernel install --user --name drlnd --display-name "drlnd"
```

7. Follow the instructions in the Terminal and navigate to the project by following the provided hyperlink.
8. Once you open the provided link, you have to navigate to `Continuous_Control.ipynb`. Then choose initial the new kernel ( navigate to ):
```bash
kernel -> change kernel -> drlnd
```

#### Congratulations, your setup is ready to go!

## Project and Environment
**NOTE: A full description is provided inside the jupyter notebook**

For this project, you will work with the [Reacher](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher) environment.

In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.
The task is episodic, and in order to solve the environment, the agent must get an average score of +30 over 100 consecutive episodes.

### Distributed Training

For this project, a single agent version of the Unity environment is provided.

### Solving the Environment
#### Getting Started

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:

    - **_Version with One (1) Agent_**
        - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
        - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
        - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)
        - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)

2. Place the file in the GitHub repository, in the `root` folder, and unzip (or decompress) the file. 

#### Instructions
Follow the instructions in `Continuous_Control.ipynb` to get started with training your own agent! 
Note that the task is episodic. Per definition, the agent must get an average score of +30 over 100 consecutive episodes
in order to solve the environment.

Results, performance and future work are shown and discussed in `Report.pdf`.