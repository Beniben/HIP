# Community Knowledge Initiative

- Author(s): Beniben#8033
- Start Date: 2021-11-14
- Category: Community
- Original HIP PR: <!-- leave this empty; maintainer will fill in ID of this pull request -->
- Tracking Issue: <!-- leave this empty; maintainer will create a discussion issue -->

# Summary
[summary]: #summary

As time goes by, we get a new set of users on Discord every day who haven't had much experience with the Helium network. It is time to offer these users another source of information besides Discord and scattered internet guides. Unfortunately, there are also enough people who don't know Discord themselves and have become aware of the project through others. A wiki or documentation would give these people more information about the network without being on Discord themselves. The idea behind this HIP is to give new users a platform where all information about the Helium network is compiled in one place by the community, based on the already experienced users who share their knowledge on a voluntary basis.

# Motivation
[motivation]: #motivation

Many community members find it difficult to answer the same thing several times on a daily basis. There are daily questions about current manufacturers, delivery times or which antenna is best or which connection a hotspot has. A platform that combines such information would make it easier for both new and old users and would allow them to concentrate on other things. The quality of conversations would also be much better if everyone had the same level of information in one place. 

# Stakeholders
[stakeholders]: #stakeholders
 
* Who is affected by this HIP? - All current and future Helium Users.
* How are we soliciting feedback on this HIP from these stakeholders? - Discord channel for discussion

# Detailed Explanation
[detailed-explanation]: #detailed-explanation

The HIP will be implemented by performing the following;

- Disable invite option in Discord server.
- Create a new single page app at https://community.helium.com which presents educational materials to
  new community members in a wizard like format including;
  + What is Helium? - introduces the IoT network and use cases
  + How does Helium work? - introduces blockchain, hotspots, validators, placement basics, rewards etc...
  + Community Rules - presents community rules
  + Scam Awareness - presents tips to avoid being scammed by others on Discord, e.g. suggesting to read
    the official docs for free rather than opting in to 30 min $200 Helium webinars being offered by 
    unscrupulous community members.
- Following presentation of the materials, or during interstitials during the materials, the user will
  be presented 5 random multiple choice questions based on the information provided.
- If the user answers all 5 questions satisfactorily then they will be invited to the Helium Discord server
  by a serverside service account.
- If the user isn't successful they will be invited to review the materials again and will be presented
  with 5 new questions.

There is no limit to the amount of attempts a user may have to enter the community. Materials should not be
as mundane as documentation and could be provided by video content to ensure easy consumption. The aim of this
entry gate is not to reduce the number of new members but to help educate new members at a high level about the
project, increase coverage of the rules, and accelerate new members to be active members of the community.
The process should be supportive and nurturing and not a barrier to entry.

# Drawbacks
[drawbacks]: #drawbacks

- May reduce number of new community members due to additional effort required to join.

# Rationale and Alternatives
[alternatives]: #rationale-and-alternatives

- Why is this design the best in the space of possible designs?
  + 100% Self-service & automated
  + Largely accessible
  

- What other designs have been considered and what is the rationale for not
  choosing them?
  + Restricting invite capability to existing members who have reached some level of cadence
    * Difficult to manage in an automated way 
    * Trusts existing community members to make reasonable invites
    * Makes it impossible to join unless you know an existing community member


- What is the impact of not doing this?
  + Continued rising tensions in the community between tenured members and new members due to lack of sympathy
    for new member's lack of experience. (at least with this system new members should have a basic understanding)
  + Continued poor experience for new members due to attitude of tenured members towards them due to their lack of
    knowledge.
  + Continued poor experience for new members being approached by unscrupulous members to buy expensive and
    exploitative consultation services most of which are sharing information freely available within the Helium docs.

# Deployment Impact
[deployment-impact]: #deployment-impact

- How will current users be impacted? - No impact to current community members, only affects new community members.
  New members will be required to review Helium community educational materials and pass basic test before receiving
  an invite to the Discord.

- How will existing documentation/knowlegebase need to be supported? - The community sign up wizard will be self documenting with an intuitive design.

- Is this backwards compatible? - Not Applicable

# Success Metrics
[success-metrics]: #success-metrics

- What should we measure to prove a performance increase? - Not Applicable

- What should we measure to prove an improvement in stability? - Not Applicable

- What should we measure to prove a reduction in complexity? - Not Applicable

- What should we measure to prove an acceptance of this by it's users? - Community vibe should be observed for less tension between tenured and new members.
