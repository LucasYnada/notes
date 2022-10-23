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
