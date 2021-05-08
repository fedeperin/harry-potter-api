# Harry Potter API

Es una API de Harry Potter en Español que devuelve información sobre hechizos, personajes, e información en sí.

## Cómo usar
Para usarlo solo copiá y pegá el siguiente código JavaScript en el JavaScript de tu web o aplicación
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
- /db Trae toda la API
- /hechizos Trae solo los hechizos almacenados en la API
- /info Trae solo la parte de información de la API
- /personajes Solo trae los personajes en la API
