# CS-370-Final-Project

Treasure Hunt Game - Reinforcement Learning w/ Neural Networks

Project Two – Design Defense 

 

Analyze the differences between human and machine approaches to solving problems: 

Human Approach: 

A human relies on visual perception and cognitive pattern recognition to solve a maze. They may use strategies like wall-following or trial and error. 

Intuition and past experience can play a role in decision-making. 

Humans may also take breaks to re-evaluate their choices and are influenced by emotions and fatigue. 

Machine Approach: 

Machines, specifically reinforcement learning agents, operate based on mathematical models and algorithms. They use a systematic approach to explore the environment and learn optimal strategies. 

Machines lack intuition but compensate by rapidly processing vast amounts of data. 

They can continually iterate without fatigue. 

 

Describe the steps a human being would take to solve this maze: 

Start at the entrance. 

Choose a direction, often based on intuition or a chosen strategy (like always turn right). 

Remember paths taken to avoid repetitive loops. 

If faced with a dead-end, backtrack and try another path. 

Continually refine the path based on feedback from the environment until the exit (treasure) is found. 

 

Describe the steps your intelligent agent is taking to solve this pathfinding problem: 

Initialize a random starting point. 

Based on the Q-values (either from a neural network or a Q-table), decide on an action (move direction). 

Explore the environment; sometimes choose a random action (exploration) and sometimes choose the best-known action (exploitation). 

Receive a reward or penalty based on the action's result. 

Store the experience (state, action, reward, next state) in memory. 

Periodically train the neural network (if used) based on experiences to refine Q-values. 

Continually refine its strategy until it finds the most optimal path to the treasure. 

 

Similarities and Differences: 

Similarities: Both humans and machines use feedback from the environment to refine their strategies and improve their chances of success. 

Differences: Humans rely on intuition, prior experience, and cognitive strategies, while machines use a systematic, algorithmic approach, iterating many times and learning from vast amounts of data. 

 

Assess the purpose of the intelligent agent in pathfinding: 

Purpose: The goal is to find the most efficient path from a starting point to a target (treasure) while navigating through an environment (maze) with various challenges and obstacles. 

 

Exploitation vs Exploration: 

Exploitation is when the agent uses what it has already learned to make a decision. 

Exploration is when the agent tries something new in hopes of finding a better solution. 

The ideal proportion varies but starts with a higher exploration rate, gradually reducing it to prioritize exploitation as the agent learns more about the environment. For this pathfinding problem, beginning with a high exploration rate helps in understanding the entire maze structure, and as the agent learns, it can shift towards exploitation to leverage its learned knowledge. 

 

Reinforcement Learning in Pathfinding: 

The agent (pirate) interacts with the environment (maze), receiving rewards or penalties based on its actions. Over time, it learns to associate certain actions in specific states with higher rewards, guiding it towards the goal (treasure) more efficiently. 

 

Evaluate the use of algorithms to solve complex problems: 

Algorithms, like deep Q-learning implemented using neural networks, allow machines to process vast amounts of data rapidly, iteratively refine their strategies, and solve complex problems that might be time-consuming or challenging for humans. 

 

Implementation of Deep Q-learning with Neural Networks: 

Define a neural network model with input as the maze state and output as Q-values for each action. 

Initialize the environment and the agent. 

Let the agent interact with the environment, choosing actions based on Q-values predicted by the neural network. 

Store each interaction (state, action, reward, next state) in memory. 

Periodically train the neural network on batches from memory to update Q-values. 

Use a discount factor to prioritize rewards that are closer in time. 

Iterate until a certain criterion is met, like a maximum number of epochs or a satisfactory win rate. 

 

 

 

 

 

 

 

 

 

References 

Sutton, R. S., & Barto, A. G. (2018). Reinforcement learning: An introduction (2nd ed.). MIT Press. 

This seminal textbook provides a comprehensive introduction to the foundational 		concepts of reinforcement learning. It thoroughly discusses the distinction between exploration and exploitation, as well as the deep Q-learning algorithm. 

Mnih, V., Kavukcuoglu, K., Silver, D., Rusu, A. A., Veness, J., Bellemare, M. G., ... & Hassabis, D. (2015). Human-level control through deep reinforcement learning. Nature, 518(7540), 529-533. 

This paper from the DeepMind team provides an in-depth exploration of using deep Q-learning for various tasks. It is particularly relevant because it discusses the implementation of neural networks in Q-learning to achieve human-level performance on certain tasks. 

Kahneman, D. (2011). Thinking, fast and slow. Macmillan. 

Daniel Kahneman's book delves deep into human decision-making processes, distinguishing between intuitive (fast) and deliberate (slow) thinking. This provides a solid base for discussing human intuition and its role in problem-solving, offering a counterpoint to the algorithmic methods of machines. 

 
