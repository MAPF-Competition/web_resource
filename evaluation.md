# Evaluation
The submissions will be evaluated on two types of AWS instances:
- CPU Instance
- GPU Instance (Coming soon)
  
They both have the same amount of RAM. But CPU instances have more processor resources, while GPU instances have additional resources for machine learning.

When you create an account on the competition website, we will create a private github repository for you. You will upload your implementation to this repository including all dependencies. We will pull your code from this repository and package up your implementation into a binary submission file for evaluation. The evaluation process runs in two steps, the preprocessing and the planning.

# Preprocessing
In preprocessing, the map is given to each planner. The planner has the opportunity to compute auxiliary data for this map before proceeding to the evaluation stage. 
Preprocessing time is 30 Minutes per map. Nothing you do at this stage will be counted into your final score.

# Planning
In planning, the initial locations of agents are revealed and  tasks will be assigned to agents.
The planner must navigate agents to designated locations to accomplish the task. Each time the agent completes a task, a new task will be assigned to the agent. The goal is to complete as many tasks as possible within the planning time horizon of 5000 timesteps. Time elapses at a rate of 1 second per timestep (i.e. each map is evaluated for 5000 seconds total).
 
During each planning episode, we will ask your planner to compute the next valid action for each agent. You can take as long as you want for planning, but the clock is ticking while you are deliberating. Failure to compute a next valid action for every agent means all agents will wait in place until the next planning episode.

# Domains
Each submission will be evaluated on 5 instances:
- Random: 100 agents, a 32 by 32 map with 20% random obstacles.
- City: 250 agents, a 256 by 256 map representing part of the city of Paris.
- Game: 500 agents, 481 by 530 map from computer games.
- Fulfilment: 1000 agents, 500 by 140 map representing synthetic automated fulfilment centre.
- Sortation: 1000 agents, 500 by 140 map representing synthetic automated sortation centre.

The maps are available for download and analysis. But the problem instances (tasks and robot locations) are hidden until after the competition.


# Planner Categories:
In real life, planners are expected to achieve efficiency in different aspects, such as high  throughput, quick computation time. Our competition take into account different areas and categorise the prize into three categories:
- Best Overall
  
In this category, we track the best solution for any instance. 
This is called the ‘virtual best’ planner, and we rank your performance on each instance relative of this baseline. We use the following formula:
$$\mbox{Your score} = \displaystyle \sum^{i}_{instance i}{\frac{\mbox{Your number of task finished for instance }i}{\mbox{best number of task finished for instance }i}}$$
The winner of this category is the planner that has the highest score.

- Line Honours
  
This category tracks the planner that has the largest number of best solutions. 
We track best solutions for each instance throughout the competition, and count the number of best solutions by any planner at the end of the submission deadline.

- Fast Mover

To be eligible for this category, planners always compute valid actions for all the agents within the time limit of each planning episode (1 second). The winner of this category has the best overall score among all eligible planners.