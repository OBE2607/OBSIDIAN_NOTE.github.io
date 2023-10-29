*Revenir au [[010NOTE OBSIDIAN/001TEST/Le commencement|commencement]]*
![[../Les pièces jointes/Le guide Obsidian.jpg]]

# 4 - Comment créer des liens entre tes notes, utiliser les tags et quelles utilisations concrètes

1.  [[#Qu'est-ce qu'un lien]]
2.  [[#Cas pratique n°1 Les liens utilisés en cuisine]]
3.  [[#Cas pratique n°2 Les liens utilisés au travail]]
4.  [[#Comment créer des liens entre tes notes]]
    1.  [[#Créer un lien simple renvoyant vers la globalité d'une note]]
    2.  [[#Créer un lien renvoyant vers un niveau de titre précis à l'intérieur d'une note]]
    3.  [[#Créer un lien renvoyant vers l'endroit précis d'un paragraphe]]
    4.  [[#Changer le nom du lien qui s'affiche créer un alias]]
    5.  [[#Renvoyer vers un paragraphe à l'intérieur de la note que tu consultes]]
    6.  [[#Les tags un autre moyen de lier tes notes]]
5. [[#Pour résumer]]

## Qu'est-ce qu'un lien
**Un lien, c'est tout simplement un moyen de lier une ou plusieurs notes entre elles.**

Pour illustrer ça, en ce qui me concerne, avant de connaître Obsidian j'ai testé pas mal de solutions différentes pour prendre des notes au travail.

Fichiers textes, Google Agenda, Trello, Asana, Les brouillons dans la boite mail, les post IT, les feuilles volantes, les Mindmap, Le Sketchnote, Les techniques de mémorisation avancée, Les brouillons sur le tépéhone, Ma femme (non je plaisante) ...

Il y en avait partout et rien n'était connecté.

En notant les informations dans un même logiciel et en créant des connexions entre mes idées, je me suis vite rendu compte de la puissance de faire des liens.

Ce qui est intéressant ici, c'est qu'avec les liens, peu importe si tes notes se trouvent dans des dossiers ou non.
En notant tout dans ton coffre, les connexions pourront se faire et les liens perdurer.

**Plus besoin de te torturer l'esprit pour savoir où ranger ta note et en ayant peur de ne pas la retrouver.**

On ne se rend pas compte quand on n'a jamais été confronté à ce problème, mais ça emmène véritablement une nouvelle dimension quant à la prise de notes et à la gestion des connaissances.

Avant de te montrer comment faire, voyons quelques exemples basiques.

---

## Cas pratique n°1 : Les liens utilisés en cuisine !

Admettons que tu sois passionné(e) de cuisine, et que tu décides d'utiliser Obsidian pour noter tes recettes de cuisine favorites.

Tu peux ranger ton système en créant des dossiers, avec d'un côté les recettes, et de l'autre les ingrédients.

Mais en plus de cela, si tu veux voir les connexions possibles, tu peux lier des notes entre elles pour créer de meilleures interactions.

À titre d'exemple, en me mettant sur la recette de poulet au Curry, je peux voir avec la vue graphique tous les ingrédients nécessaires à l'élaboration de ce plat.
![[../Les pièces jointes/Exemple numero 1 en cuisine.png]]

Ou à l'inverse, je peux me placer sur un ingrédient pour voir dans quels plats je peux utiliser cet ingrédient.
![[../Les pièces jointes/Capratique 1 cuisine.png]]

---

## Cas pratique n°2: Les liens utilisés au travail !
Admettons que tu sois responsable d'une équipe de 20 personnes et que chaque mois, tu aies besoin d'assurer le suivi de tes équipes.

Dans ton travail, tu es amené à régulièrement prendre des notes, et notamment en faisant un compte rendu des points hebdo que tu inities.

Mais il y a tellement d'informations que tu ne sais plus où donner de la tête.

Lors d'une de ces réunions, une personne de ton équipe remonte avoir besoin d'aide, car elle a trop de travail. 
![[../Les pièces jointes/Pierre demande de l'aide.png]]

Puis la semaine suivante, cette personne remercie une de ses collègues qui l'a aidée à surmonter ce cap.
![[../Les pièces jointes/Merci Alexandra.png]]


Eh bien en prenant la simple habitude de lier ces quelques notes, dans 1 mois / 6 mois / 1 an quand le temps sera venu de faire le point avec tes équipes, tu seras capable en quelques secondes de te remémorer ces évènements

Notamment grâce à la visibilité des liens sur le Volet de droite ainsi qu'à la vue graphique autour du fichier courant.
![[../Les pièces jointes/Vue graphique sur le cot.png]]

---

## Comment créer des liens entre tes notes ?

### Créer un lien simple renvoyant vers la globalité d'une note

-`[[ ]] doubles crochets avec Alt Gr + 5` 

Lorsque tu ouvres les doubles crochets, tu vas voir la liste de toutes les notes de ton coffre apparaître.
Ainsi, en connaissant le nom exact de la note vers laquelle tu souhaites pointer, tu peux continuer d'écrire son nom.
Sinon, tu peux cliquer sur la note de votre choix dans la liste déroulante.
![[../Les pièces jointes/Pasted image 20211029123039.png|400]]
Une fois la note sélectionnée, les doubles crochets vont automatiquement se refermer.

*Comment l'écrire en mode éditer*
```md
[[Tour d'horizon de l'interface et de ce qu'il faut connaître]]
```

*Le rendu en mode aperçu*
[[2 - Tour d'horizon de l'interface et de ce qu'il faut connaître]]

---

### Créer un lien renvoyant vers un niveau de titre précis à l'intérieur d'une note

Lorsque tu crées un lien, tu peux à la fin de celui-ci écrire le caractère `#` pour avoir la liste des niveaux de titres présents dans la note vers laquelle tu pointes.
Cela te permet de renvoyer vers une section plus fine de ta note.
Il te suffira alors de sélectionner le titre voulu une fois les premières lettres écrites.

![[../Les pièces jointes/Pasted image 20211027072719.png|400]]

*Comment l'écrire en mode éditer*
```md
[[Tour d'horizon de l'interface et de ce qu'il faut connaître#Le volet de gauche]]
```

*Le rendu en mode aperçu*
[[2 - Tour d'horizon de l'interface et de ce qu'il faut connaître#Le volet de gauche]]

---

### Créer un lien renvoyant vers l'endroit précis d'un paragraphe

Si tu souhaites être encore plus fin dans le lien de renvoi créé, tu peux écrire le caractère `^` puis sélectionner la section vers laquelle tu souhaites pointer.
Obsidian va alors créer une référence à l'intérieur de la note de destination.
Ainsi, lorsque tu cliqueras sur ce lien, Obsidian te renverra vers la section de la note en la surlignant pour la rendre plus visible.
![[../Les pièces jointes/Pasted image 20211027073125.png|400]]
*étape 1 le caractère `^` à la fin de la note de renvoi*

![[../Les pièces jointes/Pasted image 20211027073202.png|400]]

*étape 2 sélectionner le bloc vers lequel renvoyer puis valider le lien en fermant les crochets*
![[../Les pièces jointes/Pasted image 20211027073338.png]]
*voici ce qu'Obsidian te montrera quand tu cliqueras sur le nouveau lien créé*

![[../Les pièces jointes/Pasted image 20211027073453.png]]
*Et voici la référence que le logiciel créé*
![[../Les pièces jointes/Pasted image 20211027074308.png|400]]
*ainsi que le résultat du lien en mode aperçu*

À noter que tu peux également utiliser la syntaxe `[[^]]` pour créer un lien qui pointe vers un paragraphe n'importe où dans la note de destination. 
Si tu as par exemple en tête un mot précis, mais que tu ne sais plus où il se situe dans la note, tu peux t'aider en commençant à taper ton terme de recherche.
![[../Les pièces jointes/Pasted image 20211106155655.png|400]]
*exemple ici en recherchant plugin tiers sur l'ensemble du contenu de toutes les notes du vault*

---

### Changer le nom du lien qui s'affiche (créer un alias)

Par défaut, lorsque tu crées un lien, Obsidian va nommer le lien en mettant le titre de la note.
Quand tu crées un lien en renvoyant vers un niveau de titre, Obsidian nommera le lien en se basant sur le niveau de titre.
Mais quand tu renvoies vers une section précise qui n'est ni la note dans sa globalité, ni un niveau de titre, il va créer une référence faite de chiffres et de lettres.

![[../Les pièces jointes/Pasted image 20211114164828.png]]*exemple d'un lien créé vers une section précise avant d'avoir créé un alias, à gauche le mode édition, à droite le mode aperçu *

Créer un alias peut alors s'avérer très pratique si tu veux rendre le lien plus sexy, et l'intégrer à l'intérieur d'une phrase par exemple.
Il te suffit de mettre la barre oblique `|` en utilisant le raccourci `AltGr + 6` puis de mettre le texte que tu souhaites
![[../Les pièces jointes/Pasted image 20211114164936.png]]*à gauche le mode édition, à droite le mode aperçu*

---

### Renvoyer vers un paragraphe à l'intérieur de la note que tu consultes

Dans certains cas, tu auras peut-être besoin de créer un sommaire ou un index que tu placeras au sommet de ta note.
Ou encore si ta note est longue, peut-être auras-tu besoin de mettre une référence vers un autre paragraphe.
Le principe est le même que si tu devais créer un lien vers une note, sauf qu'à la place de commencer par le nom d'une note, tu vas tout simplement mettre un `#` ou un `^`. 

Exemple avec les captures suivantes :
![[../Les pièces jointes/Pasted image 20211106154901.png|400]]
*la syntaxe en mode édition*

![[../Les pièces jointes/Pasted image 20211106154955.png|400]]
*le résultat en mode aperçu, chaque lien renvoi vers le paragraphe concerné*

---

### Les tags un autre moyen de lier tes notes
![[../Les pièces jointes/Pasted image 20211106160052.png]]
Lorsque que tu crées une note, tu as la possibilité à l'intérieur de celle-ci d'ajouter un `#` suivi du mot qui caractérisera l'information à laquelle tu souhaites associer cette note.
Les `#` sont utiles à plusieurs égards : 
- Ils te permettent de mieux retrouver les informations
- Ils te sont également utiles dans la vue graphique, pour créer des filtres
- Ils peuvent aussi être utiles lors de la visualisation de données, pour par exemple créer des tableaux de visualisation avec le plugin Dataview afin de mieux visualiser tes notes (ce sujet est évoqué dans la formation complète).

À titre d'exemple, si tu as activé le plugin "Volet des tags", tu peux visualiser très facilement dans le volet de droite le nombre d'utilisations des tags # présents dans ton vault.
![[../Les pièces jointes/Pasted image 20211106160604.png]]

Pour une bonne première approche, retiens qu'un tag ne peut pas contenir d'espace, il faut donc mettre un seul mot, ou plusieurs mots avec des tirets.
Tu peux aussi faire des sous niveaux dans les hashtags en utilisant le `/`.
Un peu comme si tu devais créer un "dossier dans le dossier" sauf que c'est un "tag dans un tag".
Par exemple, en écrivant `#2021/formation/Obsidian/hashtags`, l'information sera répertoriée de la manière suivante.
![[../Les pièces jointes/Pasted image 20211106161723.png]]

Tu le verras en utilisant Obsidian, je conseille d'utiliser les tags avec modération, et dans un but bien précis. 
Nous verrons ensemble dans la formation complète comment utiliser les tags de manière pertinente.

---

## Pour résumer
- Nous avons vu qu'un lien était un moyen de connecter des notes entre elles
- Qu'un lien est un moyen de se libérer de la rigidité des dossiers en permettant de créer des ponts entre les idées et les sujets
- Je t'ai montré deux exemples d'utilisation concrètes: 
	- Pour un passionné de cuisine
	- Dans le cadre du travail
- Nous avons ensuite vu comment créer les différents types de liens :
	- Pour renvoyer vers la globalité d'une note
	- Pour renvoyer vers un paragraphe précis grâce aux différents niveaux de titres
	- Pour renvoyer vers n'importe quelle partie du texte de la note vers laquelle tu pointes
	- Pour renvoyer au sein même de la note que tu édites
- On a également vu comment créer un alias pour rendre les notes plus sexy
- Et enfin, nous avons vu comment utiliser les tags et "sous-tags" pour là aussi lier les notes

---

[[3 - Comment créer tes premières notes, tes dossiers et commencer à jouer avec l'interface|< Pour revenir au précédent module]] | [[5 - Comment t'amuser avec la vue graphique| Pour accéder au prochain module >]]

---

2023 ™. Tous droits réservés [cerveau-numerique.fr](https://cerveau-numerique.fr/)