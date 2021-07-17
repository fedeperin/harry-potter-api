# Harry Potter API

Una API Rest sobre Harry Potter en Español que retorna información sobre hechizos, personajes, libros e información sobre la saga. Utilizé Node js con json-server como única dependencia para crearla y la alojé en Heroku <br><br>

* Repositorio en GitHub de json-server: https://github.com/typicode/json-server <br>
* Descargar Node js: https://nodejs.org/ <br>
* Página web del hosting que utilizé: https://heroku.com/ <br>

Si querés descargarlo, ejecutá por tu terminal con node.js instalado  ``npm i json-server`` para instalar json-server

## Cómo incorporar
Para usarla, solo copiá y pegá el siguiente código JavaScript en el código de tu web o aplicación. Eso retornará los datos almacenados el el endpoint "db". Para cambiar el endpoint, solo cambiar el valor de ``url`` por otro endpoint. <br>
```javascript
const url = "https://fedeperin-harry-potter-api.herokuapp.com/db"

fetch(url)
	.then((res) => res.json())
	.then((data) => {
		// Trae todos los datos de la API y los muestra por la consola
		console.log(data)
	})
	.catch((e) => console.log(e));
```
O visitá la página principal de la API (que viene por defecto con json-server): https://fedeperin-harry-potter-api.herokuapp.com/
## Endpoints
- https://fedeperin-harry-potter-api.herokuapp.com/db Trae toda la API
- https://fedeperin-harry-potter-api.herokuapp.com/hechizos Trae solo los hechizos almacenados en la API
- https://fedeperin-harry-potter-api.herokuapp.com/info Trae solo la parte de información de la API
- https://fedeperin-harry-potter-api.herokuapp.com/personajes Solo trae los personajes en la API
- https://fedeperin-harry-potter-api.herokuapp.com/libros Trae solo la información sobre libros en la API <br>
--- 
Si se quiere acceder a un elemento específico, solo hay que especificar el ID de ese elemento al final de la ruta<br>
#### Ejemplos: 
- Con la ruta https://fedeperin-harry-potter-api.herokuapp.com/libros/3 se accede solo al libro con id 3 (el especificado al final de la ruta).<br>
- Con la ruta https://fedeperin-harry-potter-api.herokuapp.com/hechizos/10 se accede solo al hechizo con id 10 (el especificado al final de la ruta.

---
Repositorio de la versión de esta API en Inglés: https://github.com/fedeperin/harry-potter-api-english/
