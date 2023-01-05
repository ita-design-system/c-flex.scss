---
title: Axe main
description: Modifieurs c-flex pour l'axe principal "main"
layout: libdoc/page-split
order: 200
---
```html
<h2>m-main-start</h2>
<p>Pour <strong>justify-content: flex-start</strong>, valeur par défaut qui a le même effet que c-flex seul</p>
<div class="c-flex">
    <div>Item 1</div>
    <div>Item 2</div>
</div>
<div class="c-flex m-main-start">
    <div>Item 1</div>
    <div>Item 2</div>
</div>

<h2>m-main-center</h2>
<p>Pour <strong>justify-content: flex-center</strong></p>
<div class="c-flex m-main-center">
    <div>Item 1</div>
    <div>Item 2</div>
</div>

<h2>m-main-end</h2>
<p>Pour <strong>justify-content: flex-end</strong></p>
<div class="c-flex m-main-end">
    <div>Item 1</div>
    <div>Item 2</div>
</div>

<h2>m-main-space-between</h2>
<p>Pour <strong>justify-content: space-between</strong></p>
<div class="c-flex m-main-space-between">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
</div>

<h2>m-main-space-around</h2>
<p>Pour <strong>justify-content: space-around</strong></p>
<div class="c-flex m-main-space-around">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
</div>

<h2>m-main-space-evenly</h2>
<p>Pour <strong>justify-content: space-evenly</strong></p>
<div class="c-flex m-main-space-evenly">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
</div>
<!-- DEMO UNIQUEMENT -->
<style>
    body {
        padding: var(--ita-spacing-4);
        background-color: var(--ita-color-neutral-800);
        font-family: var(--ita-font-family-mono);
        font-size: 1rem;
        line-height: 1.5rem;
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
</style>
```
{:.playground title="Modifieurs pour l'axe main"}


