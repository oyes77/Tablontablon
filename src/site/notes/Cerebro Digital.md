```dataview
> > TABLE WITHOUT ID
> > file.link AS Pensamientos, length(file.inlinks) AS "Links" 
> > FROM #ZeType/Pensamiento  
> > WHERE file.name != "Cerebro Digital"
> > SORT file.mtime DESC
> > ```