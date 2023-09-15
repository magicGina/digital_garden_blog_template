---
title: <% tp.file.title %>
dg-publish: false
tags:
  - timeline
  - blog
  - byC
create-date: <% tp.file.creation_date("YYYY-MM-DDTHH:mm:ss.000Z") %>
---
<span 
class='ob-timelines' 
data-date='<% tp.file.creation_date("YYYY-MM-DD-HH") %>' 
data-title='<% tp.file.title %>' 
data-img = 'https://source.unsplash.com/random/<% tp.date.now("YYYYMMDDHHmm") %>'
data-type='range'
data-end='<% tp.file.creation_date("YYYY-MM-DD-HH") %>'> 
<% tp.file.title %>
</span>