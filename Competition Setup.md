## Problem Overview ![r13](external_page_resource/robots/r13_s.png)

A team of robots works together in a simplified grid environment. Their job is
to run infinite errands, which they accomplish by visiting different locations
on the grid. Sometimes errands must be completed in a specific order. 
A sequence of such errands is called a task. The objective is to complete as many 
tasks as possible, as quickly as possible, until time runs out. 

These types of problems are the core challenge in many real-world applications,
including warehouse logistics, multi-robot manufacturing, multi-agent computer
games and many more besides. The image below shows an example from a warehouse
domain, which we call **fulfilment**. 

<br/>

![image](external_page_resource/images/new_model.gif)

<br/>

On this page you can find further descriptions of the the problem setting, the
robot model, and the centralised controller that is responsible for plan
validation and execution. More granular technical details are available in
our competition [Start-Kit](https://github.com/MAPF-competition/Start-Kit)

## Robots and Their Environment ![r14](external_page_resource/robots/robot_on_grid_s.png)
Each grid map is deterministic, fully observable, and known ahead of time.
Robots move in parallel. Time is divided into unit-sized time steps. 

At each timestep, a robot can execute one of the following actions (see illustrations that follow): 
> - move in the robot's forward direction into an adjacent grid cell
> - rotate 90 degree clockwise 
> - rotate 90 degrees counter-clockwise
> - wait at its current location.

| `Moving Forward` |  `Rotate` |
|:---:|:---:|
| ![image](external_page_resource/images/image2.gif) | ![image](external_page_resource/images/rotate.gif)  |



An action is considered valid (or feasible) if the robot can execute that action without colliding with static obstacles in the environment or with other moving robots. Each valid action has a duration of exactly one timestep. 

Two types of collisions (i.e., invalid actions) can occur:
> - Vertex collision: two agents attempt to move to the same location at the same time.
> - Edge collision: two agents traverse the same edge from opposite directions at the same time.

| `Vertex` |  `Edge` |
|:---:|:---:|
| ![image](external_page_resource/images/vertex_conflict.gif) | ![image](external_page_resource/images/edge_conflict.gif)  |



## Tasks and Errands ![r6](external_page_resource/robots/r6_s.png) 

An **errand** is a request requiring a specific robot to visit a particular **target location** on the grid. An errand is completed when the assigned robot arrives at the designated location.

A **task** may consist of multiple errands, with the number of errands per task \( N \) ranging from \([minEPT, maxEPT]\), where \( minEPT \) and \( maxEPT \) are the minimum and maximum number of errands per task, respectively. When a task is revealed, the total number of errands, their order, and the details of each errand are disclosed. A task is completed when the assigned robot has completed all errands in the specified order.

**The objective** is to complete as many tasks as possible within the given time frame. The order of errands within a task is important and must be followed. Effective task assignment and path planning are crucial for optimal performance.

Below is an example:

1. Initially, there are three agents colored blue, yellow, and green. The cells colored pink represent potential errands that need to be assigned to the agents.

<div style="text-align: center;">
   <img src="./external_page_resource/images/img0.jpg" alt="description" style="max-width: 80%; height: auto;">
</div>

2. Each agent is assigned a task (an ordered sequence of errands). In the image, the blue agent is assigned a task consisting of five errands, while the yellow and green agents are each assigned a task consisting of three errands. The arrows indicate the possible planned path for each agent, who must follow the given order to complete the errands.

<div style="text-align: center;">
   <img src="./external_page_resource/images/img1.jpg" alt="description" style="max-width: 80%; height: auto;">
</div>

3. After completing all the assigned errands, the task of the yellow agent is considered finished. In the figure below, the yellow agent has completed its last task. 
<div style="text-align: center;">
   <img src="./external_page_resource/images/img2.jpg" alt="description" style="max-width: 80%; height: auto;">
</div>



4. Once a task is completed, an agent is assigned a new task. In the figure below, the yellow agent gets a new task containing four errands.
<div style="text-align: center;">
   <img src="./external_page_resource/images/img3.jpg" alt="description" style="max-width: 80%; height: auto;">
</div>









## The Central Controller

The central controller is responsible for the correct operation of robots in the environment. It tracks the current positions of all robots and issues commands to them, regulating their next actions.

### Planner and Path Planning

To determine which command to issue to each robot, the controller relies on a component known as **the planner**, which you must implement (for the path planning track and the combined track). The controller calls the planner at each timestep. The planner's role is to return one valid command for each robot. If the planner fails to provide a valid set of commands (one for each robot) or does not complete its computation in time, the controller instructs all robots to **wait in place** until the next timestep.

In the following example, we have illustrated two different scenarios:


- **Path with Collision:**  The "collision" figure shows a scenario where two robots’ routes intersect, leading to an expected collision. This highlights the importance of effective path planning, as failure to account for other robots' movements can result in collisions, delays, or even the failure of the robots to complete their tasks.

- **Collision-Free Path:** In contrast, the path in the "collision-free" figure is carefully planned so that the robots avoid each other entirely, finishing their tasks without any conflicts. 


<div style="text-align: center;">
   <img src="./external_page_resource/images/planning_path.png" alt="description" style="max-width: 80%; height: auto;">
</div>


### Task Assignment

In the 2024 competition, the central controller also manages **task assignment**. This involves assigning tasks, which consist of multiple errands, to the appropriate robots. Task assignment is crucial for ensuring that each robot has a specific set of errands to complete, optimizing the use of available resources and minimizing delays.

### Time Tracking and Planning Horizon

The central controller monitors the elapsed time since the start of the task (also known as **wall clock time**). Time continues to pass while the planner is deliberating. After a predetermined period, known as the **planning horizon**, the central controller stops, and the task is considered complete.

This new 2024 system ensures that the controller not only handles path planning through the planner but also efficiently assigns tasks to robots, balancing both responsibilities to achieve optimal performance.

