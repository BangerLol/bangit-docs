---
icon: question
---

# Overview

## The curator economy for Twitter/X

Upvote to earn. Free to play. Powered by Solana.

### Enjoyers: Less slop, more bangers

For people that enjoy good tweets, Bangit serves tweet feeds with less slop and more bangers. Tweets are sorted by a new engagement metric based on skin in the game.

### Curators: Proof of Taste

For people that find good tweets early, Bangit pays you to curate bangers. Upvote tweets to earn BANG tokens when other people upvote those tweets.

### Creators: Win Big

For people that post good tweets, Bangit gives real recognition and upside. Tweet authors earn BANG tokens when their tweets get upvoted.



## Overview

Users have an upvote power resource that regenerates at a rate of 50% of their max power per day. Users can variably allocate this power to tweets, with a minimum of 2% and a maximum of 10% of their max power per upvote. Users can upvote the same tweet again after a 4-hour cooldown period.

Every 24 hours at midnight UTC, new BANG tokens are minted.

* 90% of new BANG tokens are distributed to tweets based on the upvote power they received and unique upvoters in the period, for each tweet:
  * 80% goes to all historical upvoters of the tweet based on their proportional contribution to the tweet's current upvote power ("curator rewards")
  * 20% goes to the tweet author ("creator rewards", boosted with stake)
* 10% of new BANG tokens are distributed to inviters ("invite rewards", boosted with stake)

Staking BANG increases max power and a reward boost for creator and staking rewards. A daily increasing multiplier further increases max power and reward boost.

* Time Multiplier (max 5) = 1 + (0.01 \* Days Staked)
* Max Power = 100 + (Staked BANG \* Power Multiplier)
* Reward Boost (max 3) = 1 + ((sqrt(Max Power) - 100) / 1000)

When staking more BANG, New



&#x20;Boost = ((Old Stake \* Old Boost) + Additional Stake) / New Stake. Unstaking BANG does not affect power multiplier for the remaining staked BANG. Unstaking BANG incurs a 2-5% burn fee, which decreases with higher time multiplier. Unstaking BANG decreases max power and reward boost immediately, while the tokens (post burn fee) gradually become available to claim over 30 days.

## Links

App: [https://bangit.fun](https://bangit.fun/) ("Add to Home Screen" on mobile device)

Twitter: [https://x.com/bangitdotfun](https://x.com/bangitdotfun)
