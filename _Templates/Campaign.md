---
start_date: {{date}}
end_date: Ongoing
tags: campaigns my-new-campaign todo
---
# {{title}}
Lorem ipsum dolor sit amet.
^summary

This campaign started on {{date}}, and is currently ongoing.

## Background
Lorem ipsum dolor sit amet.

## Characters
```dataview
TABLE player as "Player", status as "Status"
FROM #characters AND #my-new-campaign
SORT file.name asc
```

## Sessions
```dataview
TABLE date as "Date"
FROM #sessions AND #my-new-campaign
SORT date asc
```

## Other Notes
- For topics which appeared in this campaign, see the #my-new-campaign tag.
