---
title: Select basic person details
layout: home
nav_order: 2
parent: Address book
permalink: select_basic_contact_details
---

# Select basic person details

## Explanation

Relevant identifying information is retrieved for a single contact, filtered by their name.

```
query GetPersonDetails {
  contacts(contactSearch: {personNameCont: "Cate"}) {
    id
    name
    keyNames
    gender
    isni
    notes {
      noteText
    }
  }
}
```
