# c-flex.scss

Composant CSS c-flex du système de design IT Automotive

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
$briks-components-generic: ( // SCSS map
    flex: ( // Nom du composant
        enabled: true, // Composant activé true ou false
        responsive: true, // Responsive activé true ou false
        defaults: ( // Liste des propriétés c-flex par défaut
            display: flex,
            flex-wrap: wrap,
        ),
        modifiers: ( // Liste des modifieurs contenant chacun une liste de propriétés qui surchargent celles par défaut
            main-center: ( // c-flex m-main-center
                justify-content: center
            ),
            main-space-between: ( // c-flex m-main-space-between
                justify-content: space-between
            ),
            main-space-around: ( // c-flex m-main-space-around
                justify-content: space-around
            ),
            main-space-evenly: ( // c-flex m-main-space-evenly
                justify-content: space-evenly
            ),
            main-start: ( // c-flex m-main-start
                justify-content: flex-start
            ),
            main-end: ( // c-flex m-main-end
                justify-content: flex-end
            ),
            cross-center: ( // c-flex m-cross-center
                align-items: center
            ),
            cross-baseline: ( // c-flex m-cross-baseline
                align-items: baseline
            ),
            cross-start: ( // c-flex m-cross-start
                align-items: flex-start
            ),
            cross-end: ( // c-flex m-cross-end
                align-items: flex-end
            ),
            nowrap: ( // c-flex m-nowrap
                flex-wrap: nowrap
            ),
            column: ( // c-flex m-column
                flex-direction: column
            ),
            column-reverse: ( // c-flex m-column-reverse
                flex-direction: column-reverse
            ),
            row-reverse: ( // c-flex m-cross-row-reverse
                flex-direction: row-reverse
            )
        )
    )
);
``` 

