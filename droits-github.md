# Droits Github
## Creer une clef ssh
- Ouvrir un terminal
- Creer une clef ssh : ssh-keygen puis accepter les options par defaut
- Copier la clef dans le presse papier : cat .ssh/id_rsa.pub
- Aller dans le Profil de l'utilisateur Github, rubrique SSH et ajouter la clef

## Verifier les droits
- Recuperer l'url ssh d'un depot github, en allant sur le repository et en cliquant sur "Clone or download"
ex: git@github.com:legedeon/documentation.git
- Ouvrir un terminal
- Cloner le depot: git clone git@github.com:legedeon/documentation.git
- Faire la modif souhaitee
- Commiter la modif: git add "filename"; git commit -m "commentaire de commit"; git push origin master

- Sinon on peut modifier directement le master via l'interface web et commiter sur l'interface

cat .git/config
donne la config git avec l'origine et le master et les branches

## Ajouter un collaborateur
Dans Settings Collaborator

## Liens
https://help.github.com/articles/connecting-to-github-with-ssh/
