# Notes semaine 2 sur les bases du html

## Inventeur

Tim Berners-Lee

## Balises

sémantiquement, elles servent à réferencer les élements auprès des moteur de recherches.

- `<>` **
- `<!-- mon texte -->` *commentaire*
- `<hn>` *titre de niveau n*
- `<p>` *paragraphe*
- `<ul>` *unordered list*
- `<ol>` *ordered list*
- `<li>` *élements d'une liste*
- `<nombalise />` *balises auto-fermantes*
  - `<hr />` *permet de faire une séparation entre deux sujets / sections*
- `<a href"URL">` *balise d'ancre (pour faire des liens)*
- `<section>` *définit sémentiquement un bloc de texte comme une section(pour le réferencement)*
- `<article>` *définit sémentiquement un bloc de texte comme un article(souvent le bloc enfant de section)*
- `<aside>` *définit sémentiquement un bloc sur le côté de ma page*
- `<code>` *définit sémentiquement un bloc de code*

## Attributs

Servent à paramétrer ou ajouter de l'information dans nos balise html

*exemple* `<img src="URL" alt="description />`

- `style` permet d'ajouter du css sur une balise donné directement dans le code html(à proscrire)
- `class` permet de manipuler une classe de bloc en css (tous les élements de la même classe pourront avoir des styles communs, même si la balise est totalement differente) pour la nommer on utilise une notation BEM(bloc-element-modification)

## Tips

- `CTRL + MAJ + r` raccourcis pour un navigateur (vide le cache + actualise)
- `CTRL + /` raccourcis VSCode pour balise commentaire
- `localhost` sur un navigateur pour aller dans le dossier html de ma machine
- `nom balise + TAB` mets nom balise au format `<nom balise></nom balise>` (pour une balise connu genre h1)
- `lorem + TAB` pour génerer du texte auto ( si on ajoute un nombre on aura un texte basé sur un nb de caractere)
- `F12` inspecter le html dans le navigateur
- `maintient ALT +fleche` deplace une ligne dans VSCode
- `'!' + Tab`  pour créer la structure meta html dans VSCode(grâce à l'outil emmet)
- ```md
  `h1+h2+p*3+h2+h3+ul>li*5^h3+p+ul>li*6` + Tab
  ```
  pour creer la structure du site(grâce aux formules emmet -> [lien](https://laconsole.dev/blog/raccourcis-emmet-indispensables))
- `CTRL + MAJ + P > ecrire "wrap"(envelopper une abreviation) puis le nom de la balise`  pour mettre du texte (selectionné avant) entre balises
- `CTRL + d` selectionne toutes les occurences du texte (selectionné avant)
- `selection > "utiliser CTRL + clic pour l'option multicurseur"(si pas déjà parametré)` cette option permet de selectionné plusieurs mots séparés dans un même texte
- `CTRL + l` selectionner la ligne ou le curseur se trouve

## Definitions

- **CDN(content delivery network)** Ce sont des plateformes(concretement des serveurs) qui contiennent des ressources mises à disposition des dev afin qu'ils soient intégrés aux page web(ex: police de caracteres, librairies css,...)

## Liens

- [liste des balises avec leur type(inline/block/...)](https://htmlreference.io/)
- [glossaire des élements sémantiques du html](https://developer.mozilla.org/fr/docs/Glossary/Semantics)
- [choisir des polices de caracteres(de google)](https://fonts.google.com/)
