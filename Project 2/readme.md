# Welcome to Project 2: Reinforcement Learning 

(This project is particially constructed based on online resources).

In this project, you will learn how to learn a policy for your agent based on the historical trials that the agent has already made. Two popular senarios are involved. One is Grid World, and another is Mountain Car.  This project will also be a competition among you: let's see who will find the best policy for two different Markov decision processes given sampled transitions, with each consisting of a state _s_, action _a_, reward _r_, and next state _sp_. The best policy is the one that maximizes the total expected reward.

Two CSV-formatted datasets are provided. Note that this is an instance of batch reinforcement learning (or offline reinforcement learning) where the data from exploring has been collected and given to you, and you have to work with it. There will not be an opportunity to explore in runtime in a simulator because your output will be a (deterministic) policy that we will run on our simulator. Keep this in mind, particularly if you are using a model-free approach.

![Gird World Sample](https://github.com/bonaldli/DMU-Uni-Koeln/blob/main/Project%202/Figs/grid-world.png?raw=true)
![Mountain Car Sample](https://github.com/bonaldli/DMU-Uni-Koeln/blob/main/Project%202/Figs/mountain-car.gif?raw=true)

## Datasets
First of all, we have three datasets, and the summaries are given below:
| Dataset  | Description |
| ------------- | ----------------- |
| Grid World Data | 10 x 10 grid world (100 states) with 4 actions. Use `LinearIndices((10,10))[x,y]` to find the integer state from the x and y coordinates. Actions are 1: left, 2: right, 3: up, 4: down. The discount factor is 0.95.|
| Mountain Car Data | MountainCarContinuous-v0 environment from [Open AI Gym](https://www.gymlibrary.dev/) with altered parameters. State measurements are given by integers with 500 possible position values and 100 possible velocity values (50,000 possible state measurements). `1+pos+500*vel` gives the integer corresponding to a state with position pos and velocity vel. There are 7 actions that represent different amounts of acceleration. This problem is undiscounted, and ends when the goal (the flag) is reached. Note that since the discrete state measurements are calculated after the simulation, the data in medium.csv does not quite satisfy the Markov property. |

Hints: Each line in the CSV file represents a transition from a state _s_ to a next state _sp_—along with the associated reward _r_ —when taking an action _a_. You might not have data for every state, nor are all states equally important. Use your best judgment when handling this.

## Resources:
- 1. Grid World:
  - [R1.1: Reinforcement Learning — Implement Grid World](https://towardsdatascience.com/reinforcement-learning-implement-grid-world-from-scratch-c5963765ebff)
  - [C1: Code](https://github.com/MJeremy2017/reinforcement-learning-implementation/blob/master/GridWorld/gridWorld.py)
- 2. Mountain Car:
  - [R2.1: Reinforcement Learning Applied to the Mountain Car Problem](https://towardsdatascience.com/reinforcement-learning-applied-to-the-mountain-car-problem-1c4fb16729ba)
  - [C2.1: MountainCarContinuous-v0 ](https://github.com/openai/gym/blob/master/gym/envs/classic_control/continuous_mountain_car.py): You may look at the code for the MountainCarContinuous-v0 environment, but note that we will not use exactly the same parameters.
  - [C2.2: Mountain Car Implementation](https://github.com/MJeremy2017/reinforcement-learning-implementation/tree/master/MountainCar)
  
There are a lot of resources online. You are encouraged to search and reuse it. But please take care that all the resources provided above are online reinforcement learning, which means no historical data are provided and the agent is trained and improving its policy online in a simulator. But our project is to do a batch reinforcement learning, where you learn an optimal policy based on historical data. Please pay attention to this difference.

## Task:
- Python is recommended. However, you could use any programming language that you prefer. 
- You cannot use any package/algorithms directly related to reinforcement learning. You can use general optimization packages and libraries for things like function approximation and ODE solving so long as you discuss what you use in your writeup and make it clear how it is used in your code.
- Discussions are encouraged.
- Submit a `report.pdf` file with a description of your algorithm(s) and their performance characteristics. Include the running/training time for each policy. Also, typeset your code and include it in the PDF.

## Grading:
- Grid World Policy (`grid_world.policy`): 20%
- Mmountain Car Policy (`mountain_car.policy`): 20%
- Report: 60%
  - Description of policy: 15%
  - Performance characteristics, i.e. running/training time: 15%
  - Code (in PDF): 20%
  - Reference: 10%
  - No more than 6 pages

## Template
Please use the given Overleaf [Template](https://www.overleaf.com/read/fqpyqzzjvfzy) to write the project report.

## Submission
Submit your `.zip` file to the ILIAS system before the deadline: **23:59 PM, 14 Jan 2024 (Sun)**. The file should include the following:
- `.policy` files (x2): `grid_world.policy`, `mountain_car.policy`
- `.pdf` file (x1): `Project 2 Report-First Name-Last Name.pdf`
- python file (x1): your source code file
