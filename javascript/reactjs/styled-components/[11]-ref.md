# Ref element

```js
const Input = styled.input``;
const inputRef = createRef();

<Input
    ref={inputRef}
    placeholder="Hover to focus!"
    onMouseEnter={() => {
        inputRef.current.focus();
    }}
/>;
```
