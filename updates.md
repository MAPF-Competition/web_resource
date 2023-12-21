## 🎉Results Announcement for Main Round 2023!🎉 `21 Dec 2023`

**Hello Robot Runners!**

Since the end of the competition 🎬, our organising team has been busy verifying the final standings on the leaderboard. With that work now complete we are now ready to announce the official winners of the main round for 2023! 🎊🎉🏆

We also discuss 🤔 the next steps for the League of Robot Runners and associated community initiatives**📝**, all coming up in 2024. 

**🏅 Award Winners 🏅**

Participants in the 2023 League of Robot Runners were evaluated in 3 distinct performance categories 🔥, each highlighting a distinct challenge that is faced by industry practitioners. There is one 💸**grand prize **for each category and 🥁**distinguished performance awards **for runners-up. 

* **Fast Mover:** **☄️**This category rewards the highest achieved score, subject to a 1-second limit on each planning episode. The main challenge in this case is effective performance under time pressure. 
* **Line Honours: 🎗️**This category rewards the largest number of best-known solutions across the evaluated problem instances. The main challenge in this case is to achieve the highest possible solution quality.
* **Overall Best: 🏆**This category rewards the highest achieved score across all evaluation instances. The main challenge is to maximise the global performance.


<table>
  <tr>
   <td align="left">
   </td>
   <td align="left">
<strong>☄️Fast Mover</strong>
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

Best regards,

The League of Robot Runners Organising Committee


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

**Hello Robot Runners!**

We are more than half-way in the main round -- can you believe it? There are now many submissions from teams all over the world and the leaderboard has 🧨 lit up! 🎆 Make sure to keep an eye on the latest standings so that your team doesn’t get left behind!

In this newsletter we describe a number of recent updates to the competition website, and the start-kit software and we announce new resources for participants -- all to help you get that winning edge! Let’s dive right in!


**1. Website Updates**

We have improved the leaderboard in a variety of different ways, making it easier than ever to track your progress 🤖 and those of other teams **🖥️**.



* Team names are now shown alongside their Algorithm name. We added this feature as algorithmic approaches may change over time.
* We added a new “All Submissions” tab to the leaderboard. This helps you keep an eye on submissions from other teams. Who submitted what and when!
* We added a Trend plot for the Line Honours category. This allows you to see more easily who is making progress in the race!
* Fixes for a variety of visual bugs. 

**2. Software Updates**

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


**3. Training Data!**

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

**Hello Robot Runners!**

We're excited to announce that the main round of the competition has arrived! In this post we’re going to tell you what’s new, what’s changed, and what it means for your team and your submissions. Let’s dive together into the heart of the challenge!

**1. Main Round:**

The main round officially kicks off on August 30! Building on the successful test round, we have introduced a variety of new and exciting problems, giving you more opportunities to showcase your skills in a wider variety of settings.

As before, we evaluate submissions on each of our 5 test maps, for up to 5000 time steps. However, performance will now be evaluated across 10 different instances in one of three distinct categories:


- **High-density** problems. Prepare to push your coordination skills to the limit as you navigate your robots through very congested spaces. Can you maintain order amid all the chaos?


- **Industry-scale** problems. Similar in size to some real-world applications, these problems raise the stakes: by adding more robots to a larger and more challenging path-planning environment. Adapt your strategies to maintain a winning edge!


- **Large-scale** problems. Designed to push the limits of current applications, these problems ask you to plan for thousands of robots in a fiercely contested environment. With a challenge this intense you’ll have to up your game!

**2. Enhanced Website Features:**

We’ve introduced a new leaderboard to keep track of your submissions and all the latest standings. You can now also explore archived submissions, from the test round. These enhancements give further insights into your performance, that of other teams and everyone’s progress in the competition.

**3. Updated Start-Kit (Version 1.1.2):**

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

**4. Updated PlanViz (1.2.0):**

We have updated our PlanViz visualiser, with the latest release again available from its home repository. Included in this update are a variety of enhancements:

- Allows user-specified start and end times for visualisation. This improvement allows users to more effectively inspect just the most relevant parts of a generated plan.
- UI performance improvements. 
- Various bug fixes and enhancements
- See the [changelog](https://github.com/MAPF-Competition/PlanViz/blob/v1.2.0/Changelog.md) for further details.

**5. Important Deadlines:**

As previously announced, the deadline for the main round is anytime on November 30th. Pencil this date into your calendar now and add a reminder to avoid disappointment! The date UTC-12, which means any submission on or before 23:59:59 on November 30th will be considered timely and queued for evaluation. 

We're excited to have you with us and we're looking forward to your submissions!
