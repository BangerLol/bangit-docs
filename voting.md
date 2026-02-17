# ⚡ Voting

#### Voting is gamified trading.

## Voting requires power

Upvote or Downvote tweets using 1-20% of Max Power per vote. Power regenerates at a rate of 100% per day, continuously. You can vote on the same tweet again after an 8-hour cooldown period.

The % of Max Power used represents your **conviction** in a vote.

Currently, voting with >10% of Max Power requires investing some staked BANG. Above 10% conviction, every 1% of Max Power invests 0.1% of your staked BANG. Post-TGE, this buffer will be removed so that every vote requires investing some staked BANG.

## Vote on tweets to affect + predict their Net Impact

Each tweet has a Net Impact (price). Votes are scored based on the tweet's same-direction, log-scaled, time-weighted average Net Impact change in the 24 hours after the vote (PnL).

#### Tweet Scoring

**Net Impact** = Upvote Impact - Downvote Impact

**Upvote/Downvote Impact** = (Power^0.7) \* (Conviction^0.3)

#### Vote Scoring

**Vision** = tweet's same-direction, log-scaled, time-weighted average Net Impact change in the 24 hours after vote ≈ **% price change since entry**

**Taste** = Accuracy \* Conviction ≈ **% PnL**

**Motion** = Accuracy \* Conviction \* Power ≈ **$ PnL**

## Stake BANG to increase Max Power

Higher Max Power means:

* More rewards
* More aesthetic clout
* More influence on the feeds

```
Max Power = 100 + (Staked BANG * Time Multiplier)
```

Your Max Power tier is displayed on your profile.

<div align="left"><figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure></div>
