## Evaluation Process ![r2](./external_page_resource/robots/r12_s.png)

Submissions will be evaluated using an AWS cloud compute instance with the following specifications:

> - AMD EPYC 7R13 Processor with 32 vCPUs
> - 128 GiB Memory
> - Nvidia A10G GPU

The evaluation server deploys participant code into a docker environment, which is built based on a selected Docker image. It provides necessary
software and drivers for GPU- and CPU-based compute. 
The following Docker image options are available:
> 
> **PyTorch Docker Images**:
> - [pytorch/pytorch:2.5.1-cuda11.8-cudnn9-devel](https://hub.docker.com/layers/pytorch/pytorch/2.5.1-cuda11.8-cudnn9-devel/images/sha256-676c7b7423d7e726b814b98cfd5b702e1b32016b2e0ef0270f6202a6c660c419), Ubuntu 22.04 with PyTorch 2.5.1, CUDA 11.8, and cuDNN 9.
> - [pytorch/pytorch:2.5.1-cuda12.1-cudnn9-devel](https://hub.docker.com/layers/pytorch/pytorch/2.5.1-cuda12.1-cudnn9-devel/images/sha256-e8e63dd7baca894ba11fe1ba48a52a550793c8974f89b533d697784dd20a4dc0), Ubuntu 22.04 with PyTorch 2.5.1, CUDA 12.1, and cuDNN 9.
> - [pytorch/pytorch:2.5.1-cuda12.4-cudnn9-devel](https://hub.docker.com/layers/pytorch/pytorch/2.5.1-cuda12.4-cudnn9-devel/images/sha256-14611869895df612b7b07227d5925f30ec3cd6673bad58ce3d84ed107950e014), Ubuntu 22.04 with PyTorch 2.5.1, CUDA 12.4, and cuDNN 9.
> 
> **NVIDIA CUDA Docker Images**:
> - [nvidia/cuda:12.6.3-cudnn-devel-ubuntu20.04](https://hub.docker.com/layers/nvidia/cuda/12.6.3-cudnn-devel-ubuntu20.04/images/sha256-41b64c7236c0ff59f11298584676b4af95c0ddf9924f18c6072b160fddd6c34f), Ubuntu 20.04 with CUDA 12.6.3 and cuDNN 9.
> - [nvidia/cuda:12.6.3-cudnn-devel-ubuntu22.04](https://hub.docker.com/layers/nvidia/cuda/12.6.3-cudnn-devel-ubuntu22.04/images/sha256-cb239b67719dfa32ec6b525b54c1b78559bebd51a47249dd702f6c5429372154), Ubuntu 22.04 with CUDA 12.6.3 and cuDNN 9.
> - [nvidia/cuda:12.6.3-cudnn-devel-ubuntu24.04](https://hub.docker.com/layers/nvidia/cuda/12.6.3-cudnn-devel-ubuntu24.04/images/sha256-0f8250615943f311785f9ce6379a49520a4b53c124d22b42ba859edf93af3991), Ubuntu 24.04 with CUDA 12.6.3 and cuDNN 9.
> 
> **TensorFlow Docker Images**:
> - [tensorflow/tensorflow:2.18.0-gpu](https://hub.docker.com/layers/tensorflow/tensorflow/2.18.0-gpu/images/sha256-1f16fbd9be8bb84891de12533e332bbd500511caeb5cf4db501dbe39d422f9c7), Ubuntu 22.04 with TensorFlow 2.18.0 and CUDA 12.3.
> 
> **Ubuntu Docker Images**:
> - [ubuntu:jammy](https://hub.docker.com/layers/library/ubuntu/jammy/images/sha256-3d1556a8a18cf5307b121e0a98e93f1ddf1f3f8e092f1fddfd941254785b95d7), Ubuntu 22.04.

`pytorch/pytorch:2.5.1-cuda11.8-cudnn9-devel` is used as the default image. If you need a different image, please specify it in your submission.

Submissions will be evaluated on a range of distinct grid-map domains. Each
problem instance on each map features a different number of agents and a
different number of tasks. The maps are [available for
download](https://github.com/MAPF-Competition/Start-Kit/tree/main/example_problems)
and analysis . The problem instances (used in the main round) are hidden until
after the competition.

The evaluation process has two stages: offline preprocessing, where participants
can load and prepare auxiliary data, and online planning, where participants
try to complete as many tasks as possible, up to a fixed time limit.

Prizes are available for distinguished performance in three distinct tracks. 


## Domains

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


## Offline Preprocessing


During the preprocessing stage, the current map is revealed. You then have an opportunity to analyse the map and compute auxiliary data before proceeding to the evaluation stage (e.g., initialise data structures, load models, etc). Preprocessing time is limited to 30 minutes per map. Nothing you do at this stage will be counted into your final score.

## Online Planning

After preprocessing, your submission is evaluated on a set of (a priori
unknown) tasks. The starting locations of the robots and an initial set of
tasks are revealed. As robots complete tasks, more will be revealed. 

During evaluation, time progresses at a rate of 1 second per timestep. Your
submission will be evaluated for up to 5000 seconds on each map. Your job is to
complete as many tasks as possible, before a time limit is reached. 

There are three evaluation tracks: 
- **Path Planning** 
- **Task Scheduling**
- **Combined** (Path Planning + Task Scheduling)

### Task Scheduling

In this track, participants are responsible for assigning revealed tasks to
robots. At each timestep, your scheduler must return a valid task assignment
(including no assignment) for every robot. The schedule is then realised by a
`default path planner`, which decides what paths robots will take through the
environment to complete their tasks. 

At every timestep, your scheduler must compute a valid assignment for the
revealed, unallocated tasks. While you can take as long as needed to make
scheduling decisions, time continues to elapse during deliberation. 
Failure to compute a valid assignment means your robots will not complete available
tasks efficiently.

### Planner Track
In the Planner Track, participants must implement their own planner, which is responsible for planning the paths for the robots. The **default task scheduler** will be used in this track.

During the planning stage, the initial locations of the robots are revealed, and tasks—comprising sequences of errands—are assigned, one to each robot, by the default scheduler. Time progresses at a rate of 1 second per timestep, and your planner will be evaluated for up to 5000 seconds on each map.

At every timestep, your planner must compute the next valid action for each robot. While you can take as long as needed for planning, time continues to elapse during deliberation. Failure to compute the next valid action for every robot, or deliberating for longer than 1 second, will result in all robots waiting in place until the next planning episode.

### Combined Track
In the Combined Track, participants can modify **both the task scheduler and the path planner**. Both components are evaluated
together, which gives maximum flexibility over how the problem solved. 


### Scoring and the Virtual Best

Performance in each track is determined relative to a **virtual best**
baseline. The virtual best comprises all best known solutions for every
evaluation instance, as computed by any submission. For a given submission, 
the score is computed using the following formula:

>
> $$\mbox{Submission score} = \displaystyle \sum^{max}_{i=0}{\frac{\mbox{Your number of tasks finished for instance }i}{\mbox{best number of tasks finished for instance }i}}$$

<br/>

## Track Prizes

Each track has a separate
leaderboard. Participants submitting to the Combined track compete for the
grand prize. Other participants (i.e., Path Planning only or Task
Scheduling only) compete for track prizes. 

Single-track solutions are further ranked and evaluated on the Combined
leaderboard (i.e. everyone is eligible for the grand prize). 
A separate prize, also available to participants in any track, is **Line Honours**. This prize is
awarded to the team which contributes the largest number of solutions to the
virtual best solver. 

In addition to the three tracks, we keep track of who contributed the largest number of solutions to the virtual best. The submission with largest number of best solutions at the end of the competition is declared as the winner of the Line Honours prize. 

