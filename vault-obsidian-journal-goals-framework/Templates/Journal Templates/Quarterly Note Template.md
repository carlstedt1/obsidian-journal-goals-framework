<%*
let noteTitle = tp.file.title;
let [year, quarter] = noteTitle.split("-Q");
let quarterNumber = parseInt(quarter);
let quarterStart = moment([year]).quarter(quarterNumber).startOf('quarter');
let quarterEnd = moment([year]).quarter(quarterNumber).endOf('quarter');

let currentMonth = quarterStart.format("YYYY-MM");
let currentQuarter = quarterStart.format("YYYY-[Q]Q");
let currentYear = quarterStart.format("YYYY");
%>---
tags:
  - Journal/Quarterly
  - Journal
type:
  - Journal
--- 

>   Quarterly Journal for <% currentQuarter %>
>   << [[<% moment(quarterStart).subtract(1, 'quarter').format("YYYY-[Q]Q") %>]] - [[<% moment(quarterStart).add(1, 'quarter').format("YYYY-[Q]Q") %>]] >>
>   Y: [[<% currentYear %>]]
>   Travel through time: << [[<% moment(quarterStart).subtract(1, 'year').format("YYYY-[Q]Q") %>]] / [[<% moment(quarterStart).add(1, 'year').format("YYYY-[Q]Q") %>]] >>
--- 


# Quarterly Planning
## **Goals Dataview**
> [!multi-column]
>
> > [!important]+ Yearly Goals
> > ![[<%tp.date.now("YYYY", 0)%>#Yearly Goals]]
## Quarterly Goals
- [ ] 
# Quarter Review