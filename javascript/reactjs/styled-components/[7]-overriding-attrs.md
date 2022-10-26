# Overriding .attrs

```js
const Input = styled.input.attrs((props) => ({
    type: "text",
    size: props.size || "1em",
}))`
    border: 2px solid palevioletred;
    margin: ${(props) => props.size};
    padding: ${(props) => props.size};
`;

// Input's attrs will be applied first, and then this attrs obj
const PasswordInput = styled(Input).attrs({
    type: "password",
})`
    // similarly, border will override Input's border
    border: 2px solid aqua;
`;
```
