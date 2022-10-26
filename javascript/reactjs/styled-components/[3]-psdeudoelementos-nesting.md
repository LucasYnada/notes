# Pseudoelements, pseudoselectors, and nesting

```js
const Input = styled.input.attrs({ type: "checkbox" })``;

<Input />;
```

Com props

```js
const Input = styled.input.attrs((props) => ({ type: "checkbox" }))`
    height: ${(props) => (props.primary ? "25px" : "30px")};
    width: 25px;
`;

<Input primary />;
```

Aplicando estilos no seletor, nos atributos e nos filhos

```js
const Container = styled.div`
    width: 200px;
    height: 200px;

    background-color: #002930;

    &:hover {
        background-color: #1a191a;
    }

    .square-two {
        width: 80px;
        height: 80px;
        background-color: #fff;
    }
`;

<Container>
    <div className="square-two"></div>
</Container>;
```
