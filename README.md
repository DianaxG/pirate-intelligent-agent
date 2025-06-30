# pirate-intelligent-agent

Project Reflection

### Briefly explain the work that you did on this project: 
For this project, I worked on building a reinforcement learning agent referred to as the "pirate", that could learn to navigate a grid and find treasure. The goal was to train the pirate using deep Q-learning so that it could explore the map intelligently and find the best path to the treasure over time.

The code I was given included a Jupyter Notebook that had the game environment already built. It defined the grid layout, the rules for movement, rewards and penalties, and a class called `PirateAgent` that was empty except for a few placeholders. There were also functions to help visualize the pirate's journey and track its rewards during training.

What I created myself was the entire reinforcement learning logic. I designed and implemented a deep Q-network using Keras with a few hidden layers to handle the decision-making process. I built an experience replay buffer to store past experiences and sample them for training, which helps stabilize learning. I also implemented an E-greedy exploration policy to help the agent balance between exploring new paths and exploiting what it has already learned. My training loop included logic to update the Q-values, periodically sync the target network, and track rewards over time so I could visualize the agent's progress. It took a few runs and parameter tweaks, but eventually, the pirate started to learn how to find the treasure consistently.

This project gave me hands on experience with many reinforcement learning concepts we learned in class. It also challenged me to debug and experiment with different setups when things weren’t working as expected.



### Connect your learning from throughout this course to the larger field of computer science:

**What do computer scientists do and why does it matter?**  
Computer scientists solve problems by designing systems and algorithms that make technology work smarter and more efficiently. We build the logic behind everything from video games to medical diagnostics to self-driving cars. This course specifically focused on how machines can learn from experience, something that's becoming more important in real-world tech. Reinforcement learning, like I used in this project, powers everything from recommendation engines to robotics. Understanding how to train intelligent agents like this gives us the tools to build smarter and more adaptive software systems.

It matters because the decisions these systems make have real world consequences. Whether it’s helping someone navigate traffic or determining the order of search results, what we build can shape people’s experiences with technology. That’s a big responsibility.

**How do I approach a problem as a computer scientist?**  
I start by trying to understand the problem as clearly as possible, and then I break it down into smaller pieces. In this project, I had to figure out how the pirate’s world worked first, how movement was handled, how rewards were assigned, and what success looked like. Once I understood that, I could start working on building the agent’s learning system.

I didn’t expect it to work perfectly the first time. I built a basic version of the DQN, ran a few episodes, and then adjusted things like the learning rate, batch size, and epsilon decay when the agent wasn’t improving. I also relied heavily on testing one piece at a time: making sure the replay buffer worked before moving on to the network, for example. This step-by-step process is how I handle all coding projects, it keeps things manageable and lets me catch issues early.

**What are my ethical responsibilities to the end user and the organization?**  
As a developer, I’m responsible for making sure the systems I build are not just functional, but ethical and fair. Even something as “small” as defining a reward function can have unintended consequences. If I were applying reinforcement learning in the real world like in finance, healthcare, or hiring systems, I’d have to think carefully about what I’m rewarding the system for, and how that could affect different users.

My responsibility is to ask critical questions: Is this system transparent? Can someone else understand what it’s doing and why? Could it reinforce bias or lead to unfair outcomes? Am I protecting users' privacy? I also have a responsibility to the organization to document my work clearly, test it thoroughly, and be honest about its limitations. These are things I kept in mind during this project, even though it was a simulation, because these habits translate directly into how I’ll approach real-world work as a computer scientist.
