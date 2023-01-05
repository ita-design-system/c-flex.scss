---
title: Directions
description: Modifieurs relatifs à la propriété flex-direction
layout: libdoc/page-split
order: 400
---
```html
<h2>m-column</h2>
<p>Pour <strong>flex-direction: column</strong></p>
<div class="c-flex">
    <div>Item 1 <br><strong>sans modifieur m-column</strong></div>
    <div>Item 2 <br><strong>sans modifieur m-column</strong></div>
    <div>Item 3 <br><strong>sans modifieur m-column</strong></div>
</div>
<div class="c-flex m-column">
    <div>Item 1 <br><strong>avec modifieur m-column</strong></div>
    <div>Item 2 <br><strong>avec modifieur m-column</strong></div>
    <div>Item 3 <br><strong>avec modifieur m-column</strong></div>
</div>

<h2>m-column-reverse</h2>
<p>Pour <strong>flex-direction: column-reverse</strong></p>
<div class="c-flex m-column-reverse">
    <div>Item 1 <br><strong>avec modifieur m-column-reverse</strong></div>
    <div>Item 2 <br><strong>avec modifieur m-column-reverse</strong></div>
    <div>Item 3 <br><strong>avec modifieur m-column-reverse</strong></div>
</div>

<h2>m-row-reverse</h2>
<p>Pour <strong>flex-direction: row-reverse</strong></p>
<div class="c-flex m-row-reverse">
    <div>Item 1 <br><strong>avec modifieur m-row-reverse</strong></div>
    <div>Item 2 <br><strong>avec modifieur m-row-reverse</strong></div>
    <div>Item 3 <br><strong>avec modifieur m-row-reverse</strong></div>
</div>

<h2>Exemples responsive</h2>
<p>L'exemple suivant s'affiche en colonne sur la taille d'écran xs.</p>
<div class="c-flex" m-column="xs">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
</div>
<p>L'exemple suivant s'affiche en rangée inversée sur la taille d'écran xs.</p>
<div class="c-flex" m-row-reverse="xs">
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
{:.playground title="Modifieur m-nowrap"}


