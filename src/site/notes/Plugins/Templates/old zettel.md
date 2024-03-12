---
{"dg-publish":true,"permalink":"/Plugins/Templates/old zettel/","title":"<% tp.file.title %>","created":"<% tp.date.now(\"dddd, YYYY-MM-DD, h:mm:ss a\")%>"}
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