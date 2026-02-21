---
description: '*Subject to change*'
---

# 🪙 Tokenomics

#### BANG is a utility token whose value grows with network usage.

## Supply

### Initial Supply

<figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

**Public Sale (60% of supply)**

* Raising $120k in a fixed-price ICO at an FDV of $200K
* 50% of Public Sale's tokens are staked immediately upon purchase
* 50% of Public Sale's tokens are fully unlocked when sale completes
* 25% of raised funds ($30k) paired with 15% of the initial supply for $60k of initial liquidity
* 75% of raised funds ($90k) goes to a treasury governed by decision markets. A $10k allowance per month goes to the team for operations. Any other treasury transactions must be approved by decision markets.
* Full refund if minimum is not reached

**Liquidity (15% of supply)**

* Paired with raised funds in a Meteora DAMM v2 liquidity pool
* Locked unless a portion is being used for decision markets

**Team (10% of supply)**

* Unlocked in 20% tranches at 30-day TWAPs of 5X, 10X, 20X, 30X, and 100X the ICO FDV
* Staked as they unlock with 20% effective earning power

**Private Sale (10%)**

* Unlocked in 20% tranches at 30-day TWAPs of 5X, 10X, 20X, 30X, and 100X the ICO FDV
* Staked as they unlock with 20% effective earning power
* Raised from [Colosseum](https://www.colosseum.com/) and angels

**Early Users (5%)**

* Mostly staked
* Effective airdrop to early users that contributed to the network as we iterated the product

### Emissions

To bootstrap the network, new BANG is minted daily to the Rewards Pool, 100% of which goes to top curators, creators, and inviters. Emissions start at 100K BANG (0.1% of the initial supply) on the first day and decrease by 100 BANG everyday, until emissions reach a constant 10K BANG per day.

{% hint style="info" %}
BANG's public sale, treasury, emissions, liquidity pool--and the decision markets that govern them--are managed by [Combinator](https://www.combinator.trade/) to enforce the parameters outlined here.
{% endhint %}

***

## Demand

Bangit creates value through utility, status, and entertainment. BANG is how that value is priced and competed for. Every core action in Bangit either locks or burns BANG.

{% hint style="info" %}
All value captured by Bangit flows to the official BANG token. Bangit does/will not accrue value to any other instrument (equity, token, or otherwise).
{% endhint %}

### Why BANG?

Currently, the best curators create massive value, but capture none of it. Platforms take ad revenue. Creators farm engagement. But the people who create signal in a noisy world get nothing.

BANG is a utility token that grants rewards, clout, and influence for curating higher-signal content feeds. More voting/burning -> better feeds -> more utility/status/entertainment value -> more voting/burning.

### Staking

[Staking](staking.md) BANG is required to get meaningful value from Bangit. A daily-increasing Time Multiplier compounds this value over time.

**Max Power** = 100 + (Staked BANG \* Time Multiplier)

**Time Multiplier (Max 5)** = 1 + (0.01 × Days Staked)

**Reward Boost (Max 3)** = 1 + ((Max Power - 100) / 1000)

Unstaking BANG has a 1-10% fee, which decreases as Time Multiplier increases. Unstaking BANG decreases Max Power and Reward Boost immediately, while the unstaked tokens unlock gradually over 7 days.

### Fees

Fees are paid in staked BANG. With all BANG fees: 50% is burned, 40% goes to the Rewards Pool, and 10% goes to the Lottery Pool. The Rewards Pool (from fees and emissions) is distributed every 24 hours at midnight UTC to top curators (voters), creators, and inviters. At the same time, the Lottery Pool has a 7% chance of being distributed to top voters.

**Voting**

Currently, [voting](voting.md) with >10% of Max Power requires committing some staked BANG. Above 10% conviction, every 1% of Max Power commits 0.05% of your staked BANG. Post-TGE, this buffer will be removed so that all votes require committing staked BANG.

{% hint style="info" %}
In [Multicoin's framework](https://multicoin.capital/2018/02/13/new-models-utility-tokens/), BANG is a work-style utility token. Contributors stake to earn the right to do work (curate tweets) and earn rewards, while poor performance is penalized.
{% endhint %}

**Claiming without staking**

Users that opt to claim rewards to their wallet instead of auto-staking incur a 20% fee on the claimable tokens.

**Unclaimed Rewards**

10% fee on unclaimed rewards every 7 days left unclaimed.

**Unstaking**

1-10% fee to unstake, which decreases with more time staked.

**Delegation**

10% fee on rewards earned from delegated power.

**AI Discover**

Get curated tweets from a personalized AI agent trained on your second-degree following graph (who your favorite accounts follow).

**API**

Access Bangit programmatically: bangit.xyz/skill.md

**Ads**

Pin a tweet to the 4th spot on the Hot feed.

**Slashing**

Bangit uses analysis tools to detect and slash cartels. If you move as a pack, you will be slashed.
