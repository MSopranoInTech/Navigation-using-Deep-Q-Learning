# Navigation-using-Deep-Q-Learning
DQN to train RL agent navigate a square world for maximizing rewards

For this project, we will train an agent to navigate and collect bananas in a large, square world. A reward of +1 is provided 
for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is 
to collect as many yellow bananas as possible while avoiding blue bananas. The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

0 - move forward. <br>
1 - move backward. <br>
2 - turn left. <br>
3 - turn right. <br>

The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive
episodes.

![alt text](https://github.com/MSopranoInTech/Navigation-using-Deep-Q-Learning/blob/master/banana_env2.png)

I used a Deep Q network with the following values of hyperparameters: eps_start=1.0, eps_end=0.01, eps_decay=0.995, gamma(discount factor) = 0.99, max_t (maximum time steps per episode) =1000. The 3 layer neural network was used with 3 fully connected layers having 64 neurons each.

Episode 100	Average Score: 1.07 <br>
Episode 200	Average Score: 4.26 <br>
Episode 300	Average Score: 7.59 <br>
Episode 400	Average Score: 10.41 <br>
Episode 500	Average Score: 12.29 <br>
Episode 566	Average Score: 13.00 <br>
Environment solved in 466 episodes!	Average Score: 13.00 <br>

![alt text](https://github.com/MSopranoInTech/Navigation-using-Deep-Q-Learning/blob/master/results.png)

# Additional ideas to consider in the future
1. Prioritized Experience Replay
2. Learning from Pixels
