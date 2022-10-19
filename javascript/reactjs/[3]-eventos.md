# Handling Events

```js
function activateLasers() {
    alert("Button alert (:");
}

// activateLasers() é chamado instantaneamente
<button onClick={activateLasers()}>Activate Lasers</button>;

// activateLasers() é chamando apenas quando o botão for pressionado
<button onClick={() => activateLasers()}>Activate Lasers</button>;
```

Input (prevenir que a página reinicie)

```js
function handleSubmit(e) {
    e.preventDefault();
    console.log("You clicked submit.");
}

<form onSubmit={handleSubmit}>
    <button type="submit">Submit</button>
</form>;
```
