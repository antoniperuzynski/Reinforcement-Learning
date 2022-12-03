# Reinforcement-Learning
Repository for projects from Reinforcement Learning laboratory.

## Monte Carlo 

Black Jack with Monte Carlo
In this task you are asked to find an optimal policy for a Black Jack game. You are going to use an OpenAI Gym Black Jack environment in this task. OpenAI Gym is a toolkit for developing and comparing reinforcement learning algorithms. One of its features is to provide various RL-ready environments to facilitate studing and developing new Reinforcement Learning algorithms.

The main purposes of this notebook are to introduce:

- OpenAI Gym environments
- Monte Calro Methods
- the Exploring starts exploration algorithm

### Task 1
Fill in the placeholders to complete the update_qest method. You are supposed to compute an updated state-action value according to the formula:

$q_{n+1} = q_{n} + \frac{1}{n}(G_n-q_n)$

where:

- $q_{n}$ - current estimated state-action value
- $q_{n+1}$ - new estimated state-action value
- $G_n$ - return obtained for the explored state and action
- $n$ - number of actions (computed separately for each action type)

### Task 2
Complete the generate_episode function by filling in the code placeholders You are supposed to:

- randomly select the initial action and execute this action
- select every other action according to the policy and execute it
- update policy for each state-action pair generated during the episode

### Task 3
Generate episodes and learn from them until you learn the optimal policy. You may use policy.plot() to visualize your policies.
