# Autonomous Navigation using Re-inforcement Learning 
In this project, we are implementing the Q-learning approach of reinforcement learning in order to autonomously navigate the mobile robot. <br />

The reinforcement learning is a learning technique based on trial and error, and the interaction between the agent and its environment, where from a state or situation s in the environment, the agent selects and performs an action that causes a transition to state s'. the agent receives in return a reinforcement signal r, which can be a reward or punishment. The purpose of this learning is to maximize future rewards. <br />

![deep-learning](/Images/deep-learning.png)

Q-learning is a form of model-free reinforcement learning. It can also be viewed as a method of asynchronous dynamic programming (DP). It provides agents with the capability of learning to act optimally in by experiencing the consequences of actions, without requiring them to build maps of the domains.

## MAIN OBJECTIVES
1.	Studying and understanding various machine learning approaches.

2.	Understanding the mathematical equations and working of each parameter.

3.	Creating the environment in which the robot will learn.

4.	Construct the Q-table.

5.	Assign rewards for each action that might be taken.

6.	Update the Q-table accordingly.

7.	Repeat till fine trajectory is obtained.

8.	Try the same for different environments.

### Modules

1. Evaluation function

The evaluation function is the main Q-function which evaluates the state of the agent and the action that it is likely to take. This action is performed by the agent based on the knowledge gained earlier, which is stored in the internal memory of the system.

2. Reinforcement function

The major function of this is to provide a reward or punishment for each action that is taken by the agent. This is represented as R and contains the new states’ and the generated reward r for that action. This reward can be -1, 0 or 1, based on the consequence of the action, and accordingly the Q-values in the table are updated.

3. Update function

This function utilizes the value obtained from the Reinforcement functions and updates the Q-table. The update function is repeatedly used till an optimum set of values is obtained for that system.

4. GUI

The Graphical user interface is designed using Tkinter python library. In this project, we have implemented a grid-like structure to showcase the environment.

5. The Brain

The Brain is the driver which runs the entire system. It checks against the conditions, and at each point determines whether:

a.	There is a next state possible for the concerned action<br />

b.	The agent has reached the destination<br />

Thus the brain initializes the various parameters at the beginning, and overalls drives the agent and directs its path, till it reaches the goal.

## Prerequisites
I. Python<br />

    1. NumPy<br />
    2. Pandas<br />
    3. Tkinter<br />
    
II. IDE (we used Pycharm)<br />


## Install Dependencies

Install Numpy:
``` 
    python -m pip install --user numpy
```
Install Pandas:
``` 
    python -m pip install --user pandas
```

## Output Screens
![Capture](/Images/Capture.PNG)
    
## Conclusion
After the completion of the project, we conclude that Q-learning is a simple and efficient technique to achieve autonomous robot navigation. Using Q-learning algorithm, we found out that efficiency in the results based on the prescribed use-case in this project is 50% more as compared to State–action–reward–state–action (SARSA) approach. However, we also find out that it is not optimized due to storage of many Q-values inside a 2-D array. Thus, it is not space efficient and other techniques of reinforcement learning can be applied in order to achieve the desired efficiency and optimal performance.
