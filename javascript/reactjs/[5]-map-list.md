# Map list

```jsx
function RenderList() {
    const numbers = [1, 2, 3, 4, 5];
    return (
        <div>
            <ul>
                {numbers.map((item, index) => (
                    <li key={index}>{item}</li>
                ))}
            </ul>
        </div>
    );


function App() {
    return (
        <div className="App">
            <RenderList />
        </div>
    );
}
```
