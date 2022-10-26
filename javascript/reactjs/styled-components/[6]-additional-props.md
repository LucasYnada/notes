# Additional props

```js
const Input = styled.input.attrs((props) => ({
    type: "text",
    size: props.size || "1em",
    // atributo size
}))`
    color: palevioletred;
    font-size: 1em;
    border: 2px solid palevioletred;
    border-radius: 3px;

    margin: ${(props) => props.size};
    padding: ${(props) => props.size};
`;
```
