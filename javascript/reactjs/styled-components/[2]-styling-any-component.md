# Styling any component

```js
const Link = ({ className, children }) => (
    <a className={className} href="#">
        {children}
    </a>
);

const StyledLink = styled(Link)`
    color: palevioletred;
    font-weight: bold;
`;

// JSX
<StyledLink>Login</StyledLink>;
```

If com props

```js
const Input = styled.input`
    padding: 0.5em;
    margin: 0.5em;
    color: ${(props) => props.inputColor || "palevioletred"};
    background: papayawhip;
    border: none;
    border-radius: 3px;
`;

<Input inputColor="rebeccapurple" placeholder="Email" /> // com a cor rebeccapurple
<Input /> // normal
```

Criar o estilo do componente fora para não ser recriado cada vez

```js
const StyledWrapper = styled.div`
    /* ... */
`;

const Wrapper = ({ message }) => {
    return <StyledWrapper>{message}</StyledWrapper>;
};
```

https://styled-components.com/docs/basics
Pseudoelements, pseudoselectors, and nesting
