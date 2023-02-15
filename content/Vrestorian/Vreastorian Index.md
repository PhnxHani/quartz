---
dg-home: true
dg-publish: true
---
# Player
```dataview
Table player, class
FROM #character 
```
# Sessions
```dataview
TABLE number, date
FROM #sessionNotes 
WHERE file.folder != "Templates"
SORT number asc
```
# World Map 
![[Vreastorian Empire]]

# Locations
```dataview
TABLE lastVisited
FROM #location 
WHERE file.folder != "Templates"
```

# NPC's
```dataview
TABLE lastLocation AS "last known Location", lastSeen AS "last seen"
FROM #npc 
WHERE file.folder != "Templates"
SORT lastSeen desc
```

