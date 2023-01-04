---
title: Configuration
description: Description du fichier de configuration SCSS
# layout: libdoc/page-split
---

```scss
// EXEMPLE DE COMPOSANT VIDE
$briks-components-generic: ( // SCSS map
    NOM_DU_COMPOSANT: ( // SCSS map | Nom du composant
        enabled: true, // Boolean | Composant activé true ou false
        responsive: true, // Boolean | Responsive activé true ou false
        defaults: (), // SCSS map | Liste des propriétés du composant par défaut (c-flex seul)
        modifiers: ()
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
            main-start: (
                justify-content: flex-start
            ),
            main-end: (
                justify-content: flex-end
            ),
            cross-center: (
                align-items: center
            ),
            cross-baseline: (
                align-items: baseline
            ),
            cross-start: (
                align-items: flex-start
            ),
            cross-end: (
                align-items: flex-end
            ),
            nowrap: (
                flex-wrap: nowrap
            ),
            column: (
                flex-direction: column
            ),
            column-reverse: (
                flex-direction: column-reverse
            ),
            row-reverse: (
                flex-direction: row-reverse
            )
        )
    )
);
``` 
