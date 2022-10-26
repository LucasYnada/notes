# Início

Instalar

```bash
npm i styled-components --save
```

Importar

```js
import styled, { css } from "styled-components";
```

Estilizando um componente

```js
const componente = styled.elemento`
    // css
`;

const Button = styled.button`
    background: palevioletred;
    color: white;
    ...
`;

// no JSX
<Button>Botão 1</Button>;
```

Usando props

```jsx
const Button = styled.button`
    background: ${(props) => (props.primary ? "palevioletred" : "white")};
    color: ${(props) => (props.primary ? "white" : "palevioletred")};
    ...
`;

// ou

const Button = styled.button`
    ...
${(props) =>
    props.primary &&
    css`
        background-color: #000;
        color: red;
    `}
`;

// no JSX
<Button>Button 1</Button>
<Button primary>Button 2</Button>
```
