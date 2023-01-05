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
            --gap: 0px,
            display: flex,
            flex-wrap: wrap,
        ),
        modifiers: ( // Liste des modifieurs contenant chacun une liste de propriétés qui surchargent celles par défaut
            // Axe main
            main-start: ( // c-flex m-main-start
                justify-content: flex-start
            ),
            main-center: ( // c-flex m-main-center
                justify-content: center
            ),
            main-end: ( // c-flex m-main-end
                justify-content: flex-end
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
            // Axe cross
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
            // Wrap / retour à la ligne
            nowrap: ( // c-flex m-nowrap
                flex-wrap: nowrap
            ),
            wrap-reverse: ( // c-flex m-wrap-reverse
                flex-wrap: wrap-reverse
            ),
            // Direction
            column: ( // c-flex m-column
                flex-direction: column
            ),
            column-reverse: ( // c-flex m-column-reverse
                flex-direction: column-reverse
            ),
            row-reverse: ( // c-flex m-cross-row-reverse
                flex-direction: row-reverse
            ),
            // Gap
            // Surcharge de la variable CSS --ita-gap pour compatibilité avec c-dim
            gap-1: ( // c-flex m-gap-1
                --ita-gap: my-spacing(2),
                gap: my-spacing(2)
            ),
            gap-2: ( // c-flex m-gap-2
                --ita-gap: my-spacing(4),
                gap: my-spacing(4)
            ),
            gap-3: ( // c-flex m-gap-3
                --ita-gap: my-spacing(8),
                gap: my-spacing(8)
            )
        )
    )
);
``` 

