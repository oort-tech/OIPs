---
oip: 2
title: Witness staking methods and amount
author: metav
created: 2023-10-20
---

The Olympus protocol utilizes PoS consensus, where blocks are confirmed by witnesses staking a specific amount of Oort tokens. The objective of this proposal is to ascertain the requisite number of tokens an account must stake to qualify as a witness.

#### Stake

To qualify as a witness, an account must have a total stake of 2,000,000 Oort tokens. Of this amount, a minimum of 1,000,000 Oort tokens should be staked by the account directly, while the remainder can be contributed by the community. The minimum amount of token for each stake from a community member is 10000.

#### Epoch

An epoch defines the time frame during which block validators are chosen from the pool of witnesses. Throughout the epochs, witnesses rotate into the role of block validators. Within a given epoch, these validators are termed "Active Witnesses". The duration of an epoch is anticipated to range from 30 to 60 minutes.

#### Lock period
An account has the flexibility to stake or unstake during any epoch without being subject to a lock-in period.

#### Returns
The returns from staking are governed by Oort tokenomics and are designed to be competitive when compared to other leading PoS chains.
