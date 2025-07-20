---
icon: question
---

# How it Works

## Summary

Bangit is the curator economy for Twitter/X. Free-to-Play, Upvote-to-Earn, powered by Solana.

* Enjoyers check curated tweet feeds with less slop and more bangers
* Curators upvote tweets to earn rewards when others upvote those tweets
* Creators (tweet authors) earn rewards when their tweets get upvoted

## Overview

The app integrates with Twitter/X and Privy, allowing users to log in with their Twitter/X account and have an embedded Solana wallet in the background. Users have an upvote power resource that regenerates at a rate of 50% of their max power per day. Users can variably allocate this power to tweets, with a minimum of 2% and a maximum of 10% of their max power per upvote. Users can upvote the same tweet again after a 4-hour cooldown period.

Every 24 hours at midnight UTC, new BANG tokens are minted.

* 90% of new BANG tokens are distributed to tweets based on the upvote power they received and unique upvoters in the period, for each tweet:
  * 80% goes to all historical upvoters of the tweet based on their proportional contribution to the tweet's current upvote power ("curator rewards")
  * 20% goes to the tweet author ("creator rewards", boosted with stake)
* 10% of new BANG tokens are distributed to inviters ("invite rewards", boosted with stake)

Staking BANG increases max power and a reward boost for creator and staking rewards. A daily increasing multiplier further increases max power and reward boost.

* Time Multiplier (max 5) = 1 + (0.01 \* Days Staked)
* Max Power = 100 + (Staked BANG \* Power Multiplier)
* Reward Boost (max 5) = 1 + ((sqrt(Max Power) - 100) / 1000)

When staking more BANG, New Boost = ((Old Stake \* Old Boost) + Additional Stake) / New Stake. Unstaking BANG does not affect power multiplier for the remaining staked BANG. Unstaking BANG incurs a 2-5% burn fee, which decreases with higher time multiplier. Unstaking BANG decreases max power and reward boost immediately, while the tokens (post burn fee) gradually become available to claim over 30 days.

## Links

Mobile app (iOS):

Mobile app (Android):

Twitter: [https://x.com/bangitdotfun](https://x.com/bangitdotfun)
