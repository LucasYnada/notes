# ReactJS - Componentes & props

```js
function Header(name) {
    return <h1>Hello, {name}</h1>;
}

function App() {
    return (
        <div>
            <Header name="Sara" />
        </div>
    );
}
```

```js
const user = {
    date: new Date(),
    text: "I hope you enjoy learning React!",
    author: {
        name: "Hello Kitty",
        avatarUrl: "http://placekitten.com/g/64/64",
    },
};

function ImageComponent(props) {
    return (
        <div>
            <img className="Avatar" src={props.src} alt={props.alt} />
        </div>
    );
}

function App() {
    return (
        <div>
            <ImageComponent
                src={user.author.avatarUrl}
                alt={user.author.name}
            />
        </div>
    );
}
```
