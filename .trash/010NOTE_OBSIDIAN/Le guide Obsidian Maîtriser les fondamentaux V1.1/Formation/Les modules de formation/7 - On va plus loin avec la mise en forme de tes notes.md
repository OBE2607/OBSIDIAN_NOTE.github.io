*Revenir au [[../../../001TEST/Le commencement|commencement]]*
![[../Les pièces jointes/Le guide Obsidian.jpg]]

# 7 - On va plus loin avec la mise en forme de tes notes
1.  [[#Comment fonctionne la mise en forme dans Obsidian]]
2.  [[#Les principales astuces pour mettre en forme le texte]]
    1.  [[#Créer des titres]]
    2.  [[#Mettre en gras italique surligner souligner barrer]]
    3.  [[#Sauter plusieurs lignes]]
    4.  [[#Créer des citations simples]]
    5.  [[#Créer des citations complexes]]
    6.  [[#Créer des annotations en bas de page]]
    7. [[#Faire des listes à puce ou des listes numérotées]]
    8.  [[#Créer une liste de tâches]]
    9.  [[#Insérer un commentaire en mode éditer qui est masqué en mode aperçu]]
    10.  [[#Créer un tableau]]
    11. [[#Afficher le contenu d'une note dans une autre note]]
    12.  [[#Tracer une ligne horizontale]]
3. [[#Pour résumer]]



## Comment fonctionne la mise en forme dans Obsidian

La mise en forme dans Obsidian fonctionne avec le format qui s'appelle "Markdown".
Il s'agit tout simplement d'un langage informatique permettant grâce à une syntaxe relativement simple de mettre en forme tes notes dans le logiciel.

Si tu n'as jamais touché à un langage informatique de ta vie, sois rassuré. 

Il ne s'agit ni plus ni moins que de connaître une série de quelques caractères à écrire pour mettre en forme ton texte.

 
## Les principales astuces pour mettre en forme le texte

J'ai créé cette note pour que tu puisses facilement naviguer dedans en fonction de tes besoins, et que tu aies à proximité les principales astuces pour embellir tes notes.

Pour chaque astuce, je t'ai indiqué  *Comment l'écrire en mode éditer* afin que tu puisses rapidement voir la syntaxe à écrire, puis tu trouveras *Le rendu en mode aperçu*. 
Je te conseille par conséquent de consulter cette note en mode "Aperçu".

---

### Créer des titres

Il  existe 6 niveaux de titre, à noter que selon le thème choisi, ils changeront peut-être de couleur en fonction du niveau, cela te permet une meilleure visibilité.

*Comment l'écrire en mode éditer*
```md
# Titre de niveau 1
## Titre de niveau 2
### Titre de niveau 3
#### Titre de niveau 4
##### itre de niveau 5
###### Titre de niveau 6
```

*Le rendu en mode aperçu*
# Titre de niveau 1
## Titre de niveau 2
### Titre de niveau 3
#### Titre de niveau 4
##### Titre de niveau 5
###### Titre de niveau 6

---

### Mettre en gras, italique, surligner, souligner, barrer

Les mises en forme qui suivent peuvent là aussi varier selon les thèmes choisis.
Personnellement, je trouve cela beaucoup plus confortable lorsque le gras ou les textes en italique sont d'une autre couleur.
C'est le cas par exemple avec le thème "Dracula + LYT" disponible dans *Paramètres>Apparence>Thèmes>Gérer*

*Comment l'écrire en mode éditer*
 ```md
*Le rendu en mode aperçu*
*Mettre un astérisque pour un texte en italique*
**Mettre deux astérisques pour texte en gras**
***Mettre trois astérisques pour un texte à la fois en gras et en italique***
~~Mettre deux tildes pour un texte barré ~~
==Mettre deux signes égale pour un texte surligné==
<u>Mettre le U de underline pour souligner </u>
```

*Le rendu en mode aperçu*
*Mettre un astérisque pour un texte en italique*
**Mettre deux astérisques pour texte en gras**
***Mettre trois astérisques pour un texte à la fois en gras et en italique***
~~Mettre deux tildes pour un texte barré ~~
==Mettre deux signes égale pour un texte surligné==
<u>Mettre le U de underline pour souligner </u>

---

### Sauter plusieurs lignes

Un simple appui sur la touche `entrée` n'est pas suffisant pour faire plusieurs sauts à la ligne lorsque l'on visualise dans le mode "Aperçu".
Cependant, tu peux sauter plusieurs lignes en insérant une ou plusieurs balises `<br>` en mode "Éditer".
`Chaque balise <br> inscrite représente un saut à la ligne`

---

### Créer des citations simples

Il existe plusieurs moyens de créer des citations.
Voici le moyen le plus simple.

*Comment l'écrire en mode éditer*
 ```md
 > Un jour, un vieux sage a dit "Aide-toi et le ciel t'aidera".
```

*Le rendu en mode aperçu*
 > Un jour, un vieux sage a dit "Aide-toi et le ciel t'aidera".

---

### Créer des citations complexes

Un autre moyen de créer des citations, plus "colorées" cette fois-ci, est d'utiliser la syntaxe suivante.
Il en existe 12 types différents, et chaque type dispose d'un logo et d'une couleur différente.
Le titre se mettre par défaut en fonction de ce que tu mettras entre les crochets, cependant tu peux mettre le titre que tu souhaites.
Et sache également que tu peux mettre un texte sous le titre.
Voici un premier exemple.

*Comment l'écrire en mode éditer*
 ```md
> [!NOTE]
> Voici ma note

> [!NOTE] Voici un exemple avec le titre personnalisé
> Voici ma note

```

*Le rendu en mode aperçu*
> [!NOTE]
> Voici ma note

> [!NOTE] Voici un exemple avec le titre personnalisé
> Voici ma note

Et voici les différentes citations possibles

*Comment l'écrire en mode éditer*
```md

> [!QUOTE]
> [!INFO]
> [!TODO]
> [!ABSTRACT]
> [!IMPORTANT]
> [!DONE]
> [!QUESTION]
> [!ATTENTION]
> [!FAIL]
> [!DANGER]
> [!BUG]
> [!EXAMPLE]
> 
```

*Le rendu en mode aperçu*
>[!QUOTE]

> [!INFO]

> [!TODO]

> [!ABSTRACT]

> [!IMPORTANT]

> [!DONE]

> [!QUESTION]

> [!ATTENTION]

> [!FAIL]

>[!DANGER]

>[!BUG]

>[!EXAMPLE]

---

### Créer des annotations en bas de page

Créer ce type d'annotation, te permet d'ajouter automatiquement en bas de ton document certaines informations, comme ce que l'on peut retrouver sur un livre.
Il te faut donc dans un premier temps mettre le nom de ton annotation à côté du texte souhaité `[^1]`, puis dans un second temps mettre la description de ce que tu souhaites voir apparaître en bas de la page.
La description de l'annotation peut se placer à n'importe quel endroit sur le document, il n'est pas obligatoire qu'elle soit accolée à ton annotation.
Il est aussi possible de mettre un mot au lieu d'un nombre, Obsidian affichera bien le numéro de l'annotation en fonction de l'ordre dans laquelle elle se trouve.

*Comment l'écrire en mode éditer*
 ```md
 
En cliquant ici tu vas basculer en bas de la page [^1]
Et cela fonctionne également en mettant un mot [^annotation]

[^1]: Et si tu cliques ici tu remonteras en haut
[^annotation]: Pareil pour cette annotation

```

*Le rendu en mode aperçu*
En cliquant ici, tu vas basculer en bas de la page [^1]
Et cela fonctionne également en mettant un mot [^annotation]

[^1]: Et si tu cliques ici, tu remonteras en haut
[^annotation]: Pareil pour cette annotation

---

### Faire des listes à puce ou des listes numérotées

Pour créer une liste, il te suffit de: 
- Mettre un tiret `-` suivi d'un `espace`
- Mettre un numéro `1` suivi d'un point `.` puis d'un `espace`
- `Tab` permet d'avancer 

Faire un saut à la ligne te permettra de continuer la liste, et faire un second saut à la ligne te fera rompre cette liste.

*Comment l'écrire en mode éditer*
 ```md
 - Ligne 1
	 - Ligne 2
 - Ligne 3
	 - Ligne 4

1. Premier
	1. Premier
2. Deuxième
	1. Deuxième
```

*Le rendu en mode aperçu*
 - Ligne 1
	 - Ligne 2
 - Ligne 3
	 - Ligne 4

1. Premier
	1. Premier
2. Deuxième
	1. Deuxième

---

### Créer une liste de tâches

Pour créer une liste de tâche, rien de plus simple.
Il te suffit d'écrire un tiret, ouvrir un crochet, faire un espace et refermer le crochet `- [ ]` 
Tu peux également créer une liste en maintenant `Ctrl + Entrée`

*Comment l'écrire en mode éditer*
 ```md
- [x] Première tâche
- [!] Seconde tâche
- [ ] Troisième tâche
```

*Le rendu en mode aperçu*
- [x] Première tâche
- [!] Seconde tâche
- [ ] Troisième tâche

---

### Insérer un commentaire en mode éditer qui est masqué en mode aperçu

Mettre deux fois le signe pourcentage au début et à la fin du texte souhaité pour cacher le commentaire en mode aperçu.

*Comment l'écrire en mode éditer*
 ```md
La ligne du dessous contient un commentaire masqué en mode aperçu
%% Eh oui, je me cache ! %%

```

*Le rendu en mode aperçu*
La ligne du dessous contient un commentaire masqué en mode aperçu
%% Eh oui, je me cache ! %%

---

### Créer un tableau

Pour créer un tableau, il te suffit d'utiliser: 
- La barre oblique `|` avec les touches `Alt Gr + 6` pour créer les colonnes
- Le tiret du 6 `- ` avec les touches `Shift + 6`
À noter que pour créer un tableau, la meilleure solution reste le plugin "advanced tables" qui te permet de gérer beaucoup plus facilement les tableaux que ce que propose Obsidian de base.
Si tu penses être emmené à utiliser les tableaux, je te recommande fortement ce plugin.

*Comment l'écrire en mode éditer*
 ```md
| Première colonne | Seconde colonne |
| ---------------- | --------------- |
| Première ligne   | Seconde Ligne  |
```

*Le rendu en mode aperçu*
| Première colonne | Seconde colonne |
| ---------------- | --------------- |
| Première ligne   | Seconde Ligne  |

---

### Afficher le contenu d'une note dans une autre note

Lorsque tu crées un lien vers une autre note, tu as la possibilité d'afficher le contenu de la note vers laquelle tu pointes, comme une sorte d'aperçu.
C'est ce que l'on appelle "embarquer" le contenu.
Ici par exemple, je vais embarquer le contenu de la note [[4 - Comment créer des liens entre tes notes, utiliser les tags et quelles utilisations concrètes#Créer un lien renvoyant vers l'endroit précis d'un paragraphe]] en affichant un chapitre spécifique.
Pour cela, il suffit de rajouter un point d'exclamation `!` devant le lien d'une note.

*Comment l'écrire en mode éditer*
 ```md
Voici le résultat de ma note embarquée:
![[Comment créer des liens entre tes notes et quelles utilisations concrètes#Créer un lien renvoyant vers l'endroit précis d'un paragraphe]]
```

*Le rendu en mode aperçu*
Voici le résultat de ma note embarquée :
![[4 - Comment créer des liens entre tes notes, utiliser les tags et quelles utilisations concrètes#Créer un lien renvoyant vers l'endroit précis d'un paragraphe]]


---

### Tracer une ligne horizontale

Tracer une ligne horizontale te permet de mieux séparer visuellement ton document, surtout lorsque celui-ci est très long.
Pour le faire, il te suffit de mettre trois tirets consécutifs `---`

*Comment l'écrire en mode éditer*
 ```md
---
```

*Le rendu en mode aperçu*

---

## Pour résumer
- Nous avons vu que le logiciel Obsidian fonctionnait avec le langage "Markdown"
- On a également vu qu'il était relativement simple de le maîtriser en connaissant quelques astuces
- C'est pourquoi je t'ai mis sur chacune des astuces d'une part la syntaxe et d'autre part le rendu en mode aperçu pour te permettre de mieux visualiser
- Parmi les mises en forme les plus utiles :
	- Créer différents niveaux de titres, qui changeront en fonction du thème sélectionné
	- Mettre en gras italique surligner, souligner, barrer, qui là aussi peut varier en fonction du thème
	- Créer citations simples et complexes
	- Faire des listes à puce et numérotées
	- Créer une liste de tâches
	- Créer un tableau
	- Embarquer le contenu d'une note dans une autre

---

[[6 - Les plugins utiles au lancement et comment trouver les plus adaptés à ton utilisation|< Pour revenir au précédent module]] | [[8 - Les principales astuces pour importer des fichiers et liens externes| Pour accéder au prochain module >]]

---
2023 ™. Tous droits réservés [cerveau-numerique.fr](https://cerveau-numerique.fr/)