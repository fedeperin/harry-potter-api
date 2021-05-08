# Harry Potter API

Es una API de Harry Potter en Español que devuelve información sobre hechizos, personajes, e información en sí.

## Cómo usar
```javascript
	fetch("https://fedeperin-harry-potter-api.herokuapp.com/db")
		.then((res) => res.json())
		.then((data) => {
			console.log(data)
			// Trae todos los datos de la API
		})
		.catch((e) => console.log(e));
```
## Endpoints
- /db trae todos los datos de la API
- /hechizos trae solo los hechizos
- /info trae solo la parte de información de la API
- /personajes solo trae los personajes en la API