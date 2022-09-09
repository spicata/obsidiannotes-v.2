---
banner: "![[weeklynotesbanner.png]]"
tags:
  - personalnotes
---
# Week 36

[[2022-W35|↶ Previous Week]] | [[2022-W37|Following Week ↷]]

> [!METADATA]-
> Created:: [[2022-09-09]] 14:05
> Updated:: 2022-09-09 14:05
> ID:: 20220909140527

**Table of Contents:**
```toc
style: number
```
___
### Emotional Support Graph
```tikz
\usepackage{pgfplots}
\pgfplotsset{compat=1.16}

\begin{document}

\begin{tikzpicture}
\begin{axis}[colormap/viridis]
\addplot3[
	surf,
	samples=18,
	domain=-3:3
]
{exp(-x^2-y^2)*x};
\end{axis}
\end{tikzpicture}

\end{document}
```
---
### Tasks
```todoist
{
"name": "Unfinished this week(doo doo do do do)",
"filter": "7 days & !#School Schedule",
"sorting": ["date"]
}
```
---
## Memos
- **[[2022-09-05|Monday]]**
	![[2022-09-05#^dailynotes-link]]
- **[[2022-09-06|Tuesday]]**
	![[2022-09-06#^dailynotes-link]]
- **[[2022-09-07|Wednesday]]**
	![[2022-09-07#^dailynotes-link]]
- **[[2022-09-08|Thursday]]**
	![[2022-09-08#^dailynotes-link]]
- **[[2022-09-09|Friday]]**
	![[2022-09-09#^dailynotes-link]]
- **[[2022-09-10|Saturday]]**
	![[2022-09-10#^dailynotes-link]]
- **[[2022-09-11|Sunday]]**
	![[2022-09-11#^dailynotes-link]]
---
## Overview
### Week Statistics
```dataviewjs
const daysPath = dv.current().file.folder;

const attributes = {
	'panic': {
		label: 'Panic',
		average: 100,
	},
	'money-spent': {
		label: 'Money Spent',
		backgroundColor: 'rgba(85, 174, 229, 0.2)',
		borderColor: 'rgba(85, 174, 229, 1)',
		average: 100,
	},
	'hours-worked': {
		label : 'Hours Worked',
		backgroundColor: 'rgba(143, 208, 50, 0.2)',
		borderColor: 'rgba(143, 208, 50, 1)',
		average: 100
	},
};

const date = "2022-09-09";

customJS.DvCharts.renderWeeklyChart({
	dv,
	context: this,
	daysPath: '002_PersonalNotes/002a_DailyNotes',
	attributes,
	type: 'average',
	date
})
```
---
```dataview
TABLE WITHOUT ID
	link(file.name) as "Day",
	feeling AS "💭",
	money-spent AS "💸",
	panic AS "🌪️",
	hours-worked AS "✏️"
FROM "002_PersonalNotes/002a_DailyNotes"
WHERE week = [[2022 Week 36]]
SORT file.name ASC
```
### Habits
```dataview
TABLE WITHOUT ID
	file.link AS "Day",
	Early_morning AS "🌅",
	Morning_shower AS "🚿",
	exercise AS "🏋️",
	reading AS "👓",
	revision AS "🔁",
	homework AS "📚"
FROM "002_PersonalNotes/002a_DailyNotes"
WHERE week = [[2022 Week 36]]
SORT file.name ASC
```
### Learnt Words
```dataviewjs
dv.table(
	["Learnt Word", "Meaning"],
	dv.pages('"002_PersonalNotes/002a_DailyNotes"')
	.filter(p => p["Learnt Word"] && p.week.path == "2022 Week 36")
	.sort(p => dv.date(p.file.name), 'asc')
	.flatMap(p =>
		Array.from(
			{
				length: Math.floor(
					p["Learnt Word"].length / 2
				)
			},
			(_, i) => [
				`${'**'}${p["Learnt Word"][i * 2]}${'**'}`,
				p["Learnt Word"][(i * 2) +1]
			]
		)
	)
)
```



