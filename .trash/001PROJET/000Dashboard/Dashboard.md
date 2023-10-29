
---
cssclass: dashboard
banner_icon: 🌐
archive: oui
Tag : 
- "#DASHBOARD"
- "#INSTALLATION"
banner: "https://newrelic.com/sites/default/files/styles/1200w/public/2023-01/1-Hero-Dashboards-v2.png?itok=V4vHHpDG"
banner_y: 0.272
banner_lock: true
---

%%
[[../../002DBFLODER/000PROJET/000Nom_PROJET/000PROJETS/01CLI|01CLI]]
[[../../002DBFLODER/000PROJET/000Nom_PROJET/000PROJETS/{Tilte}|{Tilte}]]%%
# Dashboard

```start-multi-column
ID: ExampleRegion1
number of columns: 3
```

>[!tip] Projets départ
```dataview
list from "002DBFLODER/000PROJET/000Nom_PROJET/000PROJETS" AND #ETAT/Départ 
```
--- end-column ---

> [!example] Projets en cours
```dataview
list from "002DBFLODER/000PROJET/000Nom_PROJET/000PROJETS" AND #ETAT/En_cours 
```
--- end-column ---
> [!success]    Projets terminé
> 
```dataview
list from "002DBFLODER/000PROJET/000Nom_PROJET/000PROJETS" AND #ETAT/Terminé 
```

--- end-multi-column

# INSTALLATION RECAP


```dataview
table without id projet as "Type installation", entreprise_siège as "entreprise siège", multisite as "Nbrs de site CLI", operateur as "type opérateur", NbrsTrunk as "Nombre de trunk", tech_ref as "technicen référent", tags as "état de l'installation", Installation_fibre as "opérateur" from "002DBFLODER/000PROJET/000Nom_PROJET/000PROJETS" where contains(INSTALLATION, "SAPHELEC") 
```

---

```dataview
table without id projet as "Type installation", entreprise_siège as "entreprise siège", multisite as "Nbrs de site CLI", operateur as "type opérateur", NbrsTrunk as "Nombre de trunk", tech_ref as "technicen référent", tags as "état de l'installation", Installation_fibre as "opérateur" from "002DBFLODER/000PROJET/000Nom_PROJET/000PROJETS" 

```

```dataview
list from "002DBFLODER/000PROJET/000Nom_PROJET/000PROJETS"
```



```dataview
TABLE file.tasks.text, length(file.tasks.text) as Total, file.tasks.completed, filter(file.tasks.completed, (t) => t = true) as C, length(filter(file.tasks.completed, (t) => t = true)) AS Completed, (length(filter(file.tasks.completed, (t) => t = true)) / length(file.tasks.text)) * 100 AS BB, "<progress value='" + (length(filter(file.tasks.completed, (t) => t = true)) / length(file.tasks.text)) * 100 + "' max='100'></progress>" AS Progress
FROM "002DBFLODER/000PROJET/000Nom_PROJET/000PROJETS"
WHERE file.tasks
```



# Work
- 💼 Projects
	- [[Cloud backup]]
	- [[Firewall upgrades]]
	- [[IT Cybersecurity training]]
- 💰 Budget review
	- [[Q1 2022]]
	- [[Q2 2022]]
	- [[Q3 2022]]
	- [[Q4 2022]]
- 👥 Personnel Review
	- [[Sally Smith]]
	- [[Bill Hansen]]
	- [[Brad Jefferson]]
	- [[Olga Olson]]

# Vault Info
- 🗄️ Recent file updates
 `$=dv.list(dv.pages('"002DBFLODER"').sort(f=>f.file.mtime.ts,"desc").limit(2).file.link)`
- 🔖 Tagged:  favorite 
 `$=dv.list(dv.pages('#INSTALLATION').sort(f=>f.file.name,"desc").limit(4).file.link)`
- 〽️ Stats
	-  File Count: `$=dv.pages().length`
	-  Personal recipes: `$=dv.pages('"001DBFLODER/000Dashboard/Dashboard"').length`
