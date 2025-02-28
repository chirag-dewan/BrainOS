---
id: <% tp.date.now("YYYYMMDDHHmm") %>
title: Daily Note <% tp.date.now("YYYY-MM-DD") %>
date: <% tp.date.now("YYYY-MM-DD") %>
type: Home
---

# Zettelkasten Home

## Current Focus

- Primary learning focus: Offensive Security, Threat Hunting
- Active project: ML IDS Detection System
- Current certification: OSCP

## Knowledge Maps

- [[MOC - Core Concepts]]
- [[MOC - Red Team]]
- [[MOC - Blue Team]]
- [[MOC - Techniques]]
- [[MOC - Tools]]
- [[MOC - Resources]]

## Recent Notes

```dataview
TABLE file.cday as "Created"
FROM "02-Permanent"
SORT file.cday desc
LIMIT 5
```

## Active Projects

```dataview
TABLE status, date_modified as "Last Modified"
FROM "04-Projects"
WHERE status = "active"
SORT date_modified desc
```

## Processing Queue

```dataview
LIST
FROM "01-Inbox/Quick-Captures"
WHERE status = "unprocessed"
LIMIT 10
```

## Daily Practice

- [[Daily Note {{date:YYYY-MM-DD}}|Today's Note]]
- [[Weekly Review {{date:YYYY-[W]ww}}|Current Week]]

## System

- [[Zettelkasten Workflow]]
- [[Note Templates]]
- [[Tag System]]