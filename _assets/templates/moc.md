---
title: "<% tp.file.title %>"
type: moc
tags:
  - moc
area: "<% tp.file.title %>"
date: <% tp.date.now("YYYY-MM-DD") %>
---

# <% tp.file.title %>

> Map of Content for **<% tp.file.title %>**

## Core Concepts

```dataview
TABLE topic, status
FROM "01_Concepts"
WHERE area = this.area
SORT file.name ASC
```

## Key Theorems & Results

```dataview
TABLE topic, source, status
FROM "04_Foundations"
WHERE area = this.area
SORT file.name ASC
```

## Papers

```dataview
TABLE authors, year, status, rating
FROM "02_Papers"
WHERE area = this.area
SORT year DESC
```

## Open Problems

```dataview
TABLE difficulty, status
FROM "03_Projects"
WHERE area = this.area
SORT status ASC
```

## Roadmap / Learning Path

```mermaid
graph TD
    A[Foundations] --> B[Core Theory]
    B --> C[Advanced Topics]
    C --> D[Open Problems]
```

## External References

- 

---
*Last updated: <% tp.date.now("YYYY-MM-DD") %>*
