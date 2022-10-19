# ReactJS - Início

```html
<head>
    ...
    <script src="https://unpkg.com/react@18/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>

    <!-- Don't use this in production: -->
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
</head>
```

```html
<body>
    <div id="App"></div>

    <script type="text/babel">
        // Necessário declarar se estiver chamando pela CDN
        function MyApp() {
            return "Meu primeiro componente";
        }

        const app = document.getElementById("App");
        const root = ReactDOM.createRoot(app);
        root.render(<MyApp />);
    </script>
</body>
```

```js
const root = ReactDOM.createRoot(document.getElementById("App"));
root.render(<MyApp />);
```

```bash
npx create-react-app my-app
cd my-app
npm start
```
