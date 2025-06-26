# Découverte de markdown

## Présentation de markdown

Markdown permet de donner un sens à du texte.

Il est très pratiqu pour prendre des notes.

## Les "commandes" de bases

De base le texte que l'on écrit correspond à un paragraphe.
Si je veux passer au paragraphe suivant je doit sauter une ligne.
Donc cette ligne est dans le même paragraphe

Cette ligne est un nouveau paragraphe

On peut préciser que du texte *en italique* ou **en gras** ou ***les deux***

On peut ~~barrer du texte~~

### Listes

On peut afficher des listes de deux manières.

Soit avec des `-`pour une liste non ordonnée (l'ordre des élements n'est pas important)

- papier toilette
- oranges
- livre très important

Soit avec des numéros pour une liste ordonnée(l'ordre des élements est important)

1. mettre de l'eau sur le feu
   1. prendre casserole
   2. ajouter de l'eau minérale
   3. allumer le feu
2. mettre les pâtes dans de l'eau bouillante
3. attendre 7min
4. égouter

On peut aussi faire des cases à cocher:

- [ ] manger
- [x] bouger

### Titres

On peut écrire de titres de différents niveaux

- `#` Permet d'ecrire un titre de niveau 1
- `##` Il existe plusieurs niveaux
- `###` Niveau 3
- `####` Niveau 4

### Tableau

| Prénom | Région | Âge |
| :---   | :---:  | ---:|
| Sébastien | Rhône-alpes | 30 |

- (alignements gérés grâce aux  `:`)
- la ligne d'en-tête est toujours en 2e

### Afficher du code

- en tant que dev, on voudra souvent afficher du code: on peut faire comme ça `ping google.com`
- ou en bloc:
  
  ```md
  # des trucs
  ## et d'autres
  ```

- >ou en discretion

### Des liens et des images

#### lien

[Je suis un lien](http://oclock.io)

#### image

![je suis une image](https://oclock.io/wp-content/uploads/2023/11/logo-noir-blanc-rouge-768x768_centre-rond720px.png)

![je suis une image local](./image.excalidraw.png)
