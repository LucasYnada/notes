# Forms

Textos: pegando o valor de um input

```jsx
const [value, setValue] = useState();

function handleSubmit(e) {
    e.preventDefault();
    alert(value);
}

<form onSubmit={handleSubmit}>
    <input type="text" row="5" onChange={(e) => setValue(e.target.value)} />
    <input type="submit" value="Submit" />
</form>;
```

Select: alterando valor do select com setValue

```jsx
const [value, setValue] = useState("coconut");
// padrão coconut

function handleChange(e) {
    setValue(e.target.value);
}

function handleSubmit(e) {
    e.preventDefault();
    alert(value);
}

<form onSubmit={handleSubmit}>
    <label>
        Pick your favorite flavor:
        <select value={value} onChange={(e) => handleChange(e)}>
            <option value="grapefruit">Grapefruit</option>
            <option value="lime">Lime</option>
            <option value="coconut">Coconut</option>
            <option value="mango">Mango</option>
        </select>
    </label>
    <input type="submit" value="Submit" />
</form>;
```

Arquivos: enviando múltiplos arquivos do tipo "image"

```jsx
function handleChangeImage(e) {
    alert(`Selected file - ${e.target.files[0].name}`); // nome do primeiro arquivo (file[0])

    // e.target.files => retorna um array com os arquivos enviados
}

<input
    type="file"
    multiple
    accept="image/*"
    onChange={(e) => handleChangeImage(e)}
/>;
```
