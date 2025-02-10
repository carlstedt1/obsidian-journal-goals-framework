---
tags:
  - Journal/Daily
  - Journal
type:
  - Journal
created: <% tp.date.now("dddd Do MMMM YYYY HH:mm") %>
createdindex: <% tp.file.title %> 05:00
aliases:
  - <% tp.date.now("dddd Do MMMM YYYY") %>
---

>   Daily Journal for <% tp.file.title %>
>   << [[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title) %>]] - [[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title) %>]] >>
>   W: [[<% tp.date.now("gggg-[W]ww", 0, tp.file.title) %>]]  M: [[<% tp.date.now("YYYY-MM", 0, tp.file.title) %>]]  Q: [[<% tp.date.now("YYYY-[Q]Q", 0, tp.file.title) %>]]  Y: [[<% tp.date.now("YYYY", 0, tp.file.title) %>]]
>   Travel through time: << [[<% tp.date.now("YYYY-MM-DD", "P-1Y", tp.file.title) %>]] / [[<% tp.date.now("YYYY-MM-DD", "P+1Y", tp.file.title) %>]] >>
---
## **Goals Dataview**
> [!multi-column]
>
> > [!important]+ Weekly
> > ![[<%tp.date.now("gggg-[W]ww", 0, tp.file.title)%>#Weekly Goals]]
>
> > [!important]+ Monthly
> > ![[<%tp.date.now("YYYY-MM", 0, tp.file.title)%>#Monthly Goals]]

## During Day
### Plan & Tasks 
- [ ] 
### Execute & Log
* **07:00** 
### Reflect & Learn
* 