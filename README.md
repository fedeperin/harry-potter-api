# Harry Potter API
> [!IMPORTANT]  
> [PotterAPI](https://github.com/fedeperin/potterapi) es una nueva versión de esta API, disponible en varios idiomas, actualizada y hecha con Express.js, recomiendo usar esa en vez de esta.

Una API Rest sobre Harry Potter en Español que retorna información sobre hechizos, personajes, libros e información en sí. Usé Node.js con json-server como su única dependencia para crearla y la alojé en Render. <br><br>

* Repositorio de json-server: https://github.com/typicode/json-server <br>
* Instalar Node.js: https://nodejs.org/ <br>
* Página web de Render: https://render.com/ <br><br>

Si la querés instalar, ejecutá ``npm i json-server`` para instalar json-server en el proyecto
## Cómo incorporar
Para usarla, solo copiá y pegá el siguiente código JavaScript en el código de tu web o aplicación que utilize ese lenguaje. Eso retornará los datos almacenados el el endpoint "db" y los almacenará dentro de la variable data. Para cambiar el endpoint, solo cambiar el valor de ``url`` por otro endpoint de la API. <br>
```javascript
const url = "https://harry-potter-api.onrender.com/db"

fetch(url)
	.then((res) => res.json())
	.then((data) => {
		/*
			Trae toda la info de la API y la deja dentro de la variable data
			También muestra la variable data por consola
		*/
		console.log(data)
	})
	.catch((e) => console.log(e))
```
O visitá la página principal de la API (que viene por defecto con json-server): https://harry-potter-api.onrender.com/ <br>

## Endpoints
- https://harry-potter-api.onrender.com/db Trae toda la API
- https://harry-potter-api.onrender.com/hechizos Trae solo los hechizos almacenados en la API
- https://harry-potter-api.onrender.com/info Trae solo la parte de información de la API
- https://harry-potter-api.onrender.com/personajes Solo trae los personajes en la API
- https://harry-potter-api.onrender.com/libros Trae solo la información sobre libros en la API <br>
--- 
Si se quiere acceder a un elemento específico, solo hay que especificar el ID de ese elemento al final de la ruta<br>
#### Ejemplos: 
- Con la ruta https://harry-potter-api.onrender.com/libros/3 se accede solo al libro con ID 3 (el especificado al final de la ruta).<br>
- Con la ruta https://harry-potter-api.onrender.com/hechizos/10 se accede solo al hechizo con ID 10 (el especificado al final de la ruta).

---
Versión de la API en Inglés: https://github.com/fedeperin/harry-potter-api-english/
