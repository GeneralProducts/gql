---
title: Select basic organisation details
layout: home
nav_order: 2
parent: Address book
permalink: select_organisation_details
---

# Select organisation details

## Explanation

Organisation IDs are retrieved for a single organisation along with relevant identifying information.

```
query GetOrgDetailsByName($organisationName: String!) {
  organisation(organisationSearch: {nameEq: $organisationName}) {
    id
    organisationName
    dunsNumber
    globalLocationNumber
    inhouseCustomerId
    inhouseSupplierId
    organisationCountry
    isni
    ringgoldId
    standardAddressNumber
    vatNumber
  }
}

```

Define your organisation name variable:

```
{
  "organisationName": "Name here"
}
```
