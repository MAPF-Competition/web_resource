# **LoRR 2026 Main Round Review:** **Summary**

During the post-competition code review for the LoRR 2026 Main Round, the Organising Committee identified two major issues affecting Team `SmartPath` (1st place, Scheduling Track; 2nd place, Combined Track; 2nd place, Execution Track) and Team `wonder` (4th place, Execution Track; 6th place, Scheduling Track; 7th place, Combined Track) . 

The review raised concerns regarding (1) the provenance and transfer of competition code, and (2) the independence of the two teams, as pertains to their combined use of evaluation resources to obtain unfair advantage in the competition. 

Following a detailed investigation, the committee determined these behaviours comprise a clear breach of competition rules. As a consequence, the two teams were disqualified from their final standings in the 2026 main round. 

1\. Findings 

**Source-code correspondence:**

The review compared the **Execution Track** submissions of Team `SmartPath` and Team `wonder`. Results showed many commits with approximately *99.5% source retention*. Closely corresponding versions were also found in `SmartPath`'s **Combined Track**.

Repository history showed a repeated pattern of code transfer, from the Team `wonder` repository to Team `SmartPath`, within a relatively short period.  The affected executors formed part of Team `SmartPath`'s evaluated implementation and therefore directly contributed to its competition performance in both tracks.

The earliest identified commit is from July 12 2026\. 

**Team independence and account sharing:**

The review also identified the Github account used for Team `wonder`'s competition development that belonged to a member of Team `SmartPath`. The committee was able to confirm, in correspondence with Team `wonder`, that the account was being shared.

The competition enforces a daily limit of 5 successful submissions per team to ensure fair resource allocation. Analysis of the submission logs reveals that these two accounts combined significantly exceeded the single-team submission limits.

2\. Rule breaches 

The identified behaviour is in clear violation of the following rules of the competition: 

1. **One team, one account:** The League of Robot Runners competition rules, supported by the [FAQ](https://www.leagueofrobotrunners.org/faq), explicitly state that each participant can only belong to a single team and that a single team may not participate using multiple accounts.  
2. **Submission limits violation:** Coordination between teams constitutes a clear attempt to hijack evaluation system functionalities (competition [rule 8](https://www.leagueofrobotrunners.org/rules)) and thus gain an unfair competitive advantage.

3\. Review procedure

After the review the committee prepared a detailed integrity report setting out the evidence and sent it to **both Team `SmartPath` and Team `wonder`**. Both teams were given an opportunity to respond to the findings and provide explanations or supporting information before any final decision was made.

The Organising Committee considered these responses together with its detailed report and  evaluation evidence. Other contributing factors included in the discussion were how to best preserve the integrity of the competition and maintain community trust in its processes, as well as how to act in the best interest of scientific advancement.    

4\. Decision

After deliberation, the committee reached the following action plan: 

* **Disqualification:** Disqualify Team `SmartPath` and Team `wonder` from all final standings in 2026 Main Round, due to coordinated manipulation of the evaluation system.  
* **AAMAS Prize Retention:** Maintain current standings for the AAMAS Prize, as there is no evidence of collusion prior to July 12, 2026\.   
* **Public Archiving:** The submitted codes and solutions will be archived for the community, as they nevertheless make significant technical contributions which advances the field.

These penalties are limited to the 2026 Main Round. However, repeated violations from these teams, and their members, may result in exclusion from future League events. 

5\. Conclusion

Post-competition code review is an important part of maintaining confidence that LoRR results are obtained under the same rules and resource constraints for all participants. This case highlights areas where the League can improve its procedures, including more emphatic participant-account requirements, stronger repository and identity verification, and systematic source-similarity checks that occur sooner. The Organising Committee will incorporate these lessons into future editions and thanks all participants for their cooperation in maintaining a fair and scientifically valuable competition.