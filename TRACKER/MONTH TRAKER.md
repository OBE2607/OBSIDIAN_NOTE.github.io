# MONTH TRAKER




```tracker
searchType: frontmatter
searchTarget: ETAT
folder: /TRACKER
datasetName : Calendrier
fixedScale : 1
month:
	startWeekOn : 'Mon'
	color : steelblue
	mode : annotation
	annotation : 👍
```

```tracker
searchType: frontmatter
searchTarget: ETAT
folder: /TRACKER
datasetName : Calendrier
summary:
    template: "Longest Streak: {{maxStreak()}} day(s)\nLongest Breaks: {{maxBreaks()}} day(s)\nLast streak: {{currentStreak()}} day(s)"
```

---

```tracker
searchType: fileMeta
searchTarget: numWords
folder: /TRACKER
line :
	lineColor: red
	title : mots
	yAxisLabel: Toto
```
