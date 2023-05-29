# Welcome to the *Ravens Codex*
This Obsidian vault contains notes for the *Ravens* setting and campaigns run by Lexi, using the [*Monster of the Week* RPG](https://evilhat.com/product/monster-of-the-week/).

## Campaigns
### Current Campaign: *[[Meta/Campaigns/Reassigned]]*
![[Meta/Campaigns/Reassigned#^summary]]

### All Campaigns
```dataview
TABLE start_date as "Started", end_date as "Ended"
FROM "Meta/Campaigns"
SORT start_date asc
```

## Recently Updated
### Sessions
```dataview
TABLE file.mtime as "Time"
FROM "Meta/Sessions"
SORT file.mtime desc
LIMIT 5
```

### Characters
```dataview
TABLE player as "Player", file.mtime as "Time"
FROM "Wiki/Characters"
SORT file.mtime desc
LIMIT 5
```

### Concepts
```dataview
TABLE file.mtime as "Time"
FROM "Wiki/Concepts"
SORT file.mtime desc
LIMIT 5
```

### Creatures
```dataview
TABLE file.mtime as "Time"
FROM "Wiki/Creatures"
SORT file.mtime desc
LIMIT 5
```

### Events
```dataview
TABLE file.mtime as "Time"
FROM "Wiki/Events"
SORT file.mtime desc
LIMIT 5
```

### Groups
```dataview
TABLE file.mtime as "Time"
FROM "Wiki/Groups"
SORT file.mtime desc
LIMIT 5
```

### Locations
```dataview
TABLE file.mtime as "Time"
FROM "Wiki/Locations"
SORT file.mtime desc
LIMIT 5
```

### Objects
```dataview
TABLE file.mtime as "Time"
FROM "Wiki/Objects"
SORT file.mtime desc
LIMIT 5
```

### Miscellaneous
```dataview
TABLE file.mtime as "Time"
FROM "Wiki/Miscellaneous"
SORT file.mtime desc
LIMIT 5
```
