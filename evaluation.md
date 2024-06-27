## Evaluation Process ![r2](./external_page_resource/robots/r12_s.png)

Submissions will be evaluated using an AWS cloud compute instance with the following specifications:

> - AMD EPYC 7R13 Processor with 32 vCPUs
> - 128 GiB Memory
> - 40 GiB Storage Space

Once you make a submission the evaluation proceeds in two stages: offline preprocessing and online planning. 

## Offline Preprocessing
During the preprocessing stage the current map is given to each planner. The planner has the opportunity to analyse the map and compute auxiliary data before proceeding to the evaluation stage. Preprocessing time is limited to 30 Minutes per map. Nothing you do at this stage will be counted into your final score.

## Online Planning
In the planning stage the initial locations of robots are revealed and errands/tasks are assigned, one for each robot. Time elapses at a rate of 1 second per timestep and your planner will be evaluated up to 5000 seconds on each map. 

At every timestep we will ask your planner to compute the next valid action for each robot. You can take as long as you want for planning, but the clock is ticking while you are deliberating. Failure to compute a next valid action for every robot, or deliberating for longer than 1 second, results in all robots waiting in place until the next planning episode.

## Domains
Each submission will be evaluated using a variety of instances on 5 different maps:

>| |   |   |
>|:---:|:---:|:---:|
>|![r](external_page_resource/images/random-32-32-20_s.jpg)|![r](external_page_resource/images/Paris_1_256_s.jpg)|![r](external_page_resource/images/brc202d_s.jpg) |
>|`Random (random-32-32-20)`| `City (Paris)`|`Game (brc202d)`|
>|a 32 by 32 map with 20% random obstacles.| a 256 by 256 map representing part of the city of Paris.|a 481 by 530 map from computer games.|

>| |
>|:---:|
>|![r](external_page_resource/images/warehouse_large_s.jpg)|
>|`Warehouse`|
>|a 500 by 140 map representing synthetic automated fulfilment centre.|

>| |
>|:---:|
>|![r](external_page_resource/images/sortation_large_s.jpg)|
>|`Sortation`|
>|a 500 by 140 map representing synthetic automated sortation centre.|


The maps are [available for download](https://github.com/MAPF-Competition/Start-Kit/tree/main/example_problems) and analysis. But the problem instances (errands and robot locations) are hidden until after the competition.


## Planner Categories:
In real life, planners are expected to achieve efficiency in different aspects, such as high  throughput, quick computation time. For this reason our competition recognises distinguished performance in three distinct categories: 

**Best Overall**
> In this category, we use a `virtual best` planner to track the best known solution for any instance and from any participant. We then rank your performance on each instance relative to this baseline. We use the following formula:
>
> $$\mbox{Your score} = \displaystyle \sum^{max}_{i=0}{\frac{\mbox{Your number of errands finished for instance }i}{\mbox{best number of errands finished for instance }i}}$$
> 
> The winner of this category is the planner that has the highest score.

**Line Honours**
> This category tracks the planner that has the largest number of best solutions. We track best solutions for each instance throughout the competition and we count the number of best solutions by any planner at the end of the submission deadline.

**Fast Mover**
> To be eligible for this category, planners always compute valid actions for all the robots within the time limit of each planning episode (1 second). The winner of this category has the best overall score among all eligible planners.
