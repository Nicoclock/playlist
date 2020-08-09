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
