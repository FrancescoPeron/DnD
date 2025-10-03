## Luoghi
```dataview
TABLE Type, Size, Contea
WHERE Type = "Luogo"
SORT file.name  ASC
```
## Personaggi Importanti
```dataview
TABLE Type as "ID", Stato, Location
FROM "PERSONAGGI/IMPORTANTI"
WHERE Type = "NPC"
SORT file.name ASC
```
## Organizzazioni
```dataview
TABLE Type
WHERE Type = "Organization"
SORT file.name ASC
```

## SESSIONI 
```dataview
LIST
FROM "SESSIONI"
SORT file.name ASC
```

## Party
```dataview
TABLE Race, Class
FROM "Party"
SORT file.name ASC
```

## Utile
```dataview
TABLE
FROM "Utile"
SORT file.name ASC
```
