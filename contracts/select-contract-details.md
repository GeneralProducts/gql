---
title: Select contract details
layout: home
nav_order: 5
parent: Contracts
description: "Select contract details"
permalink: select-contract-details
---

# Select contract details

## Explanation

Contract IDs are retrieved for a single contract along with relevant information including works and dates.

```
query GetContractDetails($contractId: Int!) {
  contract(contractSearch: {idEq: $contractId}) {
    id
    contractName
    description
    client {
      name
    }
    work {
      title
    }
    signedDate
    term
    terminatedDate
    terminationReason
    deliveryDates {
      dateDue
      deliverableType
      deliveryRequirement
      id
      percentageOfTotal
      slippedDate
    }
    gratisCopies {
      note
      numberOfCopies
      sendOn
      sentOn
      productId
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
