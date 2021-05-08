# Harry Potter API

Es una API de Harry Potter en Español que devuelve información sobre hechizos, personajes, e información en sí.

## Cómo usar
Para usarlo solo copiá y pegá el siguiente código JavaScript en el JavaScript de tu web
```javascript
fetch("https://fedeperin-harry-potter-api.herokuapp.com/db")
	.then((res) => res.json())
	.then((data) => {
		// Trae todos los datos de la API y los muestra por consola
		console.log(data)
	})
	.catch((e) => console.log(e));
```
## Endpoints
- /db trae todos los datos de la API
- /hechizos trae solo los hechizos
- /info trae solo la parte de información de la API
- /personajes solo trae los personajes en la API
