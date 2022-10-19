# Inline If with Logical && Operator

```js
const [isLoggedIn, setIsloggedIn] = useState(true);

<div>{isLoggedIn ? <h1>Hello, user!</h1> : <h1>Login Here</h1>}</div>;

// Ou

function GetUser() {
    if (isLoggedIn) {
        return <h1>Hello, user!</h1>;
    } else {
        return (
            <h1>
                <a href="#">Login Here</a>
            </h1>
        );
    }
}

<div>
    <GetUser />
</div>;
```
