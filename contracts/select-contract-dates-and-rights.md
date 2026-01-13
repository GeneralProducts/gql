---
title: Select contract dates and rights
layout: home
nav_order: 5
parent: Contracts
description: "Select contract dates and rights"
permalink: select-contract-dates-and-rights
---

# Select contract dates and rights

## Explanation

Contract IDs are retrieved for a single contract along with delivery dates and licensed rights details.

```
query GetContractDatesAndRights($contractId: Int!) {
  contract(contractSearch: {idEq: $contractId}) {
    id
    msDeliveryDate
    revisedMsDeliveryDate
    actualMsDeliveryDate
    msProofsDate
    pubBeforeDate
    licensedRights {
      authorCut
      id
      rightType
    }
  }
}
```

Define your contract ID variable:

```
{
  "contractId": YOUR_CONTRACT_ID_HERE
}
```
