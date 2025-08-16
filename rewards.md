---
icon: gift
---

# Rewards

Every 24 hours at midnight UTC, new BANG tokens are minted and distributed. Claim your rewards at anytime. 10% of unclaimed rewards are burned every 7 days they are left unclaimed.

90% of new BANG tokens go to tweets (Tweet Rewards). For each tweet's reward, 80% goes to upvoters (Curator Rewards) and 20% goes to the tweet author (Creator Rewards).

10% of new BANG tokens go to inviters (Inviter Rewards).

## Tweet Rewards

Tweet's share of the 90% of new BANG tokens:

`TweetRewards = (TweetImpactInPeriod / TotalImpactInPeriod) * (Rewards * 0.9)`

Tweet's impact in the period:

`TweetImpactInPeriod = sqrt(UpvotePowerInPeriod * UniqueUpvotersInPeriod)`

## Curator Rewards

Upvoter's share of a tweet's rewards:

`CuratorRewards = (UpvoterTaste / TotalTaste) * (TweetRewards * 0.8)`

Upvoter's taste for a tweet:

`UpvoterTaste = sum[UpvotePower * (TotalUpvotes - UpvoteOrder + 1)] for all user's upvotes on that tweet`

All historical upvoters of the tweet are included in curator rewards.

## Creator Rewards

Author's share of a tweet's rewards:

`AuthorRewards = (AuthorBoostedClout / TotalBoostedClout) * (TweetRewards * 0.2)`

Author's boosted clout:

`AuthorBoostedClout = AuthoredTweetRewardsInPeriod * RewardBoost`

## Inviter Rewards

Inviter's share of the 10% of new BANG tokens:

`InviterRewards = (InviterBoostedConnection / TotalBoostedConnection) * (Rewards * 0.1)`

Inviter's boosted connection:

`InviterBoostedConnection = sum[UpvoterCuratorRewards * InviteDegreeFactor * RewardBoost] for all upvoters that earned curator rewards in the period`

Inviter's relationship degree factor:

`InviteDegreeFactor = 5 if direct invite, 2 if second-degree invite, 1 if third-degree invite`
