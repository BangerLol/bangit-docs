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

`TweetRewards = (TweetEffectiveImpact / TotalEffectiveImpact) * (TotalRewards * 0.9)`

Tweet's effective impact:

if TweetNetImpact ≥ 0,

`TweetEffectiveImpact = TweetNetImpact`

else if TweetNetImpact < 0,

`TweetEffectiveImpact = TweetUpImpact * 0.5`

Tweet's net impact:

`TweetNetImpact = TweetUpImpact - TweetDownImpact`

`TweetUpImpact = UpvotePowerInPeriod * sqrt(UniqueUpvotersInPeriod)`

`TweetDownImpact = DownvotePowerInPeriod * sqrt(UniqueDownvotersInPeriod)`

## Curator Rewards

_Upvote popular tweets harder and earlier to earn more rewards_

Voter's share of a tweet's rewards:

If TweetNetImpact ≥ 0,

`CuratorRewards = (UpvoterTaste / TotalUpvoteTaste) * (TweetRewards * 0.8)`

If TweetNetImpact < 0,

`CuratorRewards = (DownvoterTaste / TotalDownvoteTaste) * (TweetRewards * 0.8)`

Voter's taste:

`UpvoterTaste = SUM[UpvotePower * (UpvotePowerPct / 5) * (TotalUpvotes - UpvoteIndex + 1)] for all user's upvotes on that tweet`

`DownvoterTaste = SUM[DownvotePower * (DownvotePowerPct / 5) * (TotalDownvotes - DownvoteIndex + 1)] for all user's downvotes on that tweet`

All historical voters of the tweet are included in curator rewards.



{% hint style="info" %}
A Reward Boost based on Max Power is applied to Creator and Inviter Rewards

`Reward Boost (max 3) = 1 + ((sqrt(Max Power) - 10) / 1000)`
{% endhint %}

## Creator Rewards

_Content creators earn rewards when their tweets get upvoted_

Author's share of rewards:

`AuthorRewards = (AuthorClout / TotalClout) * (SUM[0.2 * TweetRewards] for all tweets with TweetNetImpact > 0 in period)`

Author's clout:

`AuthorBoostedClout = AuthorRewardBoost * SUM[TweetRewards] for all authored tweets with TweetNetImpact > 0 in period`

## Inviter Rewards

_Invite good curators or people that invite good curators to earn more rewards_

Inviter's share of the 10% of new BANG tokens:

`InviterRewards = (InviterConnection / TotalConnection) * (Rewards * 0.1)`

Inviter's connection:

`InviterConnection = SUM[VoterCuratorRewards * InviteDegreeFactor * InviterRewardBoost] for all voters that earned curator rewards in the period`

Inviter's relationship degree factor:

`InviteDegreeFactor = 5 if direct invite, 2 if second-degree invite, 1 if third-degree invite`
