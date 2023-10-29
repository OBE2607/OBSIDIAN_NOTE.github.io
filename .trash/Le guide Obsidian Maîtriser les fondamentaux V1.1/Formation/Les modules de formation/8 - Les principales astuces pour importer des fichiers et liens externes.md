*Revenir au [[010NOTE OBSIDIAN/001TEST/Le commencement|commencement]]*
![[../Les pièces jointes/Le guide Obsidian.jpg]]

# 8 - Les principales astuces pour importer des fichiers et liens externes
1.  [[#Introduction]]
2. [[#3 manières pertinentes d'insérer des liens vers des sites externes]]
3.  [[#Les formats de fichiers reconnus par Obsidian]]
4.  [[#Importer une image dans ton coffre et modifier sa taille en mode aperçu]]
5.  [[#Te servir d'une image en ligne pour l'afficher dans ta note]]
6.  [[#Insérer un PDF]]
7.  [[#Embarquer une vidéo youtube dans une note]]
8. [[#Pour résumer]]

---

## Introduction

Prendre des notes ne se résume pas qu'à écrire du texte, c'est aussi insérer des fichiers et insérer des liens pour mettre en forme tes notes.
Je vais donc te montrer les principaux points à connaître pour facilement  importer tes fichiers et créer des liens.

Mais avant cela, je te donne (ou redonne) un conseil, en fonction de comment tu vas organiser des notes et si tu vas créer des dossiers, pense bien à aller dans *Paramètres > Fichiers et liens > Emplacement par défaut des nouvelles pièces jointes*.

Si tu as tendance à créer beaucoup de dossiers, alors préfère peut-être le paramètre *"Dans le sous dossier, sous le dossier actuel"*. 
Cela te permettra de facilement retrouver des notes en fonction de tes dossiers.

Si par contre, tu n'utilises pas ou peu de dossiers, alors je te conseille de créer un dossier Pièces jointes et de choisir le paramètre *"Dans le dossier spécifique si dessous>Nom de ton dossier"* 

---

## 3 manières pertinentes d'insérer des liens vers des sites externes

Pour insérer un lien vers un site externe, tu peux :
- Copier/Coller directement l'URL sans titre, ni mise en forme
- Télécharger le plugin "Auto link title". 
	- Pour que le titre de la page web soit directement synchronisé au moment de coller la note  
- Appuyer sur le raccourci `Ctrl + K`. 
	- Cela te permettra d'ouvrir des crochets et des parenthèses `[]()` et te permettre créer un lien de manière plus pertinente `[Nom que tu veux donner au lien](L'endroit ou coller l'URL)`

*Le lien à coller en mode éditer*
```md
Premier exemple avec un lien simple : 
- https://cerveau-numerique.fr/

Second exemple d'un lien collé avec le plugin "Auto link title" : 
- [Boostez votre productivité grâce à votre second cerveau](https://cerveau-numerique.fr/)

Troisième exemple en personnalisant manuellement le nom du lien:
- [Voici un lien vers le site cerveau-numérique.fr](https://cerveau-numerique.fr/)
```

*Le résultat en mode aperçu :*
Premier exemple avec un lien simple : 
- https://cerveau-numerique.fr/

Second exemple d'un lien collé avec le plugin "Auto link title" : 
- [Boostez votre productivité grâce à votre second cerveau](https://cerveau-numerique.fr/)

Troisième exemple en personnalisant manuellement le nom du lien:
- [Voici un lien vers le site cerveau-numérique.fr](https://cerveau-numerique.fr/)

---

## Les formats de fichiers reconnus par Obsidian 

Voici la liste des principaux formats reconnus par le logiciel.

1. Fichiers Markdown: `md`;
2. Fichiers Image: `png`, `jpg`, `jpeg`, `gif`, `bmp`, `svg`;
3. Fichiers Audio: `mp3`, `webm`, `wav`, `m4a`, `ogg`, `3gp`, `flac`;
4. Fichiers Video: `mp4`, `webm`, `ogv`;
5. Fichiers PDF: `pdf`.

---

## Importer une image dans ton coffre et modifier sa taille en mode aperçu

Pour importer une image, un simple "glisser/déposer" depuis ton explorateur de fichier vers l'endroit choisi dans ta note suffit.
Obsidian importera cette image dans ton "vault" et la mettra dans le dossier que tu as choisi dans *Paramètres > Fichiers et Liens > Emplacement par défaut des nouvelles pièces jointes*.
Lors d'un "glisser/déposer", Obsidian affichera en mode aperçu la taille exacte de l'image.
Cependant, si tu n'es pas satisfait de la taille affichée, tu peux modifier l'échelle en ajoutant à la fin du fichier la barre oblique `|` en appuyant `Alt Gr + 6`, puis en insérant un nombre.
Voici un exemple avec les images suivantes.

*Comment l'écrire en mode éditer*
```md
Image / 100
![[nick-morrison-FHnnjk1Yj7Y-unsplash.jpg|100]]

Image / 200
![[nick-morrison-FHnnjk1Yj7Y-unsplash.jpg|200]]

Image / 400
![[nick-morrison-FHnnjk1Yj7Y-unsplash.jpg|400]]
```

*Le résultat en mode aperçu :*

Image / 100
![[../Les pièces jointes/nick-morrison-FHnnjk1Yj7Y-unsplash.jpg|100]]

Image / 200
![[../Les pièces jointes/nick-morrison-FHnnjk1Yj7Y-unsplash.jpg|200]]

Image / 400
![[../Les pièces jointes/nick-morrison-FHnnjk1Yj7Y-unsplash.jpg|400]]

---

## Te servir d'une image en ligne pour l'afficher dans ta note

Pour éviter de surcharger ton vault, tu peux simplement utiliser une image déjà présente sur un site.
C'est un peu le même principe que pour insérer un lien avec le raccourci `` []() Ctrl + K . 
Il te suffit de rajouter un `!` devant le premier crochet pour rendre l'image visible en mode aperçu.
Et c'est le même principe, tu peux modifier la taille en insérant entre les crochets la barre oblique suivie d'un numéro.

*Comment l'écrire en mode éditer*
```md
Image / 100
![Photo Cheikh|50](https://cerveau-numerique.fr/wp-content/uploads/2022/06/Cheikh-NDiaye-600-X-960.png)

Image / 100
![Photo Cheikh|100](https://cerveau-numerique.fr/wp-content/uploads/2022/06/Cheikh-NDiaye-600-X-960.png)

Image / 200
![Photo Cheikh|200](https://cerveau-numerique.fr/wp-content/uploads/2022/06/Cheikh-NDiaye-600-X-960.png)
```

*Le résultat en mode aperçu :*

Image / 100
![Photo Cheikh|50](https://cerveau-numerique.fr/wp-content/uploads/2022/06/Cheikh-NDiaye-600-X-960.png)

Image / 100
![Photo Cheikh|100](https://cerveau-numerique.fr/wp-content/uploads/2022/06/Cheikh-NDiaye-600-X-960.png)

Image / 200
![Photo Cheikh|200](https://cerveau-numerique.fr/wp-content/uploads/2022/06/Cheikh-NDiaye-600-X-960.png)

---

## Insérer un PDF 

Tu peux insérer un PDF en faisant là aussi un "glisser / déposer" directement dans ta note 
Sache également que tu peux sélectionner la page vers laquelle tu souhaites renvoyer.

![[../Les pièces jointes/Personal Notes - Teacher Appreciation Week _ by Slidesgo.pdf]]


---

## Embarquer une vidéo youtube dans une note

La plupart des sites médias facilitent l'intégration de leur contenu.
Bonne nouvelle, Obsidian permet d'accepter ce contenu très facilement !
Pour cela, il te suffit de te rendre sur une vidéo Youtube, puis de cliquer sur "intégrer".
Cela devient facile d'ajouter une vidéo et de prendre des notes dessus.
Ce système fonctionne aussi avec Twitter et d'autres sites média.

![[../Les pièces jointes/Pasted image 20211106173656.png]]

![[../Les pièces jointes/Pasted image 20211106173554.png]]


*Le lien à coller en mode éditer*
```md
<iframe width="560" height="315" src="https://www.youtube.com/embed/ym7WZym0t30" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```

*Le résultat en mode aperçu :*
<iframe width="560" height="315" src="https://www.youtube.com/embed/ym7WZym0t30" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---

## Pour résumer

- Nous avons vu qu'il était important de configurer le dossier des pièces jointes en choisissant parmi : 
	- Un dossier spécifique
	- Le sous dossier du dossier actuel
- On a également vu les 3 manières pertinentes d'insérer des liens externes le raccourci `Ctrl + K` ainsi que le plugin "Auto link title"
- Ensuite, nous avons vu les principaux formats acceptés par le logiciel
- Je t'ai montré comment importer une image dans ton coffre, modifier sa taille avec la barre oblique `|` pour l'adapter en fonction de ton besoin
- On a aussi vu qu'il était possible d'utiliser une image en ligne pour éviter de surcharger ton vault
- Et enfin, je t'ai montré comme embarquer une vidéo Youtube pour l'insérer dans ta note

---

[[7 - On va plus loin avec la mise en forme de tes notes|< Pour revenir au précédent module]] | [[9 - Mes 7conseils pour bien organiser tes notes| Pour accéder au prochain module >]]

---
2023 ™. Tous droits réservés [cerveau-numerique.fr](https://cerveau-numerique.fr/)