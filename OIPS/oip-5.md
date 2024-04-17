---
oip: 5
title: Transaction receipt log bloom cache
author: metav
created: 2024-04-10
---

### Parameters
- `FORK_MCINUM`: 7,000,000
- `CHAIN_ID`: 970 (main net)

### Specification

If `block.mci >= FORK_MCINUM` and `CHAIN_ID` is available, then the contract transaction contains one or more indexed, the bloom filter of the transaction receipt will be stored, do not need calculate again.

If `block.mci < FORK_MCINUM`, then the bloom filter for contract transaction is 256-byte empty data. Recalculate the bloom field in eth_getLogs to filter the required topics.
