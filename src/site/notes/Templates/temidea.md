---
{"dg-publish":true,"permalink":"/Templates/temidea/","title":"<% tp.file.title %>","tags":["ZeType/Idea"],"created":"2023-08-22T23:49:27.944-05:00","updated":"2023-10-05T18:20:37.823-05:00"}
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


> [!summary] 🧠
> <% tp.file.cursor() %>
- - - 
> [!question] 🔗
> .
> .


