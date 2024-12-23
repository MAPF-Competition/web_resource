This page contains answers to frequently asked questions, which are not addressed elsewhere in our [documentation](http://leagueofrobotrunners.org/resources). If you have additional questions, or require further clarifications, please drop by our [Discord channel](https://discord.gg/CEYT4g4raR). You can also email the organisers at **league-of-robot-runnners [at] googlegroups [dot] com** (although Discord is usually faster).

## Frequent Questions ![r11](external_page_resource/robots/r11_s.png)

**Q: Can I modify the start kit code?**

> No, except for the bits that we explicitly tell you to modify in the start-kit instructions.

**Q: Can one team join the competition with multiple github accounts?**

> No

**Q: Can I be part of more than one team?**

> No

**Q: My team used up all of our training award credits, can we have more?**

> The total number of training awards is limited and for this reason we normally allocate only one award per team. If you believe your situation is exceptional in some way, please email us (although the answer is probably no). 

**Q: Will my implementation been reviewed by organisers?**

>Yes, the organisers will review participants' implementation at the end of the competition.

**Q: How to work with multiple collaborators?** 
>To work as a team, only one team member need to create a team on the website. The team leader can then fill in the team members' details and github usernames in the team page. The team leader can also give the team members access to the team's submission repository using the "Repo Manage" tab.

**Q: My score on the leaderboard has decreased! Why?**

> If another participant has improved a best-known solution then existing submissions will be re-scored relative to this new baseline. More details about our scoring function are available on the [evaluation](https://leagueofrobotrunners.org/evaluation) page.

**Q: A timestep is equal to one second, but my planner always takes less than 1 second to compute actions. Can I benefit from the time saved, so I can be evaluated for more timesteps?**

> Finishing before the time limit per timestep is fine. But you cannot "bank" the time saved. This is because we always evaluate your planner up to a fixed planning horizon, measured in timesteps. 