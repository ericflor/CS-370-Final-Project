# CS-370-Final-Project


# Pirate Intelligent Agent

## Overview
In this project, I developed a pirate intelligent agent using reinforcement learning and neural networks to navigate a maze and locate a treasure. The intelligent agent was built on top of a Jupyter Notebook environment and showcased the application of key concepts in reinforcement learning to address real-world challenges.

## Project Details

### Work Overview
The project provided a foundational structure where some code templates and guidance on the game mechanics were given. I was tasked with implementing the logic for the intelligent agent to learn and make decisions in the maze environment. 

- **Given Code**: 
  - I was provided with starter code that outlined the maze environment, some foundational game mechanics, and pseudocode to guide the development process.
- **Self-created Code**: 
  - I successfully built the Q-learning training mechanism (`qtrain` function) by connecting various components of the game environment like state observation, action execution, and experience replay.
  - The reinforcement learning agent utilizes a neural network model to predict actions and was trained over multiple epochs until a desired win rate was achieved.

### Connection to Computer Science
- **What do computer scientists do and why does it matter?**  
  Computer scientists design and develop algorithms, computational systems, and applications that drive technology and innovation. In this project, the essence of computer science was evident in designing an algorithm (reinforcement learning) that enables a virtual agent to learn and make intelligent decisions. Such innovations have real-world implications, from robotics to autonomous driving and beyond.

- **How do I approach a problem as a computer scientist?**  
  Tackling this project involved a systematic approach typical of computer science: understanding the problem, breaking it down into smaller tasks, and iteratively designing, coding, and testing solutions. The training mechanism I developed was iteratively refined to optimize the agent's performance.

- **What are my ethical responsibilities to the end user and the organization?**  
  As a computer scientist, I bear the responsibility of ensuring that the algorithms and systems I develop are reliable, robust, and free from biases. For this project, this meant ensuring the agent acted logically and consistently within the environment. Beyond this specific scenario, computer scientists must also prioritize user privacy, data security, and the broader implications of their creations on society.

## Reflection
This project was a culmination of the learning journey through reinforcement learning and neural networks. Building the pirate intelligent agent provided hands-on experience and deepened my understanding of how abstract concepts in machine learning can be applied to practical scenarios. By reflecting on this project, I've further solidified my understanding and am better prepared to take on more complex challenges in the realm of artificial intelligence and computer science.


---


# Treasure Hunt Game - Reinforcement Learning w/ Neural Networks

## Project Two – Design Defense

### Analyze the differences between human and machine approaches to solving problems:

**Human Approach:**
- A human relies on visual perception and cognitive pattern recognition to solve a maze. They may use strategies like wall-following or trial and error.
- Intuition and past experience can play a role in decision-making.
- Humans may also take breaks to re-evaluate their choices and are influenced by emotions and fatigue.

**Machine Approach:**
- Machines, specifically reinforcement learning agents, operate based on mathematical models and algorithms. They use a systematic approach to explore the environment and learn optimal strategies.
- Machines lack intuition but compensate by rapidly processing vast amounts of data.
- They can continually iterate without fatigue.

### Describe the steps a human being would take to solve this maze:
1. Start at the entrance.
2. Choose a direction, often based on intuition or a chosen strategy (like always turn right).
3. Remember paths taken to avoid repetitive loops.
4. If faced with a dead-end, backtrack and try another path.
5. Continually refine the path based on feedback from the environment until the exit (treasure) is found.

### Describe the steps your intelligent agent is taking to solve this pathfinding problem:
1. Initialize a random starting point.
2. Based on the Q-values (either from a neural network or a Q-table), decide on an action (move direction).
3. Explore the environment; sometimes choose a random action (exploration) and sometimes choose the best-known action (exploitation).
4. Receive a reward or penalty based on the action's result.
5. Store the experience (state, action, reward, next state) in memory.
6. Periodically train the neural network (if used) based on experiences to refine Q-values.
7. Continually refine its strategy until it finds the most optimal path to the treasure.

**Similarities and Differences:**
- **Similarities:** Both humans and machines use feedback from the environment to refine their strategies and improve their chances of success.
- **Differences:** Humans rely on intuition, prior experience, and cognitive strategies, while machines use a systematic, algorithmic approach, iterating many times and learning from vast amounts of data.

### Assess the purpose of the intelligent agent in pathfinding:
- **Purpose:** The goal is to find the most efficient path from a starting point to a target (treasure) while navigating through an environment (maze) with various challenges and obstacles.
- **Exploitation vs Exploration:**
  - **Exploitation** is when the agent uses what it has already learned to make a decision.
  - **Exploration** is when the agent tries something new in hopes of finding a better solution.
- The ideal proportion varies but starts with a higher exploration rate, gradually reducing it to prioritize exploitation as the agent learns more about the environment. For this pathfinding problem, beginning with a high exploration rate helps in understanding the entire maze structure, and as the agent learns, it can shift towards exploitation to leverage its learned knowledge.
  
### Reinforcement Learning in Pathfinding:
- The agent (pirate) interacts with the environment (maze), receiving rewards or penalties based on its actions. Over time, it learns to associate certain actions in specific states with higher rewards, guiding it towards the goal (treasure) more efficiently.

### Evaluate the use of algorithms to solve complex problems:
- Algorithms, like deep Q-learning implemented using neural networks, allow machines to process vast amounts of data rapidly, iteratively refine their strategies, and solve complex problems that might be time-consuming or challenging for humans.

### Implementation of Deep Q-learning with Neural Networks:
1. Define a neural network model with input as the maze state and output as Q-values for each action.
2. Initialize the environment and the agent.
3. Let the agent interact with the environment, choosing actions based on Q-values predicted by the neural network.
4. Store each interaction (state, action, reward, next state) in memory.
5. Periodically train the neural network on batches from memory to update Q-values.
6. Use a discount factor to prioritize rewards that are closer in time.
7. Iterate until a certain criterion is met, like a maximum number of epochs or a satisfactory win rate.

## References
- Sutton, R. S., & Barto, A. G. (2018). _Reinforcement learning: An introduction (2nd ed.)_. MIT Press.
  - This seminal textbook provides a comprehensive introduction to the foundational concepts of reinforcement learning. It thoroughly discusses the distinction between exploration and exploitation, as well as the deep Q-learning algorithm.

- Mnih, V., Kavukcuoglu, K., Silver, D., Rusu, A. A., Veness, J., Bellemare, M. G., ... & Hassabis, D. (2015). _Human-level control through deep reinforcement learning_. Nature, 518(7540), 529-533.
  - This paper from the DeepMind team provides an in-depth exploration of using deep Q-learning for various tasks. It is particularly relevant because it discusses the implementation of neural networks in Q-learning to achieve human-level performance on certain tasks.

- Kahneman, D. (2011). _Thinking, fast and slow_. Macmillan.
  - Daniel Kahneman's book delves deep into human decision-making processes, distinguishing between intuitive (fast) and deliberate (slow) thinking. This provides a solid base for discussing human intuition and its role in problem-solving, offering a counterpoint to the algorithmic methods of machines.

 
