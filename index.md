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
        padding: var(--ita-spacing-4);
        background-color: var(--ita-color-primary-900);
        color: var(--ita-color-primary-200);
        font-family: var(--ita-font-family-mono);
        font-size: 1rem;
        line-height: 1.5rem;
        padding-bottom: 50vh;
    }
    .c-flex {
        background-color: var(--ita-color-primary-800);
    }
    .c-flex > * {
        background-color: var(--ita-color-primary-500);
        color: var(--ita-color-primary-900);
        border: var(--ita-border-6);
        padding: var(--ita-spacing-4);
    }
    .c-flex + .c-flex {
        margin-top: var(--ita-spacing-4);
    }
    .c-flex + h2 {
        margin-top: var(--ita-spacing-12);
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
