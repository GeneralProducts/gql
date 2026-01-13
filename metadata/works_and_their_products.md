---
title: Select works and their products
layout: home
nav_order: 2
parent: Metadata
permalink: works_and_their_products
---


# Description

Select works and their products

## Explanation

Works are retrieved along with their products. This is structured so that the products are naturally grouped under their works, so less data needs to be processed.

```
{
  works {
    id
    title
    products {
      id
      publicationDate
      isbn {
        isbn13
      }
    }
  }
}
```
