---
banner: https://static.vecteezy.com/ti/vecteur-libre/p1/14995095-banniere-de-gestion-de-projet-icone-web-illustrationle-pour-le-conseil-aux-entreprises-et-le-travail-d-equipe-avec-l-ensemble-d-icones-de-ressources-humaines-de-risque-de-portee-de-cout-de-communication-de-temps-d-approvisionnement-et-d-objectif-vectoriel.jpg
banner_y: 0.028
banner_lock: false
banner_icon: 🐾
installation: true
entreprise_siège: GROUPE REGUILLON
entreprise_annexe: oui
adresse: adresse_multisite/oui/non
projet: 3CX
operateur: ""
NbrsTrunk: 0
multisite: oui
tech_ref: Arnaud
matériel: oui/non
ID2SON: oui/non
deadline: 2023-09-30T00:00:00.000+02:00
tags:
  - "#ETAT/En_cours"
  - "#INSTALLATION"
image: https://media.licdn.com/dms/image/C510BAQEfMrCETP003w/company-logo_200_200/0/1519863175658?
cover: PJ/olivier.jpg
INSTALLATION: SHAPELEC
Date_départ_installation: 2023-08-16T00:00:00.000+02:00
Installation_fibre: N/A
CANEVA: "[[../../001PROJET/002CANVAS/GROUPE REGUILLON CANVAS.canvas]]"
---
> [!tip]+ DEPLOIMENT
![[../../../../001PROJET/002CANVAS/GROUPE REGUILLON CANVAS.canvas|GROUPE REGUILLON CANVAS]]


# essai


# PROGRESSION

```
= "<progress value='" + (length(filter(this.file.tasks.completed, (t) => t = true)) / length(this.file.tasks)) * 100 + "' max='100'></progress>" + "<br>" + round((length(filter(this.file.tasks.completed, (t) => t = true)) / length(this.file.tasks)) * 100) + "% completed"
```

# Contexte
> [!info]
Installation VM AZURE 3cx.

# Configuration
[[001PROJET/IN_CONFIGURATION/CONFIGURATION_GROUPE_REGUILLON]]

> [!todo]
> - [ ] VM
> - [ ] Commutateur
>- [ ] SBC
> - [ ] FW MERAKI

# Matériel
[[001PROJET/IN_MATERIEL/MATERIEL_GROUPE_REGUILLON]]
> [!todo]
> - [ ] Reçu
> - [ ] matériel envoyé
	> 	- [ ] Shaphelec site de Lyon
	> 	- [ ] Client site de ...
# Installation
[[001PROJET/IN_INSTALLATION/INSTALLATION_GROUPE_REGUILLON]]
> [!todo]
> - [ ] Installation prévu le DATE

# Operateur
[[001PROJET/IN_OPERATEUR/OPERATEUR_GROUPE_REGUILLON]]
-  MSCOM
	- Alphalink
	- UNYC
	- SEWAN
		- NbrsTrunk
> [!todo]
> - [ ] Portabilité lancé
> - [ ] Date de portabilité ... /rappel/todo

# Contacts
%%Modification code dernière ligne "_Modifier le nom de l'entreprise_"%%

```dataview
table without id nom,prénom,Entreprise,Email,TELFixe as FIXE,TELPort as Portable from "002DBFLODER/003ANNUAIRE" where type="ANNUAIRE" AND contains(Entreprise, "SAPHELEC")
```

# PLAN

```mapview
{"name":"Default","mapZoom":14,"centerLat":44.933453342562984,"centerLng":4.894752502441406,"query":"","chosenMapSource":0}
```

