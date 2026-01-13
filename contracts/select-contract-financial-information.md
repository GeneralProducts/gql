---
title: Select contract financial information
layout: home
nav_order: 5
parent: Contracts
description: "Select contract financial information"
permalink: select-contract-financial-information
---

# Select contract financial information

## Explanation

Contract IDs are retrieved for a single contract along with financial information.

```
query GetContractFinancialDetails($contractId: Int!) {
  contract(contractSearch: {idEq: $contractId}) {
    id
    flatFeeValue
    guaranteedRoyaltyValue
    authorDiscount
    remainderRate
    remainderRateOverCost
  }
}
```

Define your contract ID variable:

```
{
  "contractId": YOUR_CONTRACT_ID_HERE
}
```
