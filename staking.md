---
icon: gem
---

# Staking

_Stake BANG to increase rewards, clout, and influence on feeds_

Staking BANG increases Max Power and a Reward Boost for creator and staking rewards. A daily increasing Time Multiplier further increases Max Power and Reward Boost.

`Power Multiplier (max 5) = 1 + (0.01 * Days Staked)`

`Max Power = 100 + (Staked BANG * Multiplier)`

`Reward Boost (max 3) = 1 + ((sqrt(Max Power) - 10) / 1000)`

When staking more BANG,

`New Boost = ((Old Stake * Old Boost) + Additional Stake) / New Stake`

Unstaking BANG does not affect the Power Multiplier for the remaining staked BANG. Unstaking BANG incurs a 1-10% burn fee, which decreases as the Power Multiplier increases. Unstaking BANG decreases Max Power and Reward Boost immediately, while the tokens vest gradually over 14 days.
