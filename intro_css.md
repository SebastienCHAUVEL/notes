# Notes semaine 2 sur les bases du css

## Important

`<link rel="stylesheet" href="style.css" />` dans le head de mon fichier html pour lier un style css sur mon site

## Code

- `nav li{}` pour cibler les element de liste **dans** un bloc nav(marche pour tout les element à l'interieur d'un element)
- ```md
  h1,
  h2{

  }
  ```
  permet de cibler plusieurs element(ici h1 et h2)
- `rgb(rouge.vert.bleu.opacity)` ex `color: rgb(255.255.255.0.5);`
- `#code-hexa-de-la-couleur` ex `color: #FFFFFF;`
- **rem** ex `font-size: 3rem;` unité de mesure relative au reglage du navigateur(contrairement à px qui est absolut): 1 rem equivaut au réglage du navigateur de l'user pour une police(si police user: 16px, 2 rem=32px) et pour forcé son reglage, mettre genre font-size: 16px; dans le body, et rem sera relative à ces 16px
- `margin: 2rem auto;` 2rem: la marge exterieur verticale sera de 2 fois la taille de la police du navigateur; auto: la marge horrizontale exterieur du bloc se centre automatiquement selon la taille de l'ecran
- `border-radius: 24px;` permet d'arrondir les coin d'un bloc (plus la valeur est grande, plus l'arrondit l'est aussi)

## Pseudo classe

Permet de selectionner un élement sur une action

-`a:visited` une fois visité
-`a:hover` au survol

## Tips

- `coolors.co` outil pour génerer des palettes de couleurs stylés
- `color pickers` ensemble d'outils(extension navigateur) pour pick le code hexadecimal sur une page web

## Liens

- [fichier reset by eric meyers](https://meyerweb.com/eric/tools/css/reset/) (très radical)
- [fichier reset by josh comeau](https://www.joshwcomeau.com/css/custom-css-reset/) (pas mal d'apres Olivier, plus recent donc plus actuel que celui de meyers)