---
icon: gift
---

# Rewards

Every 24 hours at midnight UTC, new BANG tokens are minted and distributed. Claim your rewards at anytime. 10% of unclaimed rewards are burned every 7 days they are left unclaimed.

90% of new BANG tokens go to tweets (Tweet Rewards). For each tweet's reward, 80% goes to voters (Curator Rewards) and 20% goes to the tweet author (Creator Rewards).

10% of new BANG tokens go to inviters (Inviter Rewards).



## Tweet Rewards

_Tweets that get more voters with higher conviction earn more rewards_



Tweet's share of the 90% of new BANG tokens:

`TweetRewards = (TweetEffectiveImpact / TotalEffectiveImpact) * (TotalRewards * 0.9)`



Tweet's effective impact:

if TweetNetImpact ≥ 0,

`TweetEffectiveImpact = TweetNetImpact`

else if TweetNetImpact < 0,

`TweetEffectiveImpact = TweetUpImpact * 0.5`



Tweet's net impact:

`TweetNetImpact = TweetUpImpact - TweetDownImpact`

`TweetUpImpact = Normalized(UniqueUpvotersInPeriod) * Normalized(AvgUpvotePowerPct) * Normalized(UpvotePowerInPeriod)`

`TweetDownImpact = Normalized(UniqueDownvotersInPeriod) * Normalized(AvgDownvotePowerPct) * Normalized(DownvotePowerInPeriod)`



## Curator Rewards

_Voters that vote for top tweets harder and earlier earn more rewards_

All historical voters of the tweet are included in curator rewards. Only the "winning" side voters of a tweet's Net Impact is rewarded. If a tweet's Net Impact is negative, then downvoters are rewarded based on 25% of the Positive Impact of the tweet. This encourages only downvoting over-upvoted slop, instead of dogpiling onto obviously bad tweets, which earns no rewards.



Voter's share of a tweet's rewards:

If TweetNetImpact ≥ 0,

`CuratorRewards = (UpvoterTaste / TotalUpvoteTaste) * (TweetRewards * 0.8)`

If TweetNetImpact < 0,

`CuratorRewards = (DownvoterTaste / TotalDownvoteTaste) * (TweetRewards * 0.8)`



Voter's taste:

`UpvoterTaste = SUM[(TotalPostUpvotes - UpvoteIndex) * UpvotePowerPct * UpvotePower] for all user's upvotes on that tweet`

`DownvoterTaste = SUM[(TotalDownvotes - DownvoteIndex) * DownvotePowerPct * DownvotePower] for all user's downvotes on that tweet`



{% hint style="info" %}
A Reward Boost based on Max Power is applied to Creator and Inviter Rewards

`Reward Boost (max 3) = 1 + ((sqrt(Max Power) - 10) / 1000)`
{% endhint %}



## Creator Rewards

_Authors whose tweets get more upvoters with higher conviction earn more rewards_

Creator Rewards for authors of negative Net Impact tweets get re-distributed to authors of positive Net Impact tweets.



Author's share of rewards:

`AuthorRewards = (AuthorClout / TotalClout) * (SUM[0.2 * TweetRewards] for all tweets with TweetNetImpact > 0 in period)`



Author's clout:

`AuthorBoostedClout = AuthorRewardBoost * SUM[TweetRewards] for all authored tweets with TweetNetImpact > 0 in period`



## Inviter Rewards

_Inviters whose invitees upvote top tweets harder and earlier earn more rewards_



Inviter's share of the 10% of new BANG tokens:

`InviterRewards = (InviterConnection / TotalConnection) * (Rewards * 0.1)`



Inviter's connection:

`InviterConnection = SUM[VoterCuratorRewards * InviteDegreeFactor * InviterRewardBoost] for all voters that earned curator rewards in the period`



Inviter's relationship degree factor:

`InviteDegreeFactor = 5 if direct invite, 2 if second-degree invite, 1 if third-degree invite`
