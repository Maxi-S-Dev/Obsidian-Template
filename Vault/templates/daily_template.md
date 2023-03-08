# <% tp.date.now("dddd - DD.MM.YYYY") %>

> [!Quote]+ Quote of the Day
> <% tp.web.daily_quote() %>

```dataview
Table without ID L.text As "Today's Goals"
From #dailies 
FLATTEN file.lists As L
WHERE meta(L.section).subpath="Action Plan" and file.name= "<% fileDate = moment(tp.file.title, 'DD.MM.YYYY').subtract(1, 'D').format('DD.MM.YYYY') %>"
```
---


> [!tip]+ Habit Tracker
> Sleep:: 0
> Reading:: 0
> Exercise:: 0
> Meditation:: 0
> Coding:: 0


> [!abstract]+ What am I grateful for?
> - 1
> - 2
> - 3


---
---

> [!success]+ What did I create today?
> - 1
> - 2
> - 3

>[!Important]+ Highlights of the Day
>- 1
>- 2
>- 3


### Notes
---
---
### Action Plan
- Achievment  