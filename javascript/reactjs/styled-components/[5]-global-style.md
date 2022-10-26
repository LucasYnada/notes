# Global style

```js
import styled, { css, createGlobalStyle } from "styled-components";
```

```js
const GlobalStyle = createGlobalStyle`
        body {
        margin: 0;
        padding: 0;
        background: teal;
        font-family: Open-Sans, Helvetica, Sans-Serif;
        color: #fff;
        font-size: 24px;
    }
    `;

const Thing = styled.span`
    && {
        font-size: 14px;
    }

    // && atua como precedence boost, para evitar conflitos
`;

// JSX
<div>
    <GlobalStyle />
    // GlobalStyle Carrega os estilos globais
    <Thing>Jabari</Thing>
</div>;
```
