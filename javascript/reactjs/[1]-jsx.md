# ReactJS - JSX

```jsx
const name = "Josh Perez";
const element = <h1>Hello, {name}</h1>;

const CallElement = () => {
    return <h1> Hello {name} </h1>;
};

<CallElement />;
```

```jsx
// camelCase (className, tabIndex)
<input tabIndex="1" className="input-login" defaultValue="" />
```

```jsx
//  JSX Prevents Injection Attacks XSS (cross-site-scripting)
const title = response.potentiallyMaliciousInput;
```
