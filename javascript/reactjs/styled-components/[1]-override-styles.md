# Override styles & +

Sobrescrever estilos

```js
const Button = styled.button`
    background: ${(props) => (props.primary ? "palevioletred" : "white")};
    border-radius: 3px;
    border: 2px solid palevioletred;
    color: ${(props) => (props.primary ? "white" : "palevioletred")};
    margin: 0 1em;
    padding: 0.25em 1em;
    cursor: pointer;
    margin-left: 20px;
`;

const AuthButton = styled(Button)`
    color: tomato;
    border-color: tomato;
`;

// JSX
<AuthButton>Auth button</AuthButton>;
```

Passar uma função para o componente

```js
const ReversedButton = (props) => (
    <Button {...props} children={props.children.split("").reverse()} />
);
// Inverte o texto

<Button as={ReversedButton}>Button 1</Button>;
```
