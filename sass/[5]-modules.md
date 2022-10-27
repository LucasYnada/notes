# Modules

```css
/* nome do arquivo: '_partials.css' */
/* não precisa citar a extensão */

@use "partials";
/*  para puxar uma variável: partials.$(nome) */
```

./\_partials.scss

```css
$color: #000;
```

./index.scss

```css
@use "partials";

body {
    color: partials.$color;
}
```
