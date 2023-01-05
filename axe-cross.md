---
title: Axe cross
description: Modifieurs c-flex pour l'axe secondaire "cross"
layout: libdoc/page-split
order: 300
---
```html
<h2>m-cross-start</h2>
<p>Pour <strong>align-items: flex-start</strong></p>
<div class="c-flex">
    <div>Item 1</div>
    <div>Item 2<br> Avec une ligne en plus <br>pour visualiser l'effet</div>
</div>
<div class="c-flex m-cross-start">
    <div>Item 1</div>
    <div>Item 2<br> Avec une ligne en plus <br>pour visualiser l'effet</div>
</div>

<h2>m-cross-center</h2>
<p>Pour <strong>align-items: flex-center</strong></p>
<div class="c-flex m-cross-center">
    <div>Item 1</div>
    <div>Item 2<br> Avec une ligne en plus <br>pour visualiser l'effet</div>
</div>

<h2>m-cross-end</h2>
<p>Pour <strong>align-items: flex-end</strong></p>
<div class="c-flex m-cross-end">
    <div>Item 1</div>
    <div>Item 2<br> Avec une ligne en plus <br>pour visualiser l'effet</div>
</div>

<h2>m-cross-baseline</h2>
<p>Pour <strong>align-items: baseline</strong>, alignement sur le bas de la première ligne de texte.</p>
<div class="c-flex m-cross-baseline">
    <div><h1>Item 1</h1></div>
    <div><h3>Item 2</h3><br> Avec une ligne en plus <br>pour visualiser l'effet</div>
    <div><h6>Item 3</h6></div>
</div>

<!-- DEMO UNIQUEMENT -->
<style>
    body {
        padding: var(--ita-spacing-4);
        background-color: var(--ita-color-neutral-800);
        font-family: var(--ita-font-family-mono);
        font-size: 1rem;
        line-height: 1.5rem;
        padding-bottom: 50vh;
    }
    .c-flex {
        background-color: var(--ita-color-support-success-900);
    }
    .c-flex > * {
        background-color: var(--ita-color-support-success-700);
        border: var(--ita-border-7);
        padding: var(--ita-spacing-4);
    }
    .c-flex + .c-flex {
        margin-top: var(--ita-spacing-4);
    }
    .c-flex + h2 {
        margin-top: var(--ita-spacing-12);
    }
    /* Pour la démo baseline */
    .c-flex h1::after {
        content: '';
        position: absolute;
        display: block;
        width: 80vw;
        height: 1px;
        background-color: var(--ita-color-neutral-900);
    }
</style>
```
{:.playground title="Modifieurs pour l'axe cross"}


