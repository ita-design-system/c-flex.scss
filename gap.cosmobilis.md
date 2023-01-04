---
title: Gap
description: Collection de gap spécifiques au projet Cosmobilis
layout: libdoc/page-split
---
```html
<!-- Feuille de style complémentaire c-flex pour le projet Cosmobilis -->
<link rel="stylesheet" href="{{'css/c-flex.cosmobilis.css'|absolute_url}}">
<div class="c-flex m-gap-1">
    <div>item un</div>
    <div>item deux</div>
    <div>item trois</div>
    <div>item quatre</div>
</div>
<div class="c-flex m-gap-2">
    <div>item un</div>
    <div>item deux</div>
    <div>item trois</div>
    <div>item quatre</div>
</div>
<div class="c-flex m-gap-3">
    <div>item un</div>
    <div>item deux</div>
    <div>item trois</div>
    <div>item quatre</div>
</div>
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
{:.playground title="Gap Cosmobilis"}


