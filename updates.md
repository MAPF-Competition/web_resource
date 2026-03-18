## 🤖 2026 League of Robot Runners Test Round Start! 🏁 `18 Mar 2026`

**Hello Robot Runners!**

We’re excited to announce that the **2026 League of Robot Runners (LoRR)** is now open for **testing** 🎉

This year’s LoRR continues the online multi-robot challenge where tasks are revealed over time: your system must **assign tasks, plan paths, and execute safely under unexpected delays** in the competition simulator.

Teams can participate in:
- the **Task Scheduling Track** 📝 (Decide which robot does which task),
- the **Execution Track** 🧭 (Implement robust execution policies to handle uncertainty and delays), or
- the **Combined Track** 🧩 (Task scheduling, path planning and execution).

**🛠️ Updated Tools: Start-Kit & PlanViz v3.0.0**

To support the new architecture and execution uncertainty, we have released major version 3.0.0 updates for both of our core repositories.

[Start-Kit (v3.0.0)](https://github.com/MAPF-Competition/Start-Kit)

- Full support for the new Execution component and runtime delay generation.
- Added configurable action counters and multistep planner communication.

[PlanViz (v3.0.0)](https://github.com/MAPF-Competition/PlanViz)

- The visualizer fully supports 2026 tick-based simulation.
- We improved rendering performance for massive simulations.

**🧪 Join the Test Round**

The **test round** will run from **18 Mar 2026 to 31 Mar 2026**. This is the best time to:
- verify your build + submission pipeline,
- get familiar with the input/output formats,
- sanity-check your results on the public leaderboard,
- and provide feedback to us.

Note that we are still tuning the default Planner/Executor performance. The final version will be released for the **main round**.🏁

We can’t wait to see what you build this season 🏆✨


## 📣 Announcing the League of Robot Runners 2026! 📣 `05 Jan 2026`

**Hello Robot Runners!**

The wait is over! We are thrilled to officially announce the **2026 League of Robot Runners**! 🤖 ✨

Building on the massive success of the 2024/5 season—which saw record-breaking submissions and innovative solutions in task scheduling—we are raising the bar once again. For 2026, we are moving beyond perfect grids and deterministic worlds to tackle one of the biggest hurdles in real-world robotics: **Uncertainty**. 🎲

**🚀 What's New in 2026?**

In previous years, robots always did exactly what they were told. But in the real world, wheels slip, networks lag, and obstacles appear.

This year, we introduce **Delay Probabilities** ⚠️.
Robots may not always execute their moves on time. Your challenge is no longer just about finding a path; it is about creating a robust **Execution Policy** that keeps the fleet moving smoothly even when individual robots fall behind.

The League of Robot Runners 2026 is proudly co-hosted with the [25th International Conference on Autonomous Agents and Multiagent Systems (AAMAS 2026)](https://cyprusconferences.org/aamas2026/).

**🏆 New Tracks and Challenges**

To accommodate these changes, we have restructured the competition into three new tracks:

* **Execution Track ⚙️:** We provide the task scheduler and path planner. You build the policy to navigate robots safely through stochastic delays.
* **Task Scheduling Track ⏱️:** We provide path planner and execution policy. You build the scheduler that assigns tasks to thousands of robots.
* **Combined Track 🏆:** The ultimate challenge! Everything is under your control for maximal efficiency.

**📅 Competition Timeline**

Mark your calendars! The race continues in early 2026:

* **Mid-February 2026:** 🛠️ **Start-Kit Release & Test Round.** Open for testing and warm-up.
* **Mid-March 2026:** 🏁 **Main Round Begins.** The official leaderboard goes live!
* **Early May 2026:** 🛑 **Main Round Ends.**
* **AAMAS 2026:** 🥇 **Winners Announcement.** Results will be presented at the AAMAS conference.

Stay tuned for further details in the coming weeks. We can't wait to see how you handle the chaos!

## 🎥 Watch the 2025 Virtual Expo Recordings Online! `18 Jul 2025`

**Hello Robot Runners!**

Missed the 2025 Virtual Expo or want to re-watch a favorite session? All talk recordings and technical reports are now available\!

Catch up on the insights and innovations from our top teams and experts by exploring the full schedule:

- [Event Website](https://expo25.leagueofrobotrunners.org/schedule/)  
- [Youtube Playlist](https://youtube.com/playlist?list=PLlLnPGrmVZcOrQ_X__5Lqo9zaD6dHQg34&si=dSatQp5Z9vPPot0a)


## 📢Call For Participation: 2025 League of Robot Runners Virtual Expo  `21 May 2025`

Hello Robot Runners\!

This is a call for participation in the [**https://expo25.leagueofrobotrunners.org**](https://expo25.leagueofrobotrunners.org).

The League of Robot Runners is a competition series that tackles one of the most challenging problems in automated logistics: scheduling tasks and coordinating a team of moving robots. 

In 2024/5 The League received a total of 1513  submissions from 50 teams worldwide, which is a big success\! To celebrate, we are holding a **Virtual Expo** \--- a free online event where we highlight the community’s progress and achievements thus far and look ahead at the challenges that yet remain. The expo is a fantastic opportunity to learn more about the problems being tackled in the competition, their importance to industry, and the experiences, insights, and innovative approaches of leading participants. 

**Program Highlights:**

The technical program will feature a number of sessions that will be of interest to competition participants and members of the broader MAPF community:

* Keynote from distinguished speakers across industry and academia:   
  * Alex Barbosa (Amazon Robotics)   
  * Amanda Porok (Cambridge University).  
* Highlights and awards from the 2024/5 main round: celebrate with us\!  
* Technical talks from successful participants.  
* Community discussion: reflections on the competition initiative and exciting news about the future competition.

We encourage all interested individuals to join us for this exciting occasion\! This includes past participants, interested future participants and members of the broader research community with an interest in Multi-Agent and/or Multi-Robot Path Planning.

**Event Details:**

* Date: June 2nd, 2025  
* Time: 0900 EDT (UTC-4)  
* Location: the event will be held online via Zoom

**Registration:**

Secure your spot via the event website: [https://expo25.leagueofrobotrunners.org/registration/](https://expo25.leagueofrobotrunners.org/registration/). Once registered, you will receive email instructions for the details of joining the Virtual Expo.

We look forward to your participation in this exciting event\!

## 🔥Resource Release: Benchmark and Code Archive\!🔥 `09 May 2025`

**Hello Robot Runners\!**

We are glad to announce the release of two new resources for the community: the 2024 Benchmark Archive and 2024 Code Archive. These repositories gather together all of your best submissions from the most recent competition (2024/5), together with all problem instances and all known best solutions. All solutions can be downloaded and analysed with [PlanViz](https://github.com/MAPF-Competition/PlanViz), our offline visualisation tool. 🥁🥁🥁

These resources will help us to track how much progress we are making on the core challenges associated with planning and coordinating teams of real robots. Researchers in the area (that’s you\!) can use these resources to further develop and compare their algorithms against the established state-of-the-art. Meanwhile, newcomers to the area also get a leg up\! They can start with working implementations and build their new ideas upon best-known solution techniques.🔥🔥🔥

💯In the [Benchmark Archive](https://github.com/MAPF-Competition/Benchmark-Archive), you will find:

* Main round evaluation instances.  
* Test round evaluation instances.  
* Example instances, released as part of the competition start-kit.  
* Best-known solutions to all evaluation instances.  
* Benchmark generator, which we used to produce all the problem instances.  
* Tables that describe the configuration of each benchmark instance, metrics describing the best-known solution for that instance, links to download the solutions and links to the implementation which produced that solution. 

📂In the [Code Archive](https://github.com/MAPF-Competition/Code-Archive), you will find:

* Implementations for the best submission of each team on the final leaderboard of the Combined, Planning, and Scheduling categories.  
* Implementations that produced any best-known solution for each evaluation instance.  
* Tables that record the metrics of each archived implementation.

## 📢 \[CFP\] 2025 League of Robot Runners Virtual Expo `21 Apr 2025`

[**https://expo25.leagueofrobotrunners.org**](https://expo25.leagueofrobotrunners.org)

**Hello Robot Runners!**

We invite all teams and team members from the League of Robot Runners to participate in our 2025 Virtual Expo, which takes place online on June 2nd, from 9 am EDT (UTC-4).

The expo is a community event where we celebrate and reflect on the recent competition round. It is an opportunity for participants to share their experiences and insights into the challenge problems, to tell the community about their innovative approaches, and to celebrate the performances that helped make the inaugural League of Robot Runners such a memorable success\!

To participate in the program teams and team members will submit a technical report on a relevant topic, as described in the Topics of Interest. Following a light review, selected works will be presented to the community, in the form of a technical talk. Written reports, and video recordings of the talks, will be made available for download during and after the expo.

**Program Highlights:**

The technical program will feature a number of sessions that will be of interest to competition participants and members of the broader MAPF community:

* Keynote speakers from Industry and Academia.  
* Awards Ceremony, to celebrate distinguished and noteworthy performances.  
* Technical talks from competing teams and team members.  
* Community meeting, to discuss the future direction of the competition.

**Topics of Interest:**

We invite submissions related to any aspect of the League of Robot Runners. This includes but is not limited to: 

* Description of systems (algorithms, implementations) used in the competition.  
* Post-competition data-analysis, including tools and methodologies.  
* Position papers, reflecting on the competition setup, goals or any other related issues that will be of interest to the community.  

Submissions are non-archival. They can describe recently published work or work that is under submission elsewhere, or encouraging preliminary results from works in progress.

**Submissions:**

Submissions take the form of a technical report describing a topic of interest and must be in AAAI style (see instructions in the [Author Kit](https://aaai.org/authorkit25/)).  The submission type can be any of the following: 2-page extended abstract or 4-page short paper or 8-page long paper, plus 1 additional page for references.  Certain types of submissions are better suited for certain types of topics; for example, authors of system descriptions may wish to aim for a longer paper, as this helps future replication and extension studies. Each submission will undergo a light review process, single-blind, to ensure an acceptable quality. Submissions must be timely and are made via EasyChair at [https://easychair.org/conferences/?conf=lorr2025](https://easychair.org/conferences/?conf=lorr2025). 

**Important Dates:**

* Abstract deadline: 9th May 2025  
* Submission deadline: 20th May 2025  
* Paper notification: 26th May 2025  
* Final version: 1st June 2025

All deadlines are “anywhere on earth” (UTC-12). 

For any questions about this call, please reach out via email to the following address: [league-of-robot-runners@googlegroups.com](mailto:league-of-robot-runners@googlegroups.com).

We look forward to your submissions\!  

## 🎉Results Announcement for Main Round 2024!🎉  `14 Mar 2025`

**Hello Robot Runners!**

Since the end of Main Round 2024, our organising team has been working diligently to verify the final rankings on the leaderboard. With this thorough review now complete, we are excited to announce the official winners! 🎊🎉🏆

**🏅 Award Winners 🏅**

Participants in the 2024 League of Robot Runners were evaluated across four distinct performance tracks 🔥, each designed to highlight crucial challenges for real-world robotics practitioners. We are awarding one 💸 grand prize for each track and 🥁 distinguished performance awards for the runners-up!

* **Combined Track: 🏆** This category rewards the highest overall score in the competition. The core challenge is to effectively integrate planning and scheduling algorithms for peak performance.
* **Planner Track: 🗺️** This category rewards the highest achieved score in the Planning Track. The core challenge is to develop efficient algorithms for optimising robot movement, given a set of default task assignments.
* **Scheduler Track: ⏱️** This category rewards the highest achieved score in the Scheduler Track. The core challenge is optimising robot task assignments	, given a default strategy for planning robot movements.

<table>
  <tr>
   <td>
   </td>
   <td>
<strong>🏆Combined Track</strong>
   </td>
   <td><strong>🗺️Planner Track</strong>
   </td>
   <td><strong>⏱️Scheduler Track</strong>
   </td>
  </tr>
  <tr>
   <td>💸Grand Prize
   </td>
   <td>🥇Team No Man's Sky
   </td>
   <td>🥇Team No Man's Sky
   </td>
   <td>🥇Team No Man's Sky
   </td>
  </tr>
  <tr>
   <td rowspan="2" >🥁Distinguished Performance
   </td>
   <td>🥈Team Kitty Knight
   </td>
   <td>🥈Team SYSU-LCIS
   </td>
   <td>🥈Team verstand
   </td>
  </tr>
  <tr>
   <td>🥉Team SYSU-LCIS
   </td>
   <td>🥉Team RAPID
   </td>
   <td>🥉Team Zn
   </td>
  </tr>
</table>

Finally, we have the **Line Honours** award, which recognises the team with the largest number of best-known solutions across all problem instances. The winner of this award is: 🎗️Team No Man's Sky.

Congratulations to all our winners and to every participant in the 2024 League of Robot Runners! 🫡 Your dedication, ingenuity, and many contributions are the driving force behind the competition's resounding success. Thank you for being part of this incredible journey! ❤️

We will be reaching out ✉️ to each winning team shortly to confirm details for the ✍️ issuance of certificates and the 📬 distribution of prizes.

**📝 Next Steps 📝**

Building on the momentum of the 2024 competition, we are excited to announce the following community initiatives in the weeks ahead:

* 📂 **Code Release:** We will soon archive and open-source the top-performing submission code from each team featured on the leaderboard. This allows others to learn from past successes and lowers entry barriers for new participants that wish to join the League.
* 💯 **Data Release:** We will release all problem instances and the best-known plans for each instance, as computed during the competition period. This release creates a new benchmark set for the community and supports further research in the area. 
* 🙋 **Problem Generator Release:** We will make available the scripts used to create all problem instances in the 2024 Main Round. With this tool anyone can create new instances and customised challenges, so as to further explore and push forward the boundaries of the problem domain.
* 🎟️ **Virtual Showcase Event:** In May 2025, we will hold a virtual event where selected participants can present their approaches and share their insights from the competition. The Virtual Expo enables dissemination and knowledge exchange in our community. Participants will also have an opportunity to discuss the current and future directions of the League of Robot Runners.

**🎯 Beyond the Horizon 🎯**

The League of Robot Runners will return in 2025 with more exciting challenges and innovations! 🔥🔥🔥. Stay tuned for the official announcement as we continue to bridge the exciting frontier between robotics and artificial intelligence!  


## 🏁 Main Round 2024: Mission Accomplished! 🏁 `18 Feb 2025`

**Hello Robot Runners!**

The word is out – we've officially crossed the Main Round 2024 finish line! The submission portal is now closed, and the final evaluations are complete. That's a wrap on the second exciting race of the League of Robot Runners! 🏁
Congratulations to each and every participant, and thank you for contributing to another incredibly successful competition! 🤖 💘

This year, we've seen incredible engagement! A record-breaking total of 1513 submissions poured in from 50 teams across the globe 🔥🔥🔥. It's inspiring to witness the diverse approaches you've each taken to the challenges, generating countless thrilling moments throughout the competition.

In the coming two weeks, our team will be diligently 🔍 reviewing all submissions 🔍 to ensure everything aligns with the competition rules and guidelines. We plan to announce the official winners around March 2nd, and prizes 🎁 will be awarded shortly afterwards.

Following the results announcement, we will archive and open source your top submissions (along with supplementary data to our large file storage). We will also record and archive the best-known solutions for every problem instance and we will release tools that can generate similar benchmarks. These resources help others to 📚 build upon your achievements 📚 and they help to grow our community, by lowering the barrier of entry into the area. We encourage everyone to leverage these resources and to continue pushing the boundaries of robot running in the post-competition period.

Your input is invaluable as we shape the future of the League. Please share any thoughts or insights you've gained during the competition period via the  feedback channel 📝 on our Discord, or by  📨 email. We read and consider all your feedback and we genuinely appreciate your input. 🤝 

Once again, thank you for making the 2024 Main Round such a resounding success. Stay tuned for news about what's coming next as the League of Robot Runners continues to grow and evolve!🌱

## 🧰 Start-kit v2.1.2 Released! 🧰 `20 Jan 2025`

**Hello Robot Runners!**

We have released the Start-kit v2.1.2, which includes fixes for issues when an agent's task is abandoned without re-assigning.
* **What's changed?**  View the [changelog](https://github.com/MAPF-Competition/Start-Kit/blob/main/Changelog.md) for more details.
* **Upgrade now:**  Follow the [update instructions](https://github.com/MAPF-Competition/Start-Kit?tab=readme-ov-file#upgrade-your-start-kit) to get the latest version.

## 🚀 New Features: Custom Docker Images & More Submission Info! 🤖 `23 Dec 2024`

**Hello Robot Runners!**

We've added two new features to enhance your 2024 League of Robot Runners experience, according to your feedback! 🎉:

**Choose Your Base Docker Image:**

   - You can now select your preferred base Docker image for building your evaluation environment!
   - Find the new option in the `My Submission` page when creating a new submission.
   - More details on available images: [leagueofrobotrunners.org/evaluation](https://leagueofrobotrunners.org/evaluation)

**Submission History Table Upgrade:**

   -  Quickly view your **Score**, **Short Commit SHA**, and **Commit Message** directly in the table!
   -  No need to open each submission for key details.

We hope these updates make your competition journey more enjoyable! 🚀

## 🤖 2024 League of Robot Runners Main Round Start! 🏁 `17 Nov 2024`

**Hello Robot Runners!** 

The 2024 League of Robot Runners Main Round is here!  🎉 🎉 🎉 

The competition period runs from 17 Nov 2024 to 16th Feb 2025 (3 whole months!) and brings a whole new level of challenge, with:
- **more** problem instances, 🤖 
- **more** errands per task, 📦
- **different** task distributions across maps. 💪

With 42 teams already registered for the competition, the race for first is sure to be intense! 🏆

Fame, glory and prizes are all up for grabs! 
We have a `$5,000 Grand Prize` for the 
`Combined Track` winner and two 
`$2,500 First Place Prize` for top performers in the 
`Path Planning` and `Task Scheduling Tracks`! 

A limited number of training awards are still available. Valued at **$1000** and distributed based on merit. These awards can help your develop algorithms that require intensive offline training and precomputing (e.g. ML and RL).

**🚀 Software Updates Based on Your Feedback! 🚀**

A huge thank you to everyone who participated in the test round and provided invaluable feedback! 🙏  Based on your suggestions, we've happy to announce new versions of our competition software. Here's what's new:

- **Start-kit v2.1.0:** We've streamlined the start-kit with additional documentation, bug fixes, and optimisations. View the [changelog](https://github.com/MAPF-Competition/Start-Kit/blob/main/Changelog.md) for more details. 👈  **Important note:** This release introduces requested API changes. As a result, you may need to make minor revisions to your submissions. Our [update Instructions](https://github.com/MAPF-Competition/Start-Kit?tab=readme-ov-file#upgrade-your-start-kit) will guide you through this process.
- **PlanViz v2.1.0:**  Our solution visualiser has also recieved an upgrade, with new features to help you develop better strategies and algorithmic insights. View the [changelog](https://github.com/MAPF-Competition/PlanViz/blob/main/Changelog.md) for more details.
- **Better auxiliary data support:** We add new features to the evaluation environment to help you access large size dependencies at compilation and runtime. View our updated [documentation](https://github.com/MAPF-Competition/Start-Kit/blob/main/Working_with_Preprocessed_Data.md) for more details.


Keep an eye out for further news and announcements during the competition period.  


## 🚀 Test Round Extended! More Time to Tinker & Tweak! 🤖 `1 Nov 2024`

**Hello Robot Runners!**

We hope you're having a blast in the current test round of the 2024 League of Robot Runners! 🎉

A huge **THANK YOU** to everyone who submitted solutions and shared their feedback! 🌟 Your insights on the competition setup, evaluation process, and start-kit are super valuable. We're hard at work squashing issues and implementing features based on your suggestions. 🛠️

To give everyone extra time to prepare their implementations we will extend the test round for two weeks! 🗓️ This also gives us extra time to finalise the competition setup ahead of the main round. 🤖✨

**Mark your calendars!** The main round will begin on **15th November 2024**. 🗓️ We’re looking forward to your amazing solutions. Until then, please don’t hesitate to contact us with your questions or further feedback. 🎙️

Best regards,
The Organisers


## 🤖 2024 League of Robot Runners Test Round Start! 🏁 `4 Oct 2024`

**Hello Robot Runners!** 

We are glad to announce that the 2024 League of Robot Runners (LoRR) is ready for testing!  🎉

The 2024 Edition of LoRR introduces a task allocation challenge where errands must first be assigned to robots 🤖, after which paths are planned to fulfill the assigned tasks. A team may choose to participate in the `Task Scheduling Track`📝,  the `Path Planning Track`🗺️, or the `Combined Track`🏇🏼! 

The test round will run during the month of October. It is an opportunity for everyone to become familiar with the environment. The main round will begin in early November and runs until February 2025 🏁.

We hope you can join us for this exciting new season 🏆!


## New Resource Release: 🌟 Problem Generator and Virtual Expo Recordings 🌟 `15 Jul 2024`

**Hello Robot Runners!**

We are glad to announce the release of two new resources for our community: the **2023 Competition Problem Generator** and **Virtual Expo Recordings**!

🚀 [**Problem Generator**](https://github.com/MAPF-Competition/Benchmark-Archive/tree/main/2023%20Competition/Problem%20Generator)

Perfect for those eager to generate their own benchmark instances, the 2023 Competition Problem Generator is packed with the following tools:

* **benchmark_generator.py**: Craft new problem instances with either randomly generated errands or pre-configured errand sets. 📊
* **warehouse_map_generator.py**: Create your own warehouse maps featuring various types of picking stations and emitters with just a few commands. 🏗️
* **warehouse_task_generator.py**: Generate tailored task sets for your custom warehouse maps according to specific distribution requirements. 🧩

Comprehensive documentation and tutorials are included to ensure you get the most out of these tools. 📚

🎥 [**Virtual Expo Recordings**](https://expo24.leagueofrobotrunners.org/schedule/) 

Missed our live sessions? No worries! All the exciting talks from the 2024 League of Robot Runners Virtual Expo are now available online. Check out the[ Expo Schedule](https://expo24.leagueofrobotrunners.org/schedule/) to access all the recordings. Dive into the insights and innovations shared by leading experts right from the comfort of your home! 🎤📹

Stay tuned for more updates on the 2024 Competition! 🏁🤖

## Call For Participation: 2024 League of Robot Runners Virtual Expo `2 May 2024`

**Hello Robot Runners!**

The League of Robot Runners is a competition series that tackles one of the most challenging problems in automated logistics: coordinating a team of moving robots. Such problems often appear in the research literature, where they are modelled and solved using a variety of simplifying assumptions. The League of Robot Runners aims to bridge the gap, between academia and industry, by identifying the core combinatorial challenges that make robot coordination problems difficult to solve, in practice.

The first round of this competition was held in 2023 and received a total of 825 submissions from 25 teams worldwide, which is a big success! To celebrate, we are holding a **Virtual Expo** --- a free online event where we highlight the community’s progress and achievements thus far and look ahead at the challenges that yet remain.

The expo is a fantastic opportunity to learn more about the challenging problems being tackled by the competition, their importance to the industry, and the experiences, insights, and innovative approaches of leading participants. 

**Program Highlights:**

The technical program will feature a number of sessions that will be of interest to competition participants and members of the broader MAPF community:

* Industry keynote from Federico Pecora (Amazon Robotics): hear about the many challenges and opportunities in this exciting research area
* Highlights and awards from the 2023 main round: celebrate with us!
* Technical talks from successful participants: hear experiences, insights and more.
* Community discussion: reflections on the competition initiative and exciting news about the 2024 main round.

We encourage all interested individuals to join us for this exciting occasion! This includes past participants, interested future participants and members of the broader research community with an interest in Multi-Agent and/or Multi-Robot Path Planning.

**Registration:**

Secure your spot via the event website: [https://expo24.leagueofrobotrunners.org/registration/](https://expo24.leagueofrobotrunners.org/registration/). Once registered, you will receive an email with further instructions and links to our Zoom Session.

We look forward to your participation in this exciting event!

## 🔥Resource Release: Benchmark and Code Archive!🔥 `4 April 2024`

**Hello Robot Runners!**

We are glad to announce the release of two new resources for the community: the Benchmark Archive and the Code Archive. These repositories gather together all of your best submissions from the 2023 competition, together with all problem instances and all known best solutions. 🥁🥁🥁

These resources will help us to track how much progress we are making on the core challenges associated with planning and coordinating teams of real robots. Researchers in the area (that’s you!) can use these resources to further develop and compare their algorithms against the established state-of-the-art. Meanwhile, newcomers to the area also get a leg up! They can start with working implementations and build their new ideas upon best-known solution techniques.🔥🔥🔥

💯In the [Benchmark Archive](https://github.com/MAPF-Competition/Benchmark-Archive), you will find:

* Example instances, released with the start-kit.
* Main round evaluation instances.
* Test round evaluation instances.
* Best-known solutions to all evaluation instances.
* Tables that describe the configuration of each benchmark instance, metrics describing the best-known solution for that instance, links to download the solutions and links to the implementation which produced that solution. 

All the best-known solutions can be downloaded and analysed with [PlanViz](https://github.com/MAPF-Competition/PlanViz), our offline visualisation tool (previously open-sourced in 2023).

📂In the [Code Archive](https://github.com/MAPF-Competition/Code-Archive), you will find:

* Implementations for the best submission of each team on the final leaderboard of the Fast Mover and Overall Best categories.
* Implementations that produced any best-known solution in the Line Honours category.
* Tables that record the metrics of each archived implementation.

We are also finalising the release of a benchmark generator, which we used to produce all the problem instances.**💪** Once done, we will push an update to the benchmark archive and send a further announcement.📢


## Call For Submissions: 2024 League of Robot Runners Virtual Expo `7 Mar 2024`

**Hello Robot Runners!**

We invite all teams and team members from the League of Robot Runners to participate in our [2024 Virtual Expo](https://expo24.leagueofrobotrunners.org), which takes place online on May 20th, from 1530 EDT (UTC-4). 

The expo is a community event where we celebrate and reflect on the recent competition round. It is an opportunity for participants to share their experiences and insights into the challenge problems, to tell the community about their innovative approaches, and to celebrate the performances that helped make the inaugural League of Robot Runners such a memorable success!

To participate in the program teams and team members will submit a technical report on a relevant topic, as described in the Topics of Interest. Following a light review, selected works will be presented to the community, in the form of a technical talk. Written reports, and video recordings of the talks, will be made available for download during and after the expo.

**Program Highlights:**

The technical program will feature a number of sessions that will be of interest to competition participants and members of the broader MAPF community:

* Industry Keynote from Amazon Robotics.
* Awards Ceremony, to celebrate distinguished and noteworthy performances.
* Technical talks from competing teams and team members.
* Community meeting, to discuss the future direction of the competition.

**Topics of Interest:**

We invite submissions related to any aspect of the League of Robot Runners. This includes but is not limited to: 

* Description of systems (algorithms, implementations) used in the competition.
* Post-competition data-analysis, including tools and methodologies.
* Position papers, reflecting on the competition setup, goals or any other related issues that will be of interest to the community.

Submissions are non-archival. They can describe recently published work or work that is under submission elsewhere, or encouraging preliminary results from works in progress.

**Submissions:**

Submissions take the form of a technical report describing a topic of interest and must be in AAAI style (see instructions in the [Author Kit](https://aaai.org/aaai-conference/submission-instructions/)).  The submission type can be any of the following: 2-page extended abstract or 4-page short paper or 8-page long paper, plus 1 additional page for references.  Certain types of submissions are better suited for certain types of topics; for example, authors of system descriptions may wish to aim for a longer paper, as this helps future replication and extension studies. Each submission will undergo a light review process, single-blind, to ensure an acceptable quality. Submissions must be timely and are made via EasyChair at [https://easychair.org/conferences/?conf=lorr2024](https://easychair.org/conferences/?conf=lorr2024). 

**Important Dates:**

* Submission deadline: 14th April 2024
* Paper notification: 1st May April 2024
* Final version: 10th May 2024

All deadlines are “anywhere on earth” (UTC-12). 

For any questions about this call, please reach out via email to the following address: [organisers@leagueofrobotrunners.org](mailto:organisers@leagueofrobotrunners.org).

We look forward to your submissions!


## 🎉Results Announcement for Main Round 2023!🎉 `22 Dec 2023`

**Hello Robot Runners!**

Since the end of the competition 🎬, our organising team has been busy verifying the final standings on the leaderboard. With that work now complete we are now ready to announce the official winners of the main round for 2023! 🎊🎉🏆

We also discuss 🤔 the next steps for the League of Robot Runners and associated community initiatives**📝**, all coming up in 2024. 

**🏅 Award Winners 🏅**

Participants in the 2023 League of Robot Runners were evaluated in 3 distinct performance categories 🔥, each highlighting a distinct challenge that is faced by industry practitioners. There is one 💸 **grand prize** for each category and 🥁 **distinguished performance awards** for runners-up. 

* **Fast Mover: ☄️**This category rewards the highest achieved score, subject to a 1-second limit on each planning episode. The main challenge in this case is effective performance under time pressure. 
* **Line Honours: 🎗️**This category rewards the largest number of best-known solutions across the evaluated problem instances. The main challenge in this case is to achieve the highest possible solution quality.
* **Overall Best: 🏆**This category rewards the highest achieved score across all evaluation instances. The main challenge is to maximise the global performance.

<table>
  <tr>
   <td align="left">
   </td>
   <td align="left"><strong>☄️Fast Mover</strong>
   </td>
   <td align="left"><strong>🎗️Line Honours</strong>
   </td>
   <td align="left"><strong>🏆Overall Best</strong>
   </td>
  </tr>
  <tr>
   <td align="left" rowspan="2" ><strong>🥁Distinguished Performance</strong>
   </td>
   <td align="left"><em>🥈Team Shadoks</em>
   </td>
   <td align="left"><em>🥈Team Pikachu</em>
   </td>
   <td align="left"><em>🥈Team Shadoks</em>
   </td>
  </tr>
  <tr>
   <td align="left"><em>🥉Team NCD-MIPT</em>
   </td>
   <td align="left"><em>🥉Team NCD-MIPT</em>
   </td>
   <td align="left"><em>🥉Team NCD-MIPT</em>
   </td>
  </tr>
  <tr>
   <td align="left"><strong>💸Grand Prize</strong>
   </td>
   <td align="left"><em>🥇Team Pikachu</em>
   </td>
   <td align="left"><em>🥇Team Shadoks</em>
   </td>
   <td align="left"><em>🥇Team Pikachu</em>
   </td>
  </tr>
</table>

We will get in touch ✉️ with each team to confirm their details for the ✍️issuance of certificates and the 📬distribution of the prizes in January.

**📝 Community Initiatives 📝**

As we move forward, we're excited to announce our plans for the League of Robot Runners and associated community initiatives:

* 📂We will soon archive and open-source the most successful submission codes from every team on the leaderboard. This allows us all to learn from one another and lowers the barrier of entry for newcomers.
* 💯We will soon share all problems and every best-known plan for each instance. Such comparisons help the community track progress in the area.
* 🙋We will soon release our problem generator so that others can create more diverse and more challenging instances in the same general style. 
* 🎟️We will soon invite participants to write about their submissions and present their ideas in a virtual event in 2024. This allows us to disseminate directly what ideas worked well, explain their limitations and identify interesting new directions.

**🎯Future Competitions 🎯**

The League of Robot Runners will return in 2024🔥🔥🔥! You can expect new setups and fresh challenges to test your problem-solving and implementation skills💪. Look out for the announcement as we work to bridge the gap 🫸~~~🫷 between robotics and AI!

Finally, we extend our sincerest 🫡gratitude -- and congratulations 🎉! -- to each participant in 2023. Without your hard work and many contributions, the competition could not have achieved the success it has. Thank you! ❤️



## 🎉 Finish Line! End of Main Round 2023 🎉 `2 Dec 2023`

**Hello Robot Runners!**

We recently crossed the deadline for Main Round 2023! The last submissions are in and now fully evaluated. This means we’ve reached the 🏁 **end of the race** 🏁 for the inaugural League of Robot Runners! 

And what a race it was! What a finish! It’s been amazing tracking your progress throughout and keeping up with the many ⬇️ twists and turns ⬆️ as teams traded places on the leaderboard. **Congratulations to all of our participants** and thank you for making the competition such a big success! 🤖 💘

During the main round, we received a total of 825 submissions from 25 teams worldwide 🔥🔥🔥. Participants tackled the challenge problems from a variety of diverse perspectives and these efforts produced many exciting moments throughout the race. Over the next two weeks, we will 🔍 review all submissions 🔍 to ensure they comply with the wording of the rules and the spirit of the competition. 

There will be an official **winners announcement** later this month and prizes 🎁 will be disbursed in the new year. 

Once the results are finalised, we will archive and open source your best submissions (and associated auxiliary data, uploaded to our large file storage). We will also record and archive the best-known solutions for every instance and we will release tools to generate similar benchmarks. These initiatives will allow every participant to continue developing their approaches and measuring their progress in the post-competition period. It also allows the broader community to 📚 build on your success. 📚

But the competition journey doesn't end here! The League of Robot Runners will return in 2024 with new challenges, changes and improvements! Stay tuned for the upcoming call!

Finally, we value your thoughts and experiences. If you have any feedback or insights for the competition this year, we encourage you to share them in the feedback channel on our Discord or reach us through email. We take all your feedback seriously, we will use it to shape the future of the League of Robot Runners.

**🎆 Thank you again for making the 2023 Main Round a resounding success! 🎆**

Best regards,

The League of Robot Runners Organising Committee.


## Emergency Fix: Start-kit V1.1.5 Release `21 Nov 2023`

**Hello Robot Runners!**

We found the previous release introduced a bug:beetle: , which will crash the program if the logger file is not specified in CLI. We are very sorry for the inconvenience introduced here. The new release comes with an emergency fix on the bug.  

More details are available in the changelog: https://github.com/MAPF-Competition/Start-Kit/blob/main/Changelog.md

Follow the upgrade instructions to update your implementation: https://github.com/MAPF-Competition/Start-Kit/tree/main#upgrade-your-start-kit


## Software Update: Start-kit V1.1.4 Release `18 Nov 2023`

**Hello Robot Runners!**

Thanks to invaluable feedback from our robot runner community. We discovered a few issues in the start-kit implementation that may cause inconvenience to participants. 

We have released Startk-kit V1.1.4 with the following updates:
- Fixed a bug causing segmentation fault on preprocess timeout. Preprocess timeout will now terminate the program with exit code 124.
- Fixed a bug causing segmentation fault on reading env->goal_locations when the plan timelimit exceeded.
- Updated documentation to better explain online timeout behaviour and preprocess timeout behaviour.

More details are available in the changelog of the Start-kit: https://github.com/MAPF-Competition/Start-Kit/blob/v1.1.4/Changelog.md

Click the link to get Instructions on upgrading your code: https://github.com/MAPF-Competition/Start-Kit/tree/main#upgrade-your-start-kit



## 🚀 Announcement: Half-way there! New Resources and Software Updates! 🚀 `27 Oct 2023`

### Hello Robot Runners!

We are more than half-way in the main round -- can you believe it? There are now many submissions from teams all over the world and the leaderboard has 🧨 lit up! 🎆 Make sure to keep an eye on the latest standings so that your team doesn’t get left behind!

In this newsletter we describe a number of recent updates to the competition website, and the start-kit software and we announce new resources for participants -- all to help you get that winning edge! Let’s dive right in!


### 1. Website Updates

We have improved the leaderboard in a variety of different ways, making it easier than ever to track your progress 🤖 and those of other teams **🖥️**.



* Team names are now shown alongside their Algorithm name. We added this feature as algorithmic approaches may change over time.
* We added a new “All Submissions” tab to the leaderboard. This helps you keep an eye on submissions from other teams. Who submitted what and when!
* We added a Trend plot for the Line Honours category. This allows you to see more easily who is making progress in the race!
* Fixes for a variety of visual bugs. 

### 2. Software Updates

We have updates for both the Start Kit software and for PlanViz, our offline visualiser. See the [upgrade instructions](https://github.com/MAPF-Competition/Start-Kit#upgrade-your-start-kit) and make sure your code is up to date!

Start Kit updates:



* We fixed a small bug affecting participants developing with python.
* We added extra documentation to help participants working with preprocessed data.
* We added extra “Debug and Visualise” documentation, to help participants diagnose and fix problems with their planners. 
* We added different logging levels, which makes it easier to parse and work with output files.
* Refer to the [changelog](https://github.com/MAPF-Competition/Start-Kit/blob/main/Changelog.md) for more details.

PlanViz updates:



* We added agent-based filters which simplify what is being shown. This helps you more easily find agents of interest.
* We improved support for visualising plans with invalid actions. This makes it easier to understand what went wrong and why.
* We added additional documentation, to help you use PlanViz more effectively
* We added support for visualising MAPF (i.e., no rotations) plans, a popular and closely related problem to the problem that we tackle in the competition.
* We added a new Tracker Transfer tool, to convert plans from the MAPF Tracker community website (more on this below!)  to the PlanViz format.
* Again, refer to the [changelog](https://github.com/MAPF-Competition/PlanViz/blob/main/Changelog.md) for more details!


### 3. Training Data!

Community resources can be invaluable for researchers. One such resource, that may be of interest to participants in the League of Robot Runners, is the **MAPF Tracker ([http://tracker.pathfinding.ai/](http://tracker.pathfinding.ai/))**. This is a new website and database that records best-known solutions on a range of popular benchmarks for the related Multi-Agent Path Finding (MAPF) problem. 

MAPF can be understood as a special case of the Robot Runners problem model. In particular, there is only one task per agent and agents do not have any facing direction, which means they do not need to turn. Since the two problems are very similar, insights into one can help improve performance on the other. In this update we explore some ideas for how your team could make use of this new resource.

**Browse the database and be inspired!**

We seeded the MAPF Tracker with a variety of results from recent and state-of-the-art MAPF algorithms, and on grid maps which are similar to those used in the competition. Using the website allows you to compare, in a non-competitive setting, the success rates and achieved costs of different and successful planning techniques. The MAPF Tracker contains a range of metadata for each claim, allowing you to locate relevant papers, follow links to author implementations and build on those ideas to improve your own submissions

**Analyse solutions and learn from the best!**

In addition to summary results the MAPF Tracker also contains a wealth of optimised plans, for thousands of instances and across many different domains. Each plan can be downloaded and visualised in [PlanViz](https://github.com/MAPF-Competition/PlanViz) (our offline visualisation tool, developed specifically for the competition) which helps you obtain new insights into the combinatorial challenges at the heart of these problems. Plans can also be downloaded en masse, which means the data could be used for training, to automatically learn new cooperative strategies and to get an edge in the competition

**Chart your own course!**

So far we have suggested a few possible starting points. However, we encourage participants to develop their own ideas and to find new ways of exploiting MAPF data, so as to improve their standing in the League of Robot Runners competition. We look forward to your submissions and to seeing what you can come up with!

Good luck!

## 🔥 The main round is here! 🔥 `30 Aug 2023`

### Hello Robot Runners!

We're excited to announce that the main round of the competition has arrived! In this post we’re going to tell you what’s new, what’s changed, and what it means for your team and your submissions. Let’s dive together into the heart of the challenge!

### 1. Main Round:

The main round officially kicks off on August 30! Building on the successful test round, we have introduced a variety of new and exciting problems, giving you more opportunities to showcase your skills in a wider variety of settings.

As before, we evaluate submissions on each of our 5 test maps, for up to 5000 time steps. However, performance will now be evaluated across 10 different instances in one of three distinct categories:


- **High-density** problems. Prepare to push your coordination skills to the limit as you navigate your robots through very congested spaces. Can you maintain order amid all the chaos?


- **Industry-scale** problems. Similar in size to some real-world applications, these problems raise the stakes: by adding more robots to a larger and more challenging path-planning environment. Adapt your strategies to maintain a winning edge!


- **Large-scale** problems. Designed to push the limits of current applications, these problems ask you to plan for thousands of robots in a fiercely contested environment. With a challenge this intense you’ll have to up your game!

### 2. Enhanced Website Features:

We’ve introduced a new leaderboard to keep track of your submissions and all the latest standings. You can now also explore archived submissions, from the test round. These enhancements give further insights into your performance, that of other teams and everyone’s progress in the competition.

### 3. Updated Start-Kit (Version 1.1.2):

We have a new release of the Start-Kit code available from the competition repository. This release features a variety of improvements, enhancements and bug fixes:


- *More Example Instances:*
  - We generated a variety of new example problems, to cover the wider range of challenge problems in the main round. Different from the evaluation instances, these examples will nevertheless help you test your submissions and track your progress locally.

- *Additional Documentation:*
  - The README.md file now contains additional descriptions for program inputs, file formats, and dependencies. These clarify questions we received in the test round.
  - Windows users will now find detailed instructions for using our Start-Kit with Windows Subsystem for Linux (WSL).  Now everyone can get started without any hiccups!

- *Bug fixes:*
  - We fixed a bug affecting the interpretation of ‘T’ type obstacle tiles
  - We’ve fixed a map-boundary issue affecting some users
  - See the [changelog](https://github.com/MAPF-Competition/Start-Kit/blob/v1.1.2/Changelog.md) for further details.

### 4. Updated PlanViz (1.2.0):

We have updated our PlanViz visualiser, with the latest release again available from its home repository. Included in this update are a variety of enhancements:

- Allows user-specified start and end times for visualisation. This improvement allows users to more effectively inspect just the most relevant parts of a generated plan.
- UI performance improvements. 
- Various bug fixes and enhancements
- See the [changelog](https://github.com/MAPF-Competition/PlanViz/blob/v1.2.0/Changelog.md) for further details.

### 5. Important Deadlines:

As previously announced, the deadline for the main round is anytime on November 30th. Pencil this date into your calendar now and add a reminder to avoid disappointment! The date UTC-12, which means any submission on or before 23:59:59 on November 30th will be considered timely and queued for evaluation. 

We're excited to have you with us and we're looking forward to your submissions!
