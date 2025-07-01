# Note 3e jour

## Github

Github est une plateforme de services en ligne qui permet de stocker et partager des projets (comme une grande bibliothèque). C’est un vrai réseau social permettant de partager son code, de communiquer avec d’autres développeurs en postant des commentaires, des issues, etc.

GitHub est probablement le réseau social de développeurs le plus populaire aujourd’hui, mais il existe également Gitlab, Bitbucket, etc.

## Git

Git est un outil de gestion de version en ligne de commande, qu’on doit installer en local sur sa machine pour l’utiliser.

## versionning

- Historique des modification
  - 1 version du code = 1 commit
  - possibilité de revenir à une ancienne version
- Travailler en équipe
  - coder à plusieurs en parrallèle
  - 1 monde parrallèle = 1 branche

## Concepts fondamentaux de Git

Pour un dossier de travail donné, Git manipule différents « espaces virtuels » :

- **Workspace(ou working directory)** espace stockant les modifications en cours qui ne sont pas prises en compte par Git
- **Staging area (ou index)**  espace stockant les modifications en cours qui seront prises en compte par Git dans le prochain commit.
- **Local repository** espace stockant les modifications prises en compte par Git dans les commits.
- **Remote repository** dépôt distant (sur GitHub par exemple) auquel est relié votre dépôt local. Les commits du dépôt local doivent y être pushés pour mettre le dépôt distant à jour et collaborer avec d’autres personnes.

![Shéma métaphorique](https://kourou.oclock.io/content/uploads/2020/09/git-github-1024x444.jpg)

![Shéma complet](https://kourou.oclock.io/content/uploads/2020/09/git-overview.png)

## invité de cmd

- `git --help` pour savoir toutes les commandes disponnibles
- `git [commande] -h` pour la doc d'une commande en particulier
- `git --version` pour connaitre sa version
- `git init` permet d'initialiser un repository(repo) git à partir d’un dossier courant(dans le dossier où on se trouve dans l'invité de commande). Si on veut ensuite le partager sur GitHub, il faudra alors paramétrer au moins un remote
- `git status` permet de visualiser l'état du repo git(si ils ont été add ou pas)
- `git add [nom du fichier/dossier]` permet d'activer l'enregistrement temporaire (dans l'index) des modif depuis le dernier commit (un pré-enregistrement avant de vérifier les erreurs et de commit) souvent `git add .` poru tout add dans "." ou `git add -A` pour add tout ce qu'il y a dans mon arborescence.
- `git commit -m "message de commit` enregistre l'ensemble des modif dans mon repo local avec le nom des modifs apportés
- `git commit -a` fait les deux dernieres commande en même temps (pas conseillé)
- `git clone {url} [nom-local]` récupère un repo distant (remote sur GitHub par exemple) en local, dans un dossier créé à la volée qu’il est possible de renommer (par défaut : nom du repo sur le remote)
- `git push` publie mes commits sur un remote repository(github par ex)
- `git log` historique de mes anciens commits
- `git commit -m "Ton message" --amend` change le message du commit précedent
- `git commit --amend --no-edit` ajouter des modifs au commit different (si on a oublier un truc avant de commit)
  
## Configuration de git

- `git config --global user.name "Sebastien CHAUVEL"`
- `git config --global user.email "monsieurchauvel22@gmail.com"`
- `git config --global core.editor code` définit VSCode comment éditeur de texte
- `git config --global color.ui true` Activation des couleurs dans le résultat des commandes Git

>`git config -l` pour vérifier les réglages

## Configurer d'une clé SSH

 >*nb: à ne faire qu'une fois par machine*

### Creation des clés

`ssh-keygen -t ed25519 -C "monsieurchauvel22@gmail.com"` génere une clée privé et une clé publique

### Ajout de la clé publique sur GitHub

`cat /home/student/.ssh/id_ed25519.pub` pour afficher ma clé publique

Copiez la clé, puis allez sur le site Github dans :

```md
Settings > SSH and GPG keys > New SSH key > Coller le contenu de la clé et valider
```

vérifier : `ssh -T git@github.com`

et accepter de faire confiance au site (taper "yes")

## Au quotidien

1. Je recupere un projet github sur mon repo `git clone {url} [nom-local]` (on peux changer son nom si on veut avec un 2e argument *optionnel*)
2. Je modifie mes fichiers
3. Je les enregistres CTRL+S
4. `git add .`
5. Quand jai "terminé" mon lot de modif ( répéter 1 à plusieurs fois ) `git status`
6. `git commit -m "message de commit`
7. Je les push sur github `git push`

## Vocabulaire

- **repository ou repo** le dossier sur lequel on va activer git
- **commit** enregistrement des modifications faites à un projet git
- **branche**
- **tracked file** les fichiers sur lesquels on souhaite enregistrés les modifications actuelles via `git add`
- **clé ssh** carte d'identité de ma machine pour github
