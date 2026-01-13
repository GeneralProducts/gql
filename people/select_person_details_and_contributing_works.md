---
title: Select person details and contributing works
layout: home
nav_order: 2
parent: Address book
permalink: select_person_details_and_contributing_works
---

# Select person details and contributing works

## Explanation

Person IDs are retrieved for a single contact along with their relevant details and any relevant associated works.

```
query GetPersonProfile($personId: Int!) {
  person(id: $personId) {
    id
    name
    biographicalNote
    contributions {
      workTitle
      role
    }
    notes {
      content
    }
    addresses {
      street
      city
      country
    }
    gender
    genderClarification
  }
}
```

Define your person contact ID variable:

```
{
  "personId": YOUR_PERSON_ID_HERE
}
```
