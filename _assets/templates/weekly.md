---
title: "Week <% tp.date.now("YYYY-[W]WW") %>"
type: weekly
tags:
  - weekly
  - review
date: <% tp.date.now("YYYY-MM-DD") %>
week: <% tp.date.now("YYYY-[W]WW") %>
---

# Week <% tp.date.now("YYYY-[W]WW") %>
*<% tp.date.now("MMM DD") %> – <% tp.date.weekday("MMM DD, YYYY", 6) %>*

## Focus This Week

> What is the one thing I want to make progress on this week?

## Goals

- [ ] 
- [ ] 
- [ ] 

## Reading

| Paper / Book | Chapter / Section | Status |
|--------------|-------------------|--------|
|              |                   | [ ]    |

## Math Work

### Problems Worked On

- 

### Key Insights / Breakthroughs

> [!success]
> 

### Stuck On

> [!warning]
> 

## Notes Created This Week

```dataview
LIST
FROM ""
WHERE type != "weekly" AND date >= date(<% tp.date.now("YYYY-MM-DD") %>) - dur(7 days)
SORT date DESC
```

## Tasks

```tasks
not done
due before <% tp.date.weekday("YYYY-MM-DD", 6) %>
```

## Reflection

### What went well?

### What was harder than expected?

### What to carry forward?

## Plan for Next Week

- [ ] 
- [ ] 

---
*Previous week: [[<% tp.date.now("YYYY-[W]WW", -7, "days") %>]]*
