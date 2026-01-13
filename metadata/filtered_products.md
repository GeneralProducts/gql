---
title: Select filtered products and their work
layout: home
nav_order: 2
parent: Metadata
description: "Select filtered products and their work"
permalink: filtered_products
---

# Select filtered products and their work

Select products with particular product forms, and their work

## Explanation

Particular products are retrieved along with their work, filtered by work ID. In this example only hardback and paperback products are returned.

```
query GetProductsByFormCode {
  products(productSearch: { onix21ProductFormCodeIn: [BB, BC] }) {
    id
    onix21ProductFormCode
    onix21ProductForm {
      code
      description
    }
    work {
      id
    }
  }
}
```
