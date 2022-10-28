# Styled object

```js
const Input = styled.input({
    background: "palevioletred",
    padding: "10px 20px",
    margin: "10px",
    cursor: "pointer",
    border: "none",
});

const Button = styled.button((props) => ({
    background: props.primary,
    color: "white",
    padding: "10px 20px",
    margin: "10px",
    cursor: "pointer",
    border: "none",
}));

<Input placeholder="Hover to focus!" />
<Button primary={"#000"}>Button</Button>
```
