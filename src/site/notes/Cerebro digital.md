```dataview
> > TABLE WITHOUT ID
> > file.link AS Referencias, length(file.inlinks) AS "Menciones" 
> > FROM #Referencia 
> > WHERE file.name != "Cerebro Digital"
> > SORT file.mtime DESC
> > ```