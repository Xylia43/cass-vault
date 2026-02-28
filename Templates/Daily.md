--- 
# <%tp.date.now("dddd, MMMM D, YYYY",0, tp.file.title)%>
< [[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>|Yesterday]]
#### 习惯
- [ ] #habit 背单词 (vocabulary::10) 个
- [ ] #habit 吃早饭
- [ ] #habit 运动
- [ ] #habit 睡午觉
#### 方向
我们要朝着这个方向努力💪
 ![[<% tp.date.now("YYYY") %>-W<% tp.date.now("ww",-7), %>#<% tp.date.now("YYYY") %>-W<% tp.date.now("ww",-7), %> Goals]]

> [!warning] Creating a new weekly note
> If you want to create the weekly note, don't click the link above. Instead, open up the Command Palette (CTRL/CMD P) and select Periodic Notes: Open weekly note as per the instructions in [[Goal-setting and Reviews]].
#### 今日到期任务

```dataviewjs
dv.taskList(dv.pages().file.tasks 
  .where(t => !t.completed)
  .where(t => t.text.includes("{{date:YYYY-MM-DD}}")))
```
#### 今日想要完成任务
今天你想要完成 [[Tasks]] 中的na? 
![[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>#Tomorrow, Pre arrange]]
- [ ] 
#### Log


#### Review
#### What I learned today ?

#### Tomorrow, Pre arrange
- [ ] 
#### Reflection: [[2025-Year of Remembering]]