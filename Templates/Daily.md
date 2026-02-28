--- 
# <%tp.date.now("dddd, MMMM D, YYYY",0, tp.file.title)%>
< [[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>|Yesterday]]
#### Habits
- [ ] #habit Vocabulary (vocabulary::20) words
- [ ] #habit HotHouse Flower(reading::1) page
- [ ] #habit BBC Session(bbcSession::1) session
- [ ] #habit Poopoo(poopoo::true) 
- [ ] #habit Workout(workout::30) mins
- [ ] #habit WXReading(wxread::1) unit
- [ ] #habit 16+8 Intermittent Fasting(168::true)
#### Direction
This is what you're working towards!
 ![[<% tp.date.now("YYYY") %>-W<% tp.date.now("ww",-7), %>#<% tp.date.now("YYYY") %>-W<% tp.date.now("ww",-7), %> Goals]]

> [!warning] Creating a new weekly note
> If you want to create the weekly note, don't click the link above. Instead, open up the Command Palette (CTRL/CMD P) and select Periodic Notes: Open weekly note as per the instructions in [[Goal-setting and Reviews]].
#### Tasks due today

```dataviewjs
dv.taskList(dv.pages().file.tasks 
  .where(t => !t.completed)
  .where(t => t.text.includes("{{date:YYYY-MM-DD}}")))
```
#### Today's Frogs
Which things from [[Tasks]] do you particularly want to accomplish today? 
![[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>#Tomorrow, Pre arrange]]
- [ ] 
#### Log


#### Review
#### What I learned today ?

#### Tomorrow, Pre arrange
- [ ] 
#### Reflection: [[2025-Year of Remembering]]