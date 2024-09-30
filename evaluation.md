## Evaluation Process ![r2](./external_page_resource/robots/r12_s.png)

Submissions will be evaluated using an AWS cloud compute instance with the following specifications:

> - AMD EPYC 7R13 Processor with 32 vCPUs
> - 128 GiB Memory
> - 40 GiB Storage Space
> - Nvidia A10G GPU

The evalution server evaluates participant submissions in official PyTorch docker container, which equips necessary software and drivers for Cuda and PyTorch. Once you make a submission the evaluation proceeds in two stages: offline preprocessing and online planning. 

## Offline Preprocessing
During the preprocessing stage the current map is given to each planner. The planner has the opportunity to analyse the map and compute auxiliary data before proceeding to the evaluation stage. Preprocessing time is limited to 30 Minutes per map. Nothing you do at this stage will be counted into your final score.
## Online Planning

In this competition, there are three tracks: **Scheduler Track**, **Planner Track**, and **Combined Track**.

### Scheduler Track
In the Scheduler Track, participants must implement their own task scheduler, which is responsible for assigning revealed, unallocated tasks to the robots. The **default path planner** will be used in this track.

During the task scheduling stage, the initial locations of the robots are known, and tasks are revealed to the robots gradually. Time progresses at a rate of 1 second per timestep, and your scheduler will be evaluated for up to 5000 seconds on each map.

At every timestep, your scheduler must compute a valid assignment for the revealed, unallocated tasks. While you can take as long as needed to make scheduling decisions, time continues to elapse during deliberation. Failure to compute an assignment results in all robots waiting in place until the next planning episode.

### Planner Track
In the Planner Track, participants must implement their own planner, which is responsible for planning the paths for the robots. The **default task scheduler** will be used in this track.

During the planning stage, the initial locations of the robots are revealed, and tasks—comprising sequences of errands—are assigned, one to each robot, by the default scheduler. Time progresses at a rate of 1 second per timestep, and your planner will be evaluated for up to 5000 seconds on each map.

At every timestep, your planner must compute the next valid action for each robot. While you can take as long as needed for planning, time continues to elapse during deliberation. Failure to compute the next valid action for every robot, or deliberating for longer than 1 second, will result in all robots waiting in place until the next planning episode.

### Combined Track
In the Combined Track, participants can modify **both the task scheduler and the path planner**, with both components being evaluated.





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

## Score Functions

In real-world scenarios, path planners and task schedulers are expected to excel in various aspects, such as high throughput and quick computation times. To reflect this, our competition recognizes outstanding performance across three distinct categories for each track, resulting in up to nine potential winners:

### Virtual Best and Score Function
> In this category, a `virtual best` benchmark is used to track the best known solution for each instance, across all participants. Your performance is ranked relative to this baseline using the following formula:
>
> $$\mbox{Your score} = \displaystyle \sum^{max}_{i=0}{\frac{\mbox{Your number of tasks finished for instance }i}{\mbox{best number of tasks finished for instance }i}}$$
>
> The winner in this category is the entry with the highest cumulative score. This award is given separately for each of the three tracks: **Scheduler Track**, **Planner Track**, and **Combined Track**.

### Line Honours
> In addition to the three tracks, we keep track of who contributed the largest number of best solutions across all instances. The number of best solutions achieved by any entry is tallied at the end of the competition, and the entry with the most best solutions is declared as the Line Honours.

