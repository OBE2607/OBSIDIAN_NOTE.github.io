---
banner: "https://static.vecteezy.com/ti/vecteur-libre/p1/14995095-banniere-de-gestion-de-projet-icone-web-illustrationle-pour-le-conseil-aux-entreprises-et-le-travail-d-equipe-avec-l-ensemble-d-icones-de-ressources-humaines-de-risque-de-portee-de-cout-de-communication-de-temps-d-approvisionnement-et-d-objectif-vectoriel.jpg"
banner_y: 0.028
banner_lock: false
banner_icon: 🐾
installation: false
entreprise siège: non_entreprise
entreprise annexe: oui/non
adresse: adresse_multisite/oui/non
projet: 3CX/wifi/Meraki
operateur: SFR/Alphalink/UNYC/SEWAN
NbrsTrunk: 0
multisite: oui_non
tech_ref: nom_tech
matériel: oui/non
ID2SON: oui/non
deadline: 20-08-2023
tags:
  - ETAT/Départ
  - ETAT/En_cours
  - ETAT/Blocage
  - ETAT/Terminé
  - INSTALLATION
image: https://media.licdn.com/dms/image/C510BAQEfMrCETP003w/company-logo_200_200/0/1519863175658?
cover: PJ/olivier.jpg
---
> [!tip]+ DEPLOIMENT
![[TRAM DEPLOIMENT CANVAS.canvas|TRAM DEPLOIMENT]]

# NOM_DU_PROJET



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
> - [ ] VM
> - [ ] Commutateur
>- [ ] SBC
> - [ ] FW MERAKI

# Matériel
[[001PROJET/IN_MATERIEL/MATERIEL]]
> [!todo]
> - [ ] Reçu
> - [ ] matériel envoyé
	> 	- [ ] Shaphelec site de Lyon
	> 	- [ ] Client site de ...
# Installation
[[INSTALLATION]]
> [!todo]
> - [ ] Installation prévu le DATE

# Operateur
[[Opérateur]]
-  MSCOM
	- Alphalink
	- UNYC
	- SEWAN
		- NbrsTrunk
> [!todo]
> - [x] _exemple_(@2023-08-25) Portabilité MSCOM ALphalink #todo
> - [ ] Portabilité lancé
> - [ ] Date de portabilité ... /rappel/todo
# Contacts
<!-- Modification code dernière ligne "le nom de la société" -->
```dataview
table without id nom,prénom,Entreprise,Email,TELFixe as FIXE,TELPort as Portable from "001PROJET/ANNUAIRE" where type="ANNUAIRE" AND contains(Projet, "BIENCHEZMOI")
```

# PLAN

```mapview
{"name":"Default","mapZoom":14,"centerLat":44.933453342562984,"centerLng":4.894752502441406,"query":"","chosenMapSource":0}
```

