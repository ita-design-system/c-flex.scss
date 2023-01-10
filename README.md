# c-flex.scss

Composant CSS c-flex du système de design IT Automotive

## Installation avec Jekyll LibDoc distant

1. Installer Jekyll sur votre machine en suivant les [instructions](https://jekyllrb.com/docs/)
2. Ajouter un Gemfile contenant la ligne suivante

  ```ruby
  gem "jekyll-remote-theme"
  ```
  et exécuter `bundle install` pour installer le plugin.
3. Ajouter les lignes suivantes dans votre fichier de configuration LibDoc `_<NOM DU FICHIER>.yml`

  ```yml
  remote_theme: ita-design-system/jekyll-libdoc
  plugins:
    - jekyll-remote-theme
  ```
4. Exécuter `jekyll build` ou `jekyll build -c _votre-fichier-config.yml`

## Configuration

Organisation et description du fichier de configuration [_sass/_flex_generic.scss](_sass/_flex_generic.scss).

```scss
// EXEMPLE DE COMPOSANT GÉNÉRIQUE VIDE
$briks-components-generic: ( // SCSS map
    NOM_DU_COMPOSANT: ( // SCSS map | Nom du composant
        enabled: true, // Boolean | Composant activé true ou false
        responsive: true, // Boolean | Responsive activé true ou false
        defaults: (), // SCSS map | Liste des propriétés du composant par défaut (c-flex seul)
        modifiers: () // SCSS map | Liste des modifieurs
    )
);
/*
    C-FLEX
    Composant générique CSS ITADS
    https://github.com/ita-design-system/c-flex.scss
*/
// SCSS map
$briks-components-generic: ( 
    // Nom du composant
    flex: ( 
        // Composant activé true ou false
        enabled: true, 
        // Responsive activé true ou false
        responsive: true, 
        // Liste des propriétés c-flex par défaut
        defaults: ( 
            --ita-gap: 0px,
            gap: var(--ita-gap),
            display: flex,
            flex-wrap: wrap,
        ),
        // Rendu: 
        // .c-flex {
        //     --ita-gap: 0px,
        //     gap: var(--ita-gap),
        //     display: flex,
        //     flex-wrap: wrap,
        // }
        // Liste des modifieurs contenant chacun une liste de propriétés qui surchargent celles par défaut
        modifiers: ( 
            // Axe main
            // c-flex m-main-start
            main-start: ( 
                justify-content: flex-start
            ),
            // Rendu:
            // .c-flex.m-main-start {
            //     justify-content: flex-start
            // }
            // Même logique pour les autres modifieurs
            // c-flex m-main-center
            main-center: ( 
                justify-content: center
            ),
            // c-flex m-main-end
            main-end: ( // c-flex m-main-end
                justify-content: flex-end
            ),
            // c-flex m-main-space-between
            main-space-between: ( 
                justify-content: space-between
            ),
            // c-flex m-main-space-around
            main-space-around: ( 
                justify-content: space-around
            ),
            // c-flex m-main-space-evenly
            main-space-evenly: ( 
                justify-content: space-evenly
            ),
            // Axe cross
            // c-flex m-cross-center
            cross-center: ( 
                align-items: center
            ),
            // c-flex m-cross-baseline
            cross-baseline: ( 
                align-items: baseline
            ),
            // c-flex m-cross-start
            cross-start: ( 
                align-items: flex-start
            ),
            // c-flex m-cross-end
            cross-end: ( 
                align-items: flex-end
            ),
            // Wrap / retour à la ligne
            // c-flex m-nowrap
            nowrap: ( 
                flex-wrap: nowrap
            ),
            // c-flex m-wrap-reverse
            wrap-reverse: ( 
                flex-wrap: wrap-reverse
            ),
            // Direction
            // c-flex m-column
            column: ( 
                flex-direction: column
            ),
            // c-flex m-column-reverse
            column-reverse: ( 
                flex-direction: column-reverse
            ),
            // c-flex m-cross-row-reverse
            row-reverse: ( 
                flex-direction: row-reverse
            ),
            // Gap
            // Surcharge de la variable CSS
            // Compatible avec c-dim
            // c-flex m-gap-1
            gap-1: ( 
                --ita-gap: my-spacing(2)
            ),
            // c-flex m-gap-2
            gap-2: ( 
                --ita-gap: my-spacing(4)
            ),
            // c-flex m-gap-3
            gap-3: ( 
                --ita-gap: my-spacing(8)
            )
        )
    )
);
``` 

