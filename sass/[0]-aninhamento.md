# Aninhamento de regras

```css
nav {
    ul {
        list-style: none;
    }

    li {
        display: inline-block;
    }

    a {
        text-decoration: none;
    }
}
```

```css
.selector {
    & {
    }

    &:hover {
        /* repetindo o seletor */
        /* .selector:hover {} */
    }
}
```
