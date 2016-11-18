# Exercice de TP:

Titouan Teyssier - TitouanT -

## 1. Création dépôt local:

a) dans le répertoire tp-note-locale: `git init`

b) création d'un readme: `echo "Titouan Teyssier" > README.md`

c) création du gitignore et initialisation pour ignorer les fichier finissant par ~: `echo "*~" > .gitignore`

d) Validation des modif et création d'une version:
+ `git add README.md .gitignore`
+	`git commit -m "premier commit"`

e) on crée un dépot distant vide sur github nommé tp-note-local.

f) pour envoyer notre dépot local sur github il faut:
+ lui indiqué le l'url ou il se trouve sur le repo distant:
`git remote add origin git@github.com:TitouanT/tp-note-local.git`
+ puis on push: `git push -u origin master`

## 2. Récupération dépôt distant:

a) création du dépôt tp-note-distant sur github

b) récupération en local: `git clone git@github.com:TitouanT/tp-note-distant.git`

c) création d'un readme: `echo "Titouan Teyssier" > README.md`

d) voir le README du dépôt.

e) une fois toutes les modif effectuée: `git push`

## 3. Pull request:

a) on fork le dépôt situer a cette adresse: https://github.com/vjousse/conduite-projet

puis on le récupere en locale: `git clone git@github.com:TitouanT/conduite-projet.git`

b) modification du README (ajout de mon nom et prénom).

+ `git add README.md`
+	`git commit -m "ajout de mon nom prénom"`
+	`git push`

c) on fait un pull request depuis github.

## 4. merge

a) Si on travaille à plusieurs sur un fichier alors le dernier qui push ces modification devra faire un merge.

b) Il faut :
+ ouvrir les fichier qui présentent un conflit (git status pour voir lesquels) et faire les modifications nécessaire (retirer les balise ajouté par git et choisir ce qu'il faut faire avec le code à l'intérieur de ces balises).
+ ajouté les fichier: `git add <les fichier qui étaitent en conflit>`
+ faire un commit: `git commit`
