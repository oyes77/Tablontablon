---
{"dg-publish":true,"permalink":"/Plugins/Templates/old zettel/","title":"<% tp.file.title %>","updated":"2024-03-09T22:53:06.549-05:00"}
---

<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
  } 
  
  tR += ""
%>
# <%* tR += title %>

## Idea Principal 🧠
<% tp.file.cursor() %>
- - - 
## Links 📎