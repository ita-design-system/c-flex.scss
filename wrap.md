---
title: Wrap
description: Modifieurs relatifs au retour à la ligne et à l'ordre d'affichage
layout: libdoc/page-split
order: 400
---
```html
<h2>m-nowrap</h2>
<p>Par défaut, le retour à la ligne est activé sur le composant c-flex. Il est possible de le désactiver avec le modifieur m-nowrap, pour <strong>flex-wrap: nowrap</strong></p>
<div class="c-flex">
    <div>Item 1 dans un conteneur c-flex <strong>sans modifieur m-nowrap</strong></div>
    <div>Item 2 dans un conteneur c-flex <strong>sans modifieur m-nowrap</strong></div>
    <div>Item 3 dans un conteneur c-flex <strong>sans modifieur m-nowrap</strong></div>
</div>
<div class="c-flex m-nowrap">
    <div>Item 1 dans un conteneur c-flex <strong>avec modifieur m-nowrap</strong></div>
    <div>Item 2 dans un conteneur c-flex <strong>avec modifieur m-nowrap</strong></div>
    <div>Item 3 dans un conteneur c-flex <strong>avec modifieur m-nowrap</strong></div>
</div>

<h2>m-wrap-reverse</h2>
<p>Pour <strong>flex-wrap: wrap-reverse</strong></p>
<div class="c-flex">
    <div>Item dans un conteneur c-flex par défaut</div>
    <div>Item 2</div>
    <div>Item 3</div>
    <div>Item 4</div>
</div>
<div class="c-flex m-wrap-reverse">
    <div>Item dans un conteneur c-flex <strong>m-wrap-reverse</strong></div>
    <div>Item 2</div>
    <div>Item 3</div>
    <div>Item 4</div>
</div>

<h2>Exemples responsive</h2>
<div class="c-flex m-nowrap--xs">
    <div>Je passe en nowrap en taille d'écran xs</div>
    <div>Item 1 dans un conteneur c-flex <strong>avec modifieur classe CSS</strong></div>
    <div>Item 2 dans un conteneur c-flex <strong>avec modifieur classe CSS</strong></div>
    <div>Item 3 dans un conteneur c-flex <strong>avec modifieur classe CSS</strong></div>
</div>
<div class="c-flex" m-nowrap="xs,sm">
    <div>Je passe en nowrap en taille d'écran xs et sm</div>
    <div>Item 1 dans un conteneur c-flex <strong>avec attribut responsive</strong></div>
    <div>Item 2 dans un conteneur c-flex <strong>avec attribut responsive</strong></div>
    <div>Item 3 dans un conteneur c-flex <strong>avec attribut responsive</strong></div>
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


