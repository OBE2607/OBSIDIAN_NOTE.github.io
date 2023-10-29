---
banner: "https://static.vecteezy.com/ti/vecteur-libre/p1/14995095-banniere-de-gestion-de-projet-icone-web-illustrationle-pour-le-conseil-aux-entreprises-et-le-travail-d-equipe-avec-l-ensemble-d-icones-de-ressources-humaines-de-risque-de-portee-de-cout-de-communication-de-temps-d-approvisionnement-et-d-objectif-vectoriel.jpg"
banner_y: 0.228
banner_lock: false
banner_icon: 🐾
installation: true
entreprise_siège: non_entreprise
entreprise_annexe: non
adresse: adresse_multisite/oui/non
projet: Wifi
operateur: SFR
NbrsTrunk: 0
multisite: oui
tech_ref: nom_tech
matériel:
  - "[[002DBFLODER/002MATERIEL_CLI/000MATERIEL_CLI/01CLI.md|01CLI]]"
ID2SON: oui/non
deadline: 20-08-2023
tags:
  - ETAT/Départ
  - ETAT/Blocage
  - ETAT/Terminé
  - INSTALLATION
image: https://media.licdn.com/dms/image/C510BAQEfMrCETP003w/company-logo_200_200/0/1519863175658?
cover: PJ/olivier.jpg
CANEVA: "[[TRAM DEPLOIMENT CANVAS.canvas]]"
Installation_fibre: N/A
Date_départ_installation: 2023-08-26T00:00:00.000+02:00
SIRET: "957501034"
INSTALLATION: true
---
> [!tip]+ DEPLOIMENT
![[TRAM DEPLOIMENT CANVAS.canvas|TRAM DEPLOIMENT]]

# 01CLI



# PROGRESSION

```
= "<progress value='" + (length(filter(this.file.tasks.completed, (t) => t = true)) / length(this.file.tasks)) * 100 + "' max='100'></progress>" + "<br>" + round((length(filter(this.file.tasks.completed, (t) => t = true)) / length(this.file.tasks)) * 100) + "% completed"
```

# Contexte
> [!info]
> exemple : Installation VM AZURE 3cx.

# Configuration
- [ ]    [scheduled:: 2023-08-25T15:15]
[[CONFIGURATION]]

> [!todo]
> - [x] VM ✅ 2023-08-27
> - [ ] Commutateur
>- [ ] SBC
> - [ ] FW MERAKI

# Matériel
[[001PROJET/IN_MATERIEL/MATERIEL]]
> [!todo]
> - [x] Reçu ✅ 2023-08-27
> - [x] matériel envoyé ✅ 2023-08-27
	> 	- [x] Shaphelec site de Lyon ✅ 2023-08-27
	> 	- [x] Client site de ... ✅ 2023-08-27
# Installation
[[INSTALLATION]]
> [!todo]
> - [x] Installation prévu le DATE ✅ 2023-08-27

# Operateur
[[Opérateur]]
-  MSCOM
	- Alphalink
	- UNYC
	- SEWAN
		- NbrsTrunk
> [!todo]
> - [x] _exemple_(@2023-08-25) Portabilité MSCOM ALphalink #todo
> - [x] Portabilité lancé ✅ 2023-08-27
> - [x] Date de portabilité ... /rappel/todo ✅ 2023-08-27
# Contacts
<!-- Modification code dernière ligne "le nom de la société" -->
```dataview
table without id nom,prénom,Entreprise,Email,TELFixe as FIXE,TELPort as Portable from "001PROJET/ANNUAIRE" where type="ANNUAIRE" AND contains(Projet, "BIENCHEZMOI")
```

# PLAN

```mapview
{"name":"Default","mapZoom":14,"centerLat":44.933453342562984,"centerLng":4.894752502441406,"query":"","chosenMapSource":0}
```

