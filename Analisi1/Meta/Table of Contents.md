
```dataview
TABLE  file.etags AS Tag, file.inlinks AS InLinks, file.outlinks AS OutLinks
WHERE file.name != this.file.name and file.name!="Board"
SORT file.name ASC 
```

# File da linkare
```dataview
LIST WHERE file.outlinks=[] and file.inlinks=[] and file.name!=this.file.name and file.name!="Board"
```
