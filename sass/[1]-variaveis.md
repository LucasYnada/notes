# Variáveis

```css
$mainColor: #c0ffee;

header {
    background-color: $mainColor;
}
```

Demilitando escopo

```scss
.main {
    $width: 5em;
    width: $width;
}

.main {
    $height: 5em !global;
}
```

Interpolação de variáveis

```css
/* #{VARIAVEL}  */

$color: yellow;
$vert: top;

.background-#{$vert} {
    background-color: $color;
}

/* .background-top {
  background-color: yellow;
} */
```

```css
$roboto-font-path: "../fonts/roboto";

@font-face {
    src: url("#{$roboto-font-path}/Roboto-Thin.woff2") format("woff2");
    font-family: "Roboto";
}
```

```css
$logo-element: logo-bg;

.logo {
    background: element(##{$logo-element});
}
```
