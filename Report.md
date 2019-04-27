# TRAINING CODE

## Training Code
This repository includes functional, well-documented, and organized code for training the agent. 
* model.py - It has Neural Network implementation for state action Q function
* dqn_agent.py - contains code for Agent learning and Replay buffer implementation.
* Navigation.ipynb - contains the code for creating the environment, training and testing the agent 

## Framework
Code is written in pytorch and python3

## Saving model weights
model weights is saved in checkpoint.pth

# README

We have used Readme provided by Udacity which has all relevant details like:-
## README.md
The GitHub submission includes a README.md file in the root of the repository.

## Project Details
The README describes the the project environment details (i.e., the state and action spaces, and when the environment is considered solved).

## Getting Started
The README has instructions for installing dependencies or downloading needed files.

## Instructions
The README describes how to run the code in the repository, to train the agent.

# REPORT

## Report
You are reading the report.

## Learning Algorithm
We used Adam optimizer with learning rate of 5e-4. We got average reward of +16 by training in more than 650 episodes. Our network architecture for Q function is 2 fully connected layers of 64 neurons followed by output layer of size matching number of actions.

## Plot of Rewards  
Our agent is able to achieve average rewards of more than +13. We have plotted the reward with episode in relevant section of notebook.

## Ideas for future work
We can work on following ideas to improve  
* double DQN
The idea of Double Q-learning is to reduce overestimations by decomposing the max operation in the target into action selection and action evaluation

* dueling DQN
Dueling network represents two separate estimators: one for the state value function and one for the state-dependent action advantage function. The main benefit of this factoring is to generalize learning across actions without imposing any change to the underlying reinforcement learning algorithm. 

* prioritized experience replay
Here rather than uniformly sampling from a replay memory, we prioritize experience, so as to replay important transitions more frequently, and therefore learn more efficiently.
