# Nested interpolation

Definir uma const com os estilos

```js
const rotate = keyframes`
  from {
    transform: rotate(0deg);
  }

  to {
    transform: rotate(360deg);
  }
`;

const styles = css`
    display: inline-block;
    animation: ${rotate} 2s linear infinite;
    padding: 2rem 1rem;
    font-size: 1.2rem;
`;

const Rotate = styled.div`
    ${styles}
`;
```
