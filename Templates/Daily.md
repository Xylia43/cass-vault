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

> [!warning] 创建一个新的每周笔记
> ru g如果你想创建每周笔记，不要点击上面的链接。 打开命令面板（CTRL/CMD P），选择“Periodic Notes：打开每周笔记”，按照[[目标设置和复习]]中的说明。

#### 今日到期任务

```dataviewjs
dv.taskList(dv.pages().file.tasks 
  .where(t => !t.completed)
  .where(t => t.text.includes("{{date:YYYY-MM-DD}}")))
```
#### 今日想要完成任务
今天你想要完成 [[Tasks]] 中的哪项任务? 

#### 工作日志


#### 回顾
#### 每日三省吾身
