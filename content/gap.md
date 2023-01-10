---
title: Gap
description: Modifieurs relatifs à l'espace entre les items flexbox
layout: libdoc/page-split
order: 600
---
```html
<p>Les différentes valeurs de la propriété "gap" sont à renseigner dans les modifieurs ou dans les valeurs par défaut. Dans cette documentation, il y a 3 valeurs de gap à titre d'exemple mais leur quantité n'est pas limitée. Cependant, plus la quantité est élevée, plus les performances du frameworks sont impactées. Il est recommandé d'aligner les valeurs de gap sur les design tokens d'espacements <strong>$briks-spacings</strong>.</p>

<h2>m-gap-1</h2>
<p>Pour <strong>gap: var(--ita-spacing-2)</strong>, valeur générique utilisée à titre d'exemple, celle-ci est à personnaliser en fonction du projet</p>
<div class="c-flex">
    <div>Item 1 <br><strong>sans gap</strong></div>
    <div>Item 2 <br><strong>sans gap</strong></div>
    <div>Item 3 <br><strong>sans gap</strong></div>
</div>
<div class="c-flex m-gap-1">
    <div>Item 1 <br><strong>avec modifieur m-gap-1</strong></div>
    <div>Item 2 <br><strong>avec modifieur m-gap-1</strong></div>
    <div>Item 3 <br><strong>avec modifieur m-gap-1</strong></div>
</div>

<h2>m-gap-2</h2>
<p>Pour <strong>gap: var(--ita-spacing-4)</strong>, valeur générique utilisée à titre d'exemple, celle-ci est à personnaliser en fonction du projet</p>
<div class="c-flex m-gap-2">
    <div>Item 1 <br><strong>avec modifieur m-gap-2</strong></div>
    <div>Item 2 <br><strong>avec modifieur m-gap-2</strong></div>
    <div>Item 3 <br><strong>avec modifieur m-gap-2</strong></div>
</div>

<h2>m-gap-3</h2>
<p>Pour <strong>gap: var(--ita-spacing-8)</strong>, valeur générique utilisée à titre d'exemple, celle-ci est à personnaliser en fonction du projet</p>
<div class="c-flex m-gap-2">
    <div>Item 1 <br><strong>avec modifieur m-gap-3</strong></div>
    <div>Item 2 <br><strong>avec modifieur m-gap-3</strong></div>
    <div>Item 3 <br><strong>avec modifieur m-gap-3</strong></div>
</div>

<h2>Exemple responsive</h2>
<p>L'exemple suivant affiche:</p>
<ul>
    <li>Un gap égal à la valeur du spacing 8 sur les tailles d'écran supérieures à sm</li>
    <li>Un gap égal à la valeur du spacing 4 sur la taille d'écran sm</li>
    <li>Un gap égal à la valeur du spacing 2 sur la taille d'écran xs</li>
</ul>
<div class="c-flex m-gap-3" m-gap-2="sm" m-gap-1="xs">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
</div>
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
{:.playground title="Modifieurs pour le gap"}


