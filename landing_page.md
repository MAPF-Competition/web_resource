## Introduction ![r8](./external_page_resource/images/2026_doodle/hi.jpg)

The League of Robot Runners, sponsored by Amazon Robotics, is a _competition series_ where participants tackle the core combinatorial challenges found in cooperative multi-robot coordination problems.

For the 2026 season, we are raising the bar. In addition to **task assignment 🎯** and **lifelong planning ♻️**, we are introducing **stochasticity** and **uncertainty management 🎲**. These challenges mirror high-impact industrial applications—such as warehouse logistics and advanced manufacturing—where robots must adapt to real-world imperfections and delays in real-time.

<!-- <div style="background-color:#cae8e6ff;padding:15px;margin:10px 0;display:flex;align-items:center;gap:15px;"> -->
<div style="background-color:#ffffff;padding:15px;margin:10px 0;display:flex;align-items:center;gap:15px;">
<div style="flex-shrink:0;">
<img src="./external_page_resource/images/2026/aamas.png" alt="AAMAS 2026" style="height:60px;"/>
</div>
<div>
<strong>🎉 Co-hosted with AAMAS 2026</strong>
<br/>
The League of Robot Runners 2026 is proudly co-hosted with the <a href="https://cyprusconferences.org/aamas2026/" target="_blank">25th International Conference on Autonomous Agents and Multiagent Systems (AAMAS 2026)</a>.
</div>
</div>

<!-- <img src="./external_page_resource/images/mission-4.jpg" style="margin-top:5px;width:100%;height:auto;max-width:1024px;margin-bottom:20px"/> -->

## How It Works ![r1](./external_page_resource/images/2026_doodle/work.jpg)

Participants in the League (that's you!) control a team of robotic errand runners operating in a grid environment. Their job is to finish as many tasks as possible, as quickly as possible. Your job (depending on the track) involves **Task Scheduling**, **Execution Control**, and **Path Planning**:

<div style="width:100%;text-align:center;vertical-align:top;display:flex;justify-content:center; margin-top:10px;">
<br/>
<div style="max-width: 1024px;display: flex;width: 100%;justify-content: space-between;flex-direction: row;flex-wrap: wrap;margin:10px;gap:10px;">

<div style="flex:1 1 calc(50% - 10px);padding:3px;text-align:center;min-width:160px;max-width:180px;display:inline-block;vertical-align:top;">
<img src="./external_page_resource/images/2026/task_coming.jpg" style="margin-top:5px;width:100%;height:auto;max-width:180px; border: 2px solid black; border-radius: 8px; box-shadow: 6px 6px 0px rgba(7, 142, 154, 0.3);"/>
<br/>
Tasks (orders) are continuously coming to a busy warehouse.
</div>

<div style="flex:1 1 calc(50% - 10px);padding:3px;text-align:center;min-width:160px;max-width:180px;display:inline-block;vertical-align:top;">
<img src="./external_page_resource/images/2026/task_allocation.jpg" style="margin-top:5px;width:100%;height:auto;max-width:180px; border: 2px solid black; border-radius: 8px; box-shadow: 6px 6px 0px rgba(7, 142, 154, 0.3);"/>
<br/>
Decide which robot should complete which task? It's your call!
</div>

<div style="flex:1 1 calc(50% - 10px);padding:3px;text-align:center;min-width:160px;max-width:180px;display:inline-block;vertical-align:top;">
<img src="./external_page_resource/images/2026/delays.jpg" style="margin-top:5px;width:100%;height:auto;max-width:180px; border: 2px solid black; border-radius: 8px; box-shadow: 6px 6px 0px rgba(7, 142, 154, 0.3);"/>
<br/>
Delays may happen! Your policy must handle interruptions.
</div>

<div style="flex:1 1 calc(50% - 10px);padding:3px;text-align:center;min-width:160px;max-width:180px;display:inline-block;vertical-align:top;">
<img src="./external_page_resource/images/2026/planning.jpg" style="margin-top:5px;width:100%;height:auto;max-width:180px; border: 2px solid black; border-radius: 8px; box-shadow: 6px 6px 0px rgba(7, 142, 154, 0.3);"/>
<br/>
Plan collision-free paths for a massive robot fleet to fulfill tasks.
</div>
</div>
<br/>
</div>

In 2026, we introduce **Delay Probabilities** ⚠️. Robots may not always execute their move on time due to simulated mechanical or communication delays. Your goal is not just to find a path, but to create a robust **Execution Policy** that keeps the fleet moving smoothly even when individual robots fall behind.

The competition is a great way to showcase your skills against the best in the world; **fame, glory and prizes** are all up for grabs! You can also make a tangible impact in the **research community** by establishing baselines for robust Multi-Agent Path Finding (MAPF) under uncertainty.

🛠️ **Low barriers:** We provide starter code, supporting tools, and documentation to help you quickly develop and validate your solutions.

📈 **Continuous feedback:** Submit anytime and track your progress on our live leaderboard.

📂 **Open source:** Top submissions and problem instances will be open-sourced after the competition ends.


## Eligibility and Prizes ![r2](./external_page_resource/images/2026_doodle/look.jpg)

Participation is open to individuals and teams from any discipline/background, anywhere in the world. Financial prizes (in USD) are available for **top performance** in three distinct tracks🏆:

> **Execution Track:**
> - We provide the task scheduler and path planner.
> - You create an **Execution Policy** that handle delays.
> - 🥇 First: **USD 2,500**
> - 🥈 Second: **USD 500**
> - 🥉 Third: **Fame and Fancy Certificate**
>
> **Task Scheduling Track:**
> - You assign tasks to robots. We provide path planner and execution policy.
> - Your schedule must account for the uncertainty of the execution phase.
> - 🥇 First: **USD 2,500**
> - 🥈 Second: **USD 500**
> - 🥉 Third: **Fame and Fancy Certificate**
>
> **Combined Track:**
> - You assign the tasks, plan paths, **and** control the execution.
> - Complete control for maximal efficiency in a stochastic environment!
> - 🏆 Grand Prize: **USD 5,000**
> - 🥈 Second: **USD 1,000**
> - 🥉 Third: **USD 500**

By the end of May 22nd, the top entry on the combined track leaderboard will be awarded a special **AAMAS Prize** valued at **1,000 USD**! At the end of the competition, there will also be a **Line Honours** prize for the team that computes the largest number of best-known solutions. Other notable performances will be recognized with certificates.

<!-- Find our more about the tracks and how they work on our [problem setup](./problem) and [evaluation](./evaluation) pages. -->

## Timeline ![r7](./external_page_resource/images/2026_doodle/read.jpg)
<br/>

All dates are AOE (UTC-12).

> - **Jan 2026**: Competition announcement
> - **18 March 2026**: Start kit release, open for testing
> - **1st April 2026**: Main round begins
> - **22nd May 2026**: AAMAS Prize deadline 
> - **AAMAS 2026**: AAMAS Prize announcement
> - **22th July 2026**: All tracks ends
> - **7st Aug 2026**: All tracks results announcement

<br/>

---

<div style="text-align:center;margin:20px 0;">
<p style="font-size:0.9em;color:#666;margin-bottom:10px;">Co-hosted with AAMAS 2026 | Sponsored by Amazon Robotics </p>
</div>

|     |     |     |     |     |     |     |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|![](./external_page_resource/logos/mit_logo.png) | ![](./external_page_resource/logos/monash_logo.png) | ![](./external_page_resource/logos/rutgers_logo.png) | ![](./external_page_resource/logos/uci-logo.jpg) | |  | ![](./external_page_resource/logos/amazon_robotics_logo.png) |

<link fetchpriority='high' rel="stylesheet" href="./external_page_resource/style.css" type="text/css">
