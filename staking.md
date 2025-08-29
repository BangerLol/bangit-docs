---
icon: gem
---

# Staking

_Stake BANG to increase rewards, clout, and influence on feeds_

Staking BANG increases Max Power and a Reward Boost for creator and staking rewards. A daily increasing Time Multiplier further increases Max Power and Reward Boost.

`Time Multiplier (max 5) = 1 + (0.01 * Days Staked)`

`Max Power = 100 + (Staked BANG * Time Multiplier)`

`Reward Boost (max 3) = 1 + ((sqrt(Max Power) - 10) / 1000)`

When staking more BANG,

`New Boost = ((Old Stake * Old Boost) + Additional Stake) / New Stake`

Unstaking BANG does not affect power multiplier for the remaining staked BANG. Unstaking BANG incurs a 1-10% burn fee, which decreases with higher time multiplier. Unstaking BANG decreases Max Power and Reward Boost immediately, while the tokens (post burn fee) gradually become available to claim over 30 days.
