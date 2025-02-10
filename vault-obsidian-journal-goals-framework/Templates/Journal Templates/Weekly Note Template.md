<%*
let noteTitle = tp.file.title;
let [year, weekNumber] = noteTitle.split("-W");
let weekStart = moment().isoWeekYear(year).isoWeek(weekNumber).startOf('isoWeek').format("YYYY-MM-DD");
let weekEnd = moment().isoWeekYear(year).isoWeek(weekNumber).endOf('isoWeek').format("YYYY-MM-DD");

let currentMonth = moment(weekStart).format("YYYY-MM");
let currentQuarter = moment(weekStart).format("YYYY-[Q]Q");
let currentYear = moment(weekStart).format("YYYY");

let monday = weekStart;
let tuesday = moment(weekStart).add(1, 'days').format("YYYY-MM-DD");
let wednesday = moment(weekStart).add(2, 'days').format("YYYY-MM-DD");
let thursday = moment(weekStart).add(3, 'days').format("YYYY-MM-DD");
let friday = moment(weekStart).add(4, 'days').format("YYYY-MM-DD");
let saturday = moment(weekStart).add(5, 'days').format("YYYY-MM-DD");
let sunday = moment(weekStart).add(6, 'days').format("YYYY-MM-DD");
%>---
tags:
  - Journal/Weekly
  - Journal
type:
  - Journal
created: <% tp.date.now("dddd Do MMMM YYYY HH:mm") %>
createdindex: <% tp.date.now("YYYY-MM-DD") %>
---


>   WeeklyJournal for the <% tp.date.now("Wo") %> week of [[<% tp.date.now("YYYY") %>]] 
>   << [[<%tp.date.now("gggg-[W]ww", "P-1W", tp.file.title)%>]] - [[<%tp.date.now("gggg-[W]ww", "P+1W", tp.file.title)%>]] >> 
>   M:[[<%* tR += monday %>]] Tu: [[<%* tR += tuesday %>]] W: [[<%* tR += wednesday %>]] Th: [[<%* tR += thursday %>]] F: [[<%* tR += friday %>]] Sa: [[<%* tR += saturday %>]] Su: [[<%* tR += sunday %>]]
>   M. [[<%tp.date.now("YYYY-MM", 0, tp.file.title)%>]]  Q: [[<%tp.date.now("YYYY-[Q]Q", 0, tp.file.title)%>]]  Y: [[<%tp.date.now("YYYY", 0, tp.file.title)%>]]
>   Travel through time: << [[<%tp.date.now("gggg-[W]ww", "P-1Y", tp.file.title)%>]] / [[<%tp.date.now("gggg-[W]ww", "P+1Y", tp.file.title)%>]] >>
--- 
# Weekly Planning
## **Goals Dataview**
> [!multi-column]
>
> > [!important]+ Monthly
> > ![[<%tp.date.now("YYYY-MM", 0, tp.file.title)%>#Monthly Goals]]
>
> > [!important]+ Quarterly
> > ![[<%tp.date.now("YYYY-[Q]Q", 0, tp.file.title)%>#Quarterly Goals]]

## Weekly Goals
- [ ] 