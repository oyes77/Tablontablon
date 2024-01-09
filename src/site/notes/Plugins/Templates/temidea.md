---
{"dg-publish":true,"permalink":"/Plugins/Templates/temidea/","title":"<% tp.file.title %>","updated":"2023-12-30T18:06:30.564-05:00"}
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