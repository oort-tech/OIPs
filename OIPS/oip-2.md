---
oip: 2
title: Witness staking methods and amount
author: metav
created: 2023-10-20
---

The Olympus protocol, or the Oort mainnet consensus, utilizes PoS where blocks are confirmed by witnesses staking a specific amount of Oort tokens. The objective of this proposal is to ascertain the requisite number of tokens an account must stake to qualify as a witness.

### Witness Staking Framework

#### Participation Requirements

To be eligible as a witness, a staking pool should be created to hold a total of **500,000** Oort tokens. Out of this, the pool creator must directly stake **200,000** Oort tokens, with the community contributing the additional **300,000** tokens. Each community member must stake at least **1000** tokens to participate.

#### Operational Cycle

The operational cycle, or 'epoch', is the interval for selecting block validators from the witness pool. Witnesses alternate as block validators during these cycles. Those serving as validators in a current cycle are known as "Active Witnesses". An epoch spans 10000 MCIs (a specific time metric in the Olympus protocol), typically lasting between 60 and 120 minutes.

#### Staking Commitment
The staking pool creator is authorized to set a commission rate for the pool. This rate applies to the staking contributions from the community, providing a commission to the pool creator. Unstaking is permissible at any point unless the staking pool has reached capacity and the witness is activated. Once activated, the witness must wait out a lock-in period of 300 epochs (about two weeks) before initiating an exit.

#### Community Involvement
Community members are free to stake or unstake in any witness pool without restrictions.

#### Profit Distribution
The staking returns are subject to the Oort tokenomics and aim to offer competitive yields in the range between 10% and 15%.

### Mainnet Bootup Scheme: Genesis Witness Staking and Rewards System
For the decentralized mainnet to function properly, it requires the establishment of **50** genesis witnesses. These pivotal nodes can either be initiated by the Oort Foundation or by the community, provided they meet the specified hardware criteria.

Community members participate by staking Huygens testnet tokens, culminating in a collective staking pool composed of contributions from all genesis witnesses. This collective pool's capacity is defined by the combined stakes of the individual genesis witnesses. Once this pool reaches its capacity, the mainnet is activated. The staking period is set for a duration of **6 months**.

Yields from the genesis witnesses' operations are added to the staking pool and allocated to the stakeholders based on their respective share of the pool, with distributions occurring weekly. After the 6-month period, the staked Huygens tokens are set to be burned, and the Oort mainnet tokens are then disbursed to the stakeholders' wallets.
