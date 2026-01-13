---
title: Select professional details
layout: home
nav_order: 2
parent: Address book
permalink: select_professional_details
---

# Select professional details

## Explanation

Person IDs are retrieved for a single contact along with their relevant professional information.

```
query GetProfessionalDetails($personId: Int!) {
  person(id: $personId) {
    id
    professionalAffiliations {
      affiliation
    }
    qualificationsAndHonoursAfterNames
    roleFulfillments {
      role
      organization
    }
  }
}
```

Define your person contact ID variable:

```
{
  "personId": YOUR_PERSON_ID_HERE
}
```
