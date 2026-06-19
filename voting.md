# ⚡ Voting

#### Voting = gamified trading.

## Voting requires Power

Upvote or Downvote tweets using 1-20% of Max Power per vote. The % of Max Power for a vote represents your **conviction** in its quality.

Power regenerates at a rate of 100% per day, continuously. You can vote on the same tweet again after an 8-hour cooldown period.

Currently, voting with >10% conviction requires committing staked BANG. Above 10% conviction, every 1% of Max Power commits 0.05% of your staked BANG. Post-TGE, this buffer will be removed so that every vote (1-20% conviction) requires committing staked BANG.

## Vote on tweets to affect + predict their Net Impact

Each tweet has a Net Impact (price). Votes are scored on the tweet's Net Impact change in the 24 hours after the vote, measured relative to what's *expected* of a tweet like it — so beating expectations is what earns (PnL).

#### Tweet Scoring

**Net Impact** = Upvote Impact - Downvote Impact

**Upvote/Downvote Impact** = (Total Power^0.7) \* (Total Conviction^0.3)

#### Vote Scoring

Votes are scored on how the tweet performs *relative to expectations* — a benchmark of how this kind of tweet (mainly the author's recent posts) typically performs after a vote. Beating the benchmark earns; underperforming it loses.

**Vision** = the tweet's same-direction, log-scaled, time-weighted Net Impact change in the 24h after the vote, in excess of its expected (benchmark) change ≈ **% out/underperformance vs expectation since entry**

Vision blends two signals: the tweet's Bangit Net Impact change (80%) and its X/Twitter engagement growth (20%), each measured against its own benchmark. When a tweet has too little X data, Vision uses Net Impact alone.

**Taste** = Vision \* Conviction ≈ **% PnL**

**Motion** = Vision \* Conviction \* sqrt(Power) ≈ **$ PnL**
