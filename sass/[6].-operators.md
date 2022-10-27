# Operators

```
+, -, *, math.div() e %
```

```css
@use "sass:math";

article[role="main"] {
    width: math.div(600px, 960px) * 100%;
}

aside[role="complementary"] {
    width: math.div(300px, 960px) * 100%;
    margin-left: auto;
}
```
