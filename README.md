# Commandes GIT

## git init

- initialise le répertoire courant comme dépôt git
- création du dossier .git contenant les infos nécessaires à la gestion du dépôt

---

## git status

- donne l'état du dépôt à un moment donné

---

## git add

- ajout d'un ou plusieurs fichiers dans la zone de surveillance

    - `git add README.md` ajoute le fichier README.md

    - `git add fichier1 fichier2` ajoute les fichiers listés

    - `git add .` ajoute tous les fichiers non surveillés 

- à chaque modification, on doit ajouter la nouvelle version du fichier dans la zone de surveillance

---

## git rm --cached 

- retire un ou plusieurs fichiers de la zone de surveillance

    - `git rm --cached README.md`

---

## git commit

- enregistre dans l'historique une étape du développement

    - `git commit -m "message explicite sur l'étape de développement"`

- avant l'envoi sur un repo distant, on peut modifier le message du commit

    - `git commit --amend`

- cette commande ouvre l'éditeur de texte [vi](http://wiki.linux-france.org/wiki/Utilisation_de_vi)

## VI

- quelques commandes de base :

    - i pour insérer du contenu

    - esc pour sortir de l'édition

    - :x pour sauvegarder les modifs

    - :q! pour quitter sans sauvegarder

## git remote

- avec add, on donne une adresse distante où envoyer notre dépôt local

    - `git remote add origin (nom par défaut) git@github.com:xxx (adresse ssh du dépôt)`

- avec -v, on liste les adresses distantes enregistrées

    - `git remove -v`


## git push

- lors du 1er envoi, il faut lier la branche locale courante à une branche du dépôt distant

    - `git push --set-upstream (ou -u) origin (dépôt distant) master (branche distante)`

- lors des envois de mise à jour, git saura comment lier cette branche à une branche distante

    - `git push`

# Commandes GIT

## git init

- initialise le répertoire courant comme dépôt git
- création du dossier .git contenant les infos nécessaires à la gestion du dépôt

---

## git status

- donne l'état du dépôt à un moment donné

---

## git add

- ajout d'un ou plusieurs fichiers dans la zone de surveillance

    - `git add README.md` ajoute le fichier README.md

    - `git add fichier1 fichier2` ajoute les fichiers listés

    - `git add .` ajoute tous les fichiers non surveillés 

- à chaque modification, on doit ajouter la nouvelle version du fichier dans la zone de surveillance

---

## git rm --cached 

- retire un ou plusieurs fichiers de la zone de surveillance

    - `git rm --cached README.md`

---

## git commit

- enregistre dans l'historique une étape du développement

    - `git commit -m "message explicite sur l'étape de développement"`

- avant l'envoi sur un repo distant, on peut modifier le message du commit

    - `git commit --amend`

- cette commande ouvre l'éditeur de texte [vi](http://wiki.linux-france.org/wiki/Utilisation_de_vi)

## VI

- quelques commandes de base :

    - i pour insérer du contenu

    - esc pour sortir de l'édition

    - :x pour sauvegarder les modifs

    - :q! pour quitter sans sauvegarder

## git remote

- avec add, on donne une adresse distante où envoyer notre dépôt local

    - `git remote add origin (nom par défaut) git@github.com:xxx (adresse ssh du dépôt)`

- avec -v, on liste les adresses distantes enregistrées

    - `git remove -v`


## git push

- lors du 1er envoi, il faut lier la branche locale courante à une branche du dépôt distant

    - `git push --set-upstream (ou -u) origin (dépôt distant) master (branche distante)`

- lors des envois de mise à jour, git saura comment lier cette branche à une branche distante

    - `git push`

## git branch

- depuis la branche courante, on peut créer une nouvelle branche ET rester dans la branche courante

- si on est sur la branche master, `git branch henriette` va créer la branche henriette mais on restera sur la branche master

    - `git branch <nom_branche>`

- Astuce : on peut créer une nouvelle branche et se positionner dessus directement

    `git checkout -b <nom_branche>`

- on peut supprimer une branche

    - avec un warning si la branche n'a pas été pushée sur la branche distante

        - `git branch -d <nom_branche>`

    - sans warning ni vérification

        - `git branch -D <nom_branche>`