---
oip: 3
title: Mainnet Distribution Event - Genesis Witnesses
author: metav
created: 2023-11-20
---

### Mainnet Distribution Event - Genesis Witnesses

In [OIP2](https://github.com/oort-tech/OIPs/blob/master/OIPS/oip-2.md), the Oort witness node and staking pool creation rule was proposed. 

For Olympus Protocol to function properly in a distributed and decentralized manner, our Protocol requires the establishment of a minimum **50** Witnesses, which at launch will be called Genesis Witnesses. 

The Oort foundation will create and stake for 14 Genesis Witnesses and the rest **36** will be built by the community. More witnesses shall be created along with the development of Oort community and ecosystem.

Considering limited Oort mainnet token liquidity after the initial launch, we propose a mechanism for Oort’s community to stake Huygens tokens. Huygens (CCN) staking pools will be created from 36 Genesis Witnesses. 

Considering each Genesis Witness has the staking capacity of 500k CCN (from [OIP2](https://github.com/oort-tech/OIPs/blob/master/OIPS/oip-2.md)). 

The total pool size would be 36*500k = 18 million CCN tokens.

Oort’s mainnet will start to run immediately once all the 50 genesis witnesses are activated. All Witness Pools and stakers begin to earn rewards at launch of Olympus Protocol. 

Staking will be locked at the launch of mainnet with a lockup period of **6 months**. Post 6-month lock-up period, staked Huygens tokens will be burned, and converted to Oort’s mainnet native tokens which will be distributed to all stakeholders' wallets. 

The reward for the Genesis Witness Pool will be set in the range between 15% and 20%.

Consider the “Genesis Witness” staking program as **one of the ways** to convert the Huygens CCN token to Olympus Protocol’s native token.

Yields from the Genesis Witness operations, **Oort's mainnet tokens**, will be allocated to stakeholders based on their respective share of the pool they belong to. The distributions will occur on a **monthly** basis.

**Assertion: The network distribution event serves as Oort's method for encouraging active community participation, hastening decentralization, and promoting early node adoption. It is distinct from both the TGE date and token listing date.**

---
#### How to stake?
If you're interested in becoming a witness, whether as an individual or entity from the community, please contact the project directly to discuss your desired staking amount and commission rate.

The Oort foundation has plans to create a portal where CCN holders can stake in the pool. This portal will provide comprehensive information about the Genesis Witness nodes, such as pool size, staking amounts, APYs, and reward history.

#### Reward calculation
All witnesses and stakers will begin earning rewards after the mainnet distribution event, specifically when the staking pool for the total of 50 Genesis Witnesses is filled.

As outlined in [OIP2](https://github.com/oort-tech/OIPs/blob/master/OIPS/oip-2.md), a witness is required to contribute $200k$ CCN tokens and set up a validator node (please refer to [OIP2](https://github.com/oort-tech/OIPs/blob/master/OIPS/oip-2.md) for the hardware requirements of setting up a validator node). A staker will stake in a pool with a total of 10.8 million CCN tokens. The pool size is the aggregation of 36 witness pools, each with a capacity of $300k$ CCN tokens.

Let $r$ represent the APY of the witness pool, and $m$ denote the commission rate chosen by the witnesses.

A witness's reward earned during the 6-month period can be calculated as follows: $$R_w = (200,000 + 300,000 \times m) \times \frac{r}{2}.$$ On the other hand, let $S$ be the amount of CCN tokens initially placed by a staker into the pool. The staker's monthly stake during the 6-month period will be $(S, \frac{5}{6}S, \frac{4}{6}S, \frac{3}{6}S, \frac{2}{6}S, \frac{1}{6}S)$ due to the linear release nature of the staking. Therefore, the total reward for the staker in the $i$-th month is calculated as follows: $$R_s(i) = \frac{6-i+1}{6} \times S \times (1 - m) \times \frac{r}{2}, \text{where}~~i = 1,2,3,4,5,6.$$ 

#### Example
Suppose the network distribution event occurs on January 1, 2024.

Let us take a look at a more specific example. Assume a staker has put $600$ CCN into the pool, and the APY of the pool is set to be 20%. The witness wants to take 10% commission from the pool earning. 

The total reward earned by a witness up to July 1, 2024, will be $23,000 in OORT. Witnesses have the flexibility to withdraw their rewards from the staking contract whenever they become available.

The reward for the staker will be transferred to the staker's wallet according the following table.

| Date | Reward (OORT) | Linear Release (OORT) |
|---|---|---|
| Feb 1, 2024   | 9 | 100 |
| Mar 1, 2024 | 7.5 | 100 | 
| Apr 1, 2024 | 6 | 100 | 
| May 1, 2024 | 4.5 | 100 | 
| Jun 1, 2024 | 3 | 100 | 
| Jul 1, 2024 | 1.5 | 100 | 

