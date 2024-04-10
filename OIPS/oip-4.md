---
oip: 4
title: NotEnoughCash transaction receipt gasUsed error
author: metav
created: 2024-04-10
---

### Parameters
- `FORK_MCINUM`: 7,000,000
- `CHAIN_ID`: 970 (main net)

### Specification

If `block.mci >= FORK_MCINUM` and `CHAIN_ID` is available, then when the EVM initialize throw the exception of `NotEnoughCash`, the gasUsed in the receipt of the transaction should be 0, not the gas of the transaction.

If `block.mci < FORK_MCINUM`, then the gasUsed in the receipt is equal transaction gas, but the gasUsed fee is not deducted from the account.
