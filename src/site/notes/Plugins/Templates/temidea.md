---
{"dg-publish":true,"permalink":"/Plugins/Templates/temidea/","title":"<% tp.file.title %>","updated":"2023-11-25T09:21:26.875-05:00"}
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