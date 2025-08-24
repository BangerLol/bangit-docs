---
icon: gift
---

# Rewards

Every 24 hours at midnight UTC, new BANG tokens are minted and distributed. Claim your rewards at anytime. 10% of unclaimed rewards are burned every 7 days they are left unclaimed.

90% of new BANG tokens go to tweets (Tweet Rewards). For each tweet's reward, 80% goes to voters (Curator Rewards) and 20% goes to the tweet author (Creator Rewards).

10% of new BANG tokens go to inviters (Inviter Rewards).

## Tweet Rewards

_Tweets that get more upvotes across more people earn more rewards_

Tweet's share of the 90% of new BANG tokens:

`TweetRewards = (TweetNetImpactInPeriod / TotalNetImpactInPeriod) * (Rewards * 0.9)`

Tweet's net impact in the period:

`TweetNetImpactInPeriod = TweetUpImpactInPeriod - TweetDownImpactInPeriod`

`TweetUpImpactInPeriod = UpvotePowerInPeriod * UniqueUpvotersInPeriod`

`TweetDownImpactInPeriod = DownvotePowerInPeriod * UniqueDownvotersInPeriod`

## Curator Rewards

_Upvote popular tweets harder and earlier to earn more rewards_

Upvoter's share of a tweet's rewards:

`UpvoterRewards = (UpvoterTaste / TotalTaste) * UpvoterPool`

Upvoter's taste for a tweet:

`UpvoterTaste = SUM[UpvotePower * (TotalUpvotes - UpvoteIndex + 1)] for all user's upvotes on that tweet`

`DownvoterTaste = SUM[DownvotePower * (TotalDownvotes - DownvoteIndex + 1)] for all the user's downvotes on that tweet`

All historical upvoters of the tweet are included in curator rewards.



{% hint style="info" %}
A Reward Boost based on Max Power is applied to Creator and Inviter Rewards

`Reward Boost (max 3) = 1 + ((sqrt(Max Power) - 100) / 1000)`
{% endhint %}

## Creator Rewards

_Content creators earn rewards when their tweets get upvoted_

Author's share of a tweet's rewards:

`AuthorRewards = (AuthorBoostedClout / TotalBoostedClout) * (TweetRewards * 0.2)`

Author's boosted clout:

`AuthorBoostedClout = AuthoredTweetRewardsInPeriod * AuthorRewardBoost`

## Inviter Rewards

_Invite good curators or people that invite good curators to earn more rewards_

Inviter's share of the 10% of new BANG tokens:

`InviterRewards = (InviterBoostedConnection / TotalBoostedConnection) * (Rewards * 0.1)`

Inviter's boosted connection:

`InviterBoostedConnection = SUM[UpvoterCuratorRewards * InviteDegreeFactor * InviterRewardBoost] for all upvoters that earned curator rewards in the period`

Inviter's relationship degree factor:

`InviteDegreeFactor = 5 if direct invite, 2 if second-degree invite, 1 if third-degree invite`
