---
icon: gift
---

# Rewards

#### Rewards are distributed daily to curators, creators, and inviters.

Everyday at midnight UTC, new BANG tokens are minted to curators, creators, and inviters based on performance in the last 24 hours. Bangit's logic to allocate rewards is open source and governed by decision markets. Contributors can claim their rewards at anytime. 10% of unclaimed rewards are burned every 7 days they are left unclaimed.&#x20;

## Curators

* 80% of rewards
* Allocated to voters with positive net profit in the period, proportionally
* Vote raw profit = Post's final realtime net impact - Post's realtime net impact after vote
* Vote profit = Vote raw profit \* Vote power

## Creators

* 10% of rewards
* Allocated to author of tweets with positive period net impact in the period, proportionally, scaled by Reward Boost
* Creator Rewards = SUM\[Authored Post Period Net Impact \* Reward Boost] for all authored posts
* Post period net impact = Post's positive period impact - Post's negative period impact
* Period impact = # voters \* total power \* average conviction

## Inviters

* 10% of rewards
* Allocated to inviters of voters that earned curator rewards in the period, proportionally, scaled by invite degrees and Reward Boost
* Inviter Rewards = (Inviter Boosted Connection / Total Boosted Connection) \* (Inviter Reward Pool)
* Inviter Boosted Connection = SUM\[Voter Curator Rewards \* Invite Degree Factor \* Inviter Reward Boost] for all upvoters that earned curator rewards in the period
* Invite Degree Factor= 5 if direct invite, 2 if second-degree invite, 1 if third-degree invite

