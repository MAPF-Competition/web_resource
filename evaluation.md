Submissions will be evaluated using AWS.  We offer two different types of instances and you get to choose which one best suits your planner:
- CPU Instance
- GPU Instance (Coming soon)

CPU instances have more processor resources, while GPU instances have additional resources for machine learning. Both have the same amount of storage and RAM. 

Once you make a submission the evaluation proceeds in two stages: offline preprocessing and online planning. 

## Offline Preprocessing
During the preprocessing stage the current map is given to each planner. The planner has the opportunity to analyse the map and compute auxiliary data before proceeding to the evaluation stage. Preprocessing time is limited to 30 Minutes per map. Nothing you do at this stage will be counted into your final score.

## Online Planning
In the planning stage the initial locations of robots are revealed and errands/tasks are assigned, one for each robot. Time elapses at a rate of 1 second per timestep and your planner will be evaluated for 5000 seconds on each map. 

At every timestep we will ask your planner to compute the next valid action for each robot. You can take as long as you want for planning, but the clock is ticking while you are deliberating. Failure to compute a next valid action for every robot, or deliberating for longer than 1 second, results in all robots waiting in place until the next planning episode.

## Domains
Each submission will be evaluated on 5 instances:
- Random: 100 robots, a 32 by 32 map with 20% random obstacles.
- City: 250 robots, a 256 by 256 map representing part of the city of Paris.
- Game: 500 robots, 481 by 530 map from computer games.
- Fulfilment: 1000 robots, 500 by 140 map representing synthetic automated fulfilment centre.
- Sortation: 1000 robots, 500 by 140 map representing synthetic automated sortation centre.

The maps are [available for download](https://github.com/MAPF-Competition/Start-Kit/tree/main/example_problems) and analysis. But the problem instances (errands and robot locations) are hidden until after the competition.


## Planner Categories:
In real life, planners are expected to achieve efficiency in different aspects, such as high  throughput, quick computation time. For this reason our competition recognises distinguished performance in three distinct categories: 

**Best Overall**
In this category, we use a `virtual best` planner to track the best known solution for any instance and from any participant. We then rank your performance on each instance relative to this baseline. We use the following formula:
$$\mbox{Your score} = \displaystyle \sum^{max}_{i=0}{\frac{\mbox{Your number of errands finished for instance }i}{\mbox{best number of errands finished for instance }i}}$$
The winner of this category is the planner that has the highest score.

**Line Honours**
This category tracks the planner that has the largest number of best solutions. We track best solutions for each instance throughout the competition and we count the number of best solutions by any planner at the end of the submission deadline.

**Fast Mover**
To be eligible for this category, planners always compute valid actions for all the robots within the time limit of each planning episode (1 second). The winner of this category has the best overall score among all eligible planners.
