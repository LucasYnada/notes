# Themes

```js
const Button = styled.button`
    font-size: 1em;
    margin: 1em;
    padding: 0.25em 1em;
    border-radius: 3px;
    background-color: transparent;

    /* Color the border and text with theme.main */
    color: ${(props) => props.theme.main};
    border: 2px solid ${(props) => props.theme.main};
`;

Button.defaultProps = {
    theme: {
        main: "palevioletred",
    },
};
```

Usando o ThemeProvider

```js
const theme = {
    main: "mediumseagreen",
};

<Button>Normal</Button>
<ThemeProvider theme={theme}>
    <Button>Themed</Button>
</ThemeProvider>
```

Pegando o tema sem componentes estilizados

```js
// Classes
import { withTheme } from "styled-components";

class MyComponent extends React.Component {
    render() {
        console.log("Current theme: ", this.props.theme);
        // ...
    }
}

export default withTheme(MyComponent);
```

```js
// useContext
import { useContext } from "react";
import { ThemeContext } from "styled-components";

const MyComponent = () => {
    const themeContext = useContext(ThemeContext);

    console.log("Current theme: ", themeContext);
    // ...
};
```

```js
// useTheme
import { useTheme } from "styled-components";

const MyComponent = () => {
    const theme = useTheme();

    console.log("Current theme: ", theme);
    // ...
};
```
