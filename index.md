---
layout: libdoc/page-split
---
```html
<div class="c-flex">
    <div>item un</div>
    <div>item deux</div>
    <div>item trois</div>
    <div>item quatre</div>
</div>
<ul class="c-flex">
    <li>item un</li>
    <li>item deux</li>
    <li>item trois</li>
    <li>item quatre</li>
</ul>
<!-- DEMO UNIQUEMENT -->
<style>
    body {
        padding: 1rem;
        background-color: ghostwhite;
        font-family: monospace;
    }
    .c-flex {
        background-color: #EEE;
    }
    .c-flex > * {
        background-color: #e8ffba;
        border: 0.5px dashed grey;
        padding: 1rem;
    }
    .c-flex + .c-flex {
        margin-top: 1rem;
    }
</style>
```
{:.playground title="Exemple générique"}

Composant CSS de grille flexbox polyvalent, personnalisable et cascadable. c-flex peut être personnalisé en fonction du projet.

```scss
$briks-components-generic: (
    flex: (
        enabled: true,
        responsive: true,
        defaults: (
            display: flex,
            flex-wrap: wrap,
        ),
        modifiers: (
            main-center: (
                justify-content: center
            ),
            main-space-between: (
                justify-content: space-between
            ),
            main-space-around: (
                justify-content: space-around
            ),
            main-space-evenly: (
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
