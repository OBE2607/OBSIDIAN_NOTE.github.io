---
banner: "https://m.media-amazon.com/images/I/614FNxmBSUL._AC_UF894,1000_QL80_.jpg"
banner_y: 0.15
banner_lock: true
banner_icon: 🏯
tags:
  - note
---
# 01 - 01 - OBSIDIAN_NOTE
#TUTO/OBSIDIAN 
## SOMMAIRE

- [[#PLUGIN]]
- [[#Optionnel/TEST]]
- [[#Raccourci]]
- [[#Call OUT]]
- [[#DATAVIEW]]
	- [[#Note qui parte du lien]]
- [[#table]]
- [[#GIT HUB]]
- [[#BUTTON]]

---

## 01 - 01 - OBSIDIAN_NOTE

> [!todo]+ Vidéo
> Tuto Obsidian
> ![[VIEDO TUTO OBSIDIAN.canvas|VIEDO TUTO OBSIDIAN]]


## PLUGIN

- BANNER
	- Affichage bannière et icon
- Advanced Tables
	- Correction des tableur par la touche **TAB**
- Calendar
	- Prise de note sur un calendrier
-  Cheklist
	- Utilisation avec #todo et d'un todo liste devant
- Dataview
	- Recherche et base de donnée
- Exel to Markdown Table
	- Copier colle document Exel
- Emoji Toolbar
	- Création Emoji
- [[01 - 03 - reminder]]
	- Rappel code : **(@** *fonctionne avec un todo devant*
- Icon folder
	- Création icon sur les repertoires
- Kanban
	- <font color="#b7dde8">Création de Kanban</font>
- Full Calendar
	- <font color="#b7dde8">Affiche un calendrier et prise de rendez-vous avec time lipes</font>
	- Note dans répertoire **calendar**
- Day planner
	- <font color="#b7dde8">Afficgage d'une time lipes par jour dans le repertoir Day Planner </font>
- Mind map
	- <font color="#b7dde8">Création de mind map</font>
	- [[../02 - PLUGIN/02 - 01 - plugin Enhancing mindmap]]
		- Extention Mind map 
	- obsedian marmind
		- Extention Mind map
- Task
	- <font color="#b7dde8">Création de Todo liste</font>
- Natural Language Dates in Obsidian
	- <font color="#b7dde8">Insertion de date</font>
- Tasks Timeline
-  Filename Heading Sync
	- Module supp Dataview 
	- https://forum.obsidian.md/t/plugin-for-keeping-the-filename-and-first-heading-of-a-file-in-sync/12042

---

## Optionnel/TEST

- Edit toolbar
	- Script mise en forme tes
- Obsidian to Notion
	- https://akshayhallur.com/blog/use-notion-with-obsidian
- DBFOLDER
	- Création de base de donnée
- Map views
	- Affichage de carte
- [Minimal Theme Settings](https://minimal.guide/Plugins/Minimal+Theme+Settings)
	- Thème
- Chronologie

---

## Raccourci

-  Déplacement 
	- haut bas fichier
		- ![[Pasted image 20230814110645.png]]
- Task 
	- Création note todo deux foi la même touche
		- ![[Pasted image 20230814112115.png]]
- Minimap
	- Afficher la minimap
		- ![[Pasted image 20230814112306.png]]
- Ctr P
	- <font color="#b7dde8">Affichge menu luncher</font>
- Ctr G
	- <font color="#b7dde8">Affichage de la cate</font>
- CTR E
	- <font color="#b7dde8">Mode EDITION</font>

##  Call OUT

-  [[01 - 02 - Call out]]

---

## SYNTAXE

- [[01 - 05 - Syntaxe]]
- https://help.obsidian.md/Editing+and+formatting/Properties
	- DB _base de donnée
 https://rafaelgb.github.io/obsidian-db-folder/features/Sources/_

---

## DATAVIEW

> [!tip]+
> https://blacksmithgu.github.io/obsidian-dataview/queries/data-commands/


- [[001Syntaxe dataview]]

##### Note qui parte du lien

**FROM**
```dataview
list from outgoing([[000OBSIDIAN_NOTE]])

```

##### Ne contient pas ""!"" (plugin à disparue)
```dataview
list from outgoing([[000OBSIDIAN_NOTE]]) AND !#plugins 

```

---
## table
```dataview
list table

```
##### table et date
##### file
```dataview
table file.ctime
```

##### table et dernière date de modification
```dataview
table file.ctime , file.mtime
```

##### Modification du titre avec _as_
```dataview
table file.ctime as "Date de création" , file.mtime as "Date de modification"
```
##### Trier commande _sort file.mtime asc_ pour ⬆️ et _desc_ ⬇️
```dataview
table file.ctime as "Date de création" , file.mtime as "Date de modification"
sort file.mtime desc
```
##### autre syntaxe

![[Pasted image 20230817092102.png]]
```dataview
table file.ctime as "Date de création" , file.mtime as "Date de modification" , file.name , file.size , file.ctime as "date de création"
sort file.mtime desc
```

##### Sélections des plus gros fichier supérieur à 200 _where file.size_

```dataview
table  file.size where file.size > 200
```

##### Ensemble des notes modifiées les cinq dernier jours _>= date(today) - dur(5day)_
**Tris par date _sort  file.mtime desc_**

```dataview
table file.mtime >= date(today) - dur(5day) sort  file.mtime desc
```






##### FILES TAG

**TAG** 
valeur des tags supérieur à 0 _where length(file.tags) >1_



```dataview
table file.tags as "label" , length(file.tags) as "nbrs de tags"
where length(file.tags) >1 

```


##### TASK avec tags
```dataview
task from "0000TEST" AND #PROJET
```
##### METADONNEE

```dataview
list from "0000TEST"

```

 rajoute entreprise par files _flatten entreprise_
```dataview
table entreprise, pays from "0000TEST" where pays="fr" flatten entreprise

```

Rajout syntaxe _contains_
```dataview
table entreprise, pays from "0000TEST" where contains(pays, "SA") flatten entreprise

```

```dataview
table entreprise, pays from "0000TEST" where contains(type, "3cx") flatten entreprise

```
##### Synthèses

- Liste , donne une liste avec un lien
- Table et ajout de champ
-  Task liste des notes qui contiennent des taches

## Advanced



Prendre en compte les majuscules et les minuscules. _UPPER_

Ne fonctionne pas avec une majuscule
```dataview
table type from "0000TEST" where pays="fr" AND contains(type, "3Cx")
```

Fonctionne avec une majuscule
```dataview
table type from "0000TEST" where pays="fr" AND contains(upper(type),"3CX")
```


Possible d'intégrer un table avec exemple (marque::voiture) ou [marque::voiture]

- INLINE _(modification du fichier actuelle)_
`=this.file.mtime`


```dataview
table eval.avis as "avis" from "0000TEST"
```

Enlever le *FILE* avec _WITHOUT ID_

```dataview
table without id type as matériel, eval.avis as "avis" from "0000TEST"  flatten entreprise
```

## FONTAWESOME

```
[Default](#){.btn .btn-default}
[Primary](#){.btn .btn-primary}
[Info](#){.btn .btn-info}
[Success](#){.btn .btn-success}
[Warning](#){.btn .btn-warning}
[Danger](#){.btn .btn-danger}
[Link](#){.btn .btn-link}
```


[Default](#){.btn .btn-default}


Texte normal suivi d’un <span style="color: #26B260">texte coloré en vert</span> dans un paragraphe.


```
   [fa=firefox /]
    [fa=firefox extras=fa-2x /]
    [[fa=firefox extras=fa-3x /] Avec un lien](https://www.mozilla.org/fr/firefox/new/)
    [fa=firefox extras=fa-4x,fa-spin /]
```

https://fontawesome.com/v4/icons/

<i class="fa fa-bath" aria-hidden="true"></i>


<i class="fa fa-camera-retro fa-lg"></i> fa-lg
<i class="fa fa-camera-retro fa-2x"></i> fa-2x
<i class="fa fa-camera-retro fa-3x"></i> fa-3x
<i class="fa fa-camera-retro fa-4x"></i> fa-4x
<i class="fa fa-camera-retro fa-5x"></i> fa-5x 


<i class="fa fa-calendar fa-2x" aria-hidden="true"></i>


<div class="list-group">
  <a class="list-group-item" href="https://fontawesome.com/v4/examples/"><i class="fa fa-home fa-fw" aria-hidden="true"></i>&nbsp; Home</a>
  <a class="list-group-item" href="#"><i class="fa fa-book fa-fw" aria-hidden="true"></i>&nbsp; Library</a>
  <a class="list-group-item" href="#"><i class="fa fa-pencil fa-fw" aria-hidden="true"></i>&nbsp; Applications</a>
  <a class="list-group-item" href="#"><i class="fa fa-cog fa-fw" aria-hidden="true"></i>&nbsp; Settings</a>
</div>







## Call out
![[01 - 02 - Call out]]

## GIT HUB

![[01 - 07 - GIT HUB]]

## BUTTON

![[01 - 08 - BUTTON]]

