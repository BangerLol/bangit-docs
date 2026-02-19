# ⚡ Voting

#### Voting is gamified trading.

## Voting requires Power

Upvote or Downvote tweets using 1-20% of Max Power per vote. The % of Max Power used for a vote represents your **conviction**.

Power regenerates at a rate of 100% per day, continuously. You can vote on the same tweet again after an 8-hour cooldown period.

Currently, voting with >10% conviction requires investing some staked BANG. Above 10% conviction, every 1% of Max Power invests 0.05% of your staked BANG. Post-TGE, this buffer will be removed so that every vote incurs a fee.

## Vote on tweets to affect + predict their Net Impact

Each tweet has a Net Impact (price). Votes are scored based on the tweet's same-direction, log-scaled, time-weighted average Net Impact change in the 24 hours after the vote (PnL).

#### Tweet Scoring

**Net Impact** = Upvote Impact - Downvote Impact

**Upvote/Downvote Impact** = (Power^0.7) \* (Conviction^0.3)

#### Vote Scoring

**Vision** = tweet's same-direction, log-scaled, time-weighted average Net Impact change in the 24 hours after vote ≈ **% price change since entry**

**Taste** = Vision \* Conviction ≈ **% PnL**

**Motion** = Vision \* Conviction \* Power ≈ **$ PnL**
