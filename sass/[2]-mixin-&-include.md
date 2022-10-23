# Mixin & Include

```css
@mixin border-radius($radius) {
    border-radius: $radius;
}

.container {
    @include border-radius(20px);
}

/* .container {
  border-radius: 20px;
} */
```

```css
@mixin rounded($color: yellow, $radius: 10px) {
    /* por padrão, a cor é amarela e o radius 10px */
    border-radius: $radius;
    background-color: $color;
}

.container {
    @include rounded(blue, 5px);
    /* @include rounded(); */
}

/* .container {
  border-radius: 5px;
  background-color: blue;
} */
```
