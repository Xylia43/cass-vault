# Review: <% tp.date.now("YYYY-MM") %>
## Habit Track
```dataviewjs
let pages = dv.pages(`"Reviews/Daily/2026"`)
const year = 2025
const month = 2
const date_pattern = 'YYYY-MM-DD'
const habit_tag = '#habit'
const habits = {
	'vocabulary': '☑️ {habit} words',
	'reading':'☑️ Hot Houser Flower',
	'bbcSession':'☑️ BBc session',
	'poopoo':'☑️ 💩',
	'workout':'☑️ 🏃',
	'wxread':'☑️ WX reading',
	'168':'☑️ Intermittent Fasting'
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
## Direction
Keep these things in mind as you do this month's review:
### [[My Core Principles]]

### Yearly OKRs
![[ <% tp.date.now("YYYY") %>#OKRs]]
## Last month
![[<% tp.date.now("YYYY-MM","P-1M") %>#Month Review <% tp.date.now("YYYY-MM","P-1M") %>]]
> [!question] Questions to ask
> Did you finish the initiatives? If so, how do you think you did? If not, what do you need to change to finish them this month?

### Other reflections
> [!question] Questions to ask
> How do you feel about your accomplishments? What prevented you from working optimally?

## Month Review <% tp.date.now("YYYY-MM") %>
> [!question] Questions to ask
> What initiatives are you setting this month?
- [ ] 