# Review: <% tp.date.now("YYYY-MM") %>
## 每日习惯
```dataviewjs
let pages = dv.pages(`"Reviews/Daily/"`)
const year = dv.
const month = month
const date_pattern = 'YYYY-MM-DD'
const habit_tag = '#habit'
const habits = {
	'背单词': '☑️ {habit} words',
	'吃早饭':'☑️ 吃早饭',
	'运动':'☑️ 运动',
	'睡午觉':'☑️ 睡午觉'
}

let data = {}
for (let page of pages) {
	let date = page.file.name
	data[date] = data[date] || ''
	for (let task of page.file.tasks.filter(task => task.tags.contains(habit_tag) && task.checked)) {
		for (let habit in habits) {
			if (task[habit]) {
				data[date] += habits[habit].replace('{habit}', task[habit]) + '\n'
			}
		}
	} 
}

let calendarData = []
for (let date in data) {
	calendarData.push({date: date, content: data[date]})
}
renderHabitCalendar(this.container, dv, {year, month, data: calendarData, date_pattern}) 
```

### 年终目标 OKRs
![[ <% tp.date.now("YYYY") %>#OKRs]]
## 上月回顾
![[<% tp.date.now("YYYY-MM","P-1M") %>#本月回顾 <% tp.date.now("YYYY-MM","P-1M") %>]]
> [!question] 灵魂拷问
> 你完成了这些计划了吗？如果有，你觉得自己表现如何？如果没有，这个月你需要做些什么才能完成？

## 本月回顾 <% tp.date.now("YYYY-MM") %>
> [!question] 灵魂拷问
> 你这个月会制定哪些目标？
- [ ] 