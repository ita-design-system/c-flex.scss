---
title: Inline
description: Modifieurs inline pour c-flex
layout: libdoc/page-split
order: 150
---
```html
<div class="c-flex">c-flex<br> Je suis un c-flex standard</div>
<div class="c-flex">c-flex<br> Je suis un autre c-flex standard</div>
<div class="c-flex m-inline-flex">c-flex m-inline-flex<br> Je suis un c-flex inline</div>
<div class="c-flex m-inline-flex">c-flex m-inline-flex<br> Je suis un autre c-flex inline</div>
<!-- DEMO UNIQUEMENT -->
<style>
    body {
        padding: var(--ita-spacing-4);
        background-color: var(--ita-color-primary-900);
        color: var(--ita-color-primary-200);
        font-family: var(--ita-font-family-mono);
        font-size: 1rem;
        line-height: 1.5rem;
        min-height: 100vh;
    }
    .c-flex {
        background-color: var(--ita-color-primary-500);
        color: var(--ita-color-neutral-900);
        padding: var(--ita-spacing-4);
    }
    .c-flex + .c-flex {
        margin-top: var(--ita-spacing-4);
    }
</style>
```
{:.playground title="Modifieurs inline-flex"}


