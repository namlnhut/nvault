---
title: Home
type: dashboard
tags:
  - home
  - dashboard
---

# Research Dashboard

> Mathematics — Optimization · ODEs · PDEs

## Areas

| Area | MOC |
|------|-----|
| Optimization | [[Optimization MOC]] |
| Ordinary Differential Equations | [[ODE MOC]] |
| Partial Differential Equations | [[PDE MOC]] |

---

## This Week

```dataview
LIST
FROM "05_Weekly"
SORT file.name DESC
LIMIT 1
```

## Recently Added

```dataview
TABLE type, area, status
FROM "" AND !"_assets" AND !"00_Home"
WHERE type != "moc" AND type != "dashboard"
SORT file.ctime DESC
LIMIT 10
```

## Open Problems

```dataview
TABLE area, difficulty, status
FROM "03_Projects"
WHERE status = "open"
SORT file.mtime DESC
```

## Papers — In Progress

```dataview
TABLE area, status, rating
FROM "02_Papers"
WHERE status != "done"
SORT file.mtime DESC
```

## Papers — Done

```dataview
TABLE area, year, rating
FROM "02_Papers"
WHERE status = "done"
SORT rating DESC
LIMIT 10
```

## Concepts by Area

```dataview
TABLE area, topic, status
FROM "01_Concepts"
SORT area ASC, file.name ASC
```

## Tasks

```tasks
not done
```

---
*Vault initialized: 2026-04-13*
