# 🎁 Rewards

#### Rewards are distributed daily to top voters, authors, and inviters.

Everyday at midnight UTC, new BANG is minted into the **Rewards Pool**, which splits into the **Performance Pool** (90%) and the **Jackpot Pool** (10%).

The Performance Pool is distributed to voters, authors, and inviters based on performance in the last 24 hours. At the same time, the Jackpot Pool has a 7% chance of also being distributed to top voters proportionally.

Users can claim rewards at anytime. "Claim + Stake" is free, while "Claim" has a 20% fee on the claimable tokens. A 10% fee on unclaimed rewards is applied every 24 hours they are left unclaimed.

## Curator Rewards (voters): 80%

* Split among voters with positive Motion in the period, proportionally
* [Voting](voting.md) is **gamified trading**. Each vote is scored on the tweet's performance in the 24 hours after the vote, measured relative to what's *expected* of a tweet like it (mainly from the author's recent posts) — beating expectations earns, underperforming loses.
  * **Vision** = the tweet's same-direction, log-scaled, time-weighted Net Impact change in the 24h after the vote *in excess of its benchmark* (80% weight), blended with the same measure on its X/Twitter engagement growth (20% weight; shifts fully to Net Impact when X data is thin) ≈ **% out/underperformance vs expectation since trade**
  * **Taste** = Vision \* Conviction (% of Max Power used for vote) ≈ **% profit**
  * **Motion** = Vision \* Conviction \* sqrt(Power) ≈ **$ profit**
* Since each vote is scored based on the 24-hour period after the vote, it may be partially rewarded by 2 daily reward distributions

## Creator Rewards (authors): 10%

* Split among authors of tweets with positive Net Impact in the period, proportionally, scaled by Reward Boost

## Inviter Rewards: 10%

* Split among inviters of voters that earned curator rewards in the period, proportionally, scaled by invite degrees and Reward Boost

