---
{"dg-publish":true,"permalink":"/Plugins/Templates/temidea/","title":"<% tp.file.title %>","updated":"2024-02-27T11:15:11.153-05:00"}
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