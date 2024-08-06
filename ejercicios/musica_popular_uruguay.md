### Programa de Gestión de Música Popular Uruguaya con JavaScript y GitHub Copilot

## Introducción

En este ejercicio, crearemos un programa en JavaScript que gestione información sobre la música popular uruguaya, utilizando GitHub Copilot para ayudarnos en el proceso de codificación.

## Requisitos previos

1. Tener instalado Visual Studio Code
2. Tener instalada la extensión de GitHub Copilot en VS Code
3. Tener conocimientos básicos de JavaScript

## Paso 1: Configurar el entorno

Abre Visual Studio Code y crea un nuevo archivo llamado `musica_uruguaya.js`.

## Paso 2: Comenzar con el código

Empecemos escribiendo un comentario para describir nuestro programa. Este comentario servirá como prompt para GitHub Copilot:

```javascript
// Programa para gestionar información sobre artistas y canciones de música popular uruguaya
```

GitHub Copilot comenzará a sugerir código basado en este comentario. Vamos a crear una clase para representar un artista de música:

```javascript
// Crear una clase Artista con propiedades nombre, genero y canciones
```

GitHub Copilot probablemente sugerirá algo como esto:

```javascript
class Artista {
    constructor(nombre, genero) {
        this.nombre = nombre;
        this.genero = genero;
        this.canciones = [];
    }
}
```

## Paso 3: Agregar métodos a la clase

Ahora, agreguemos algunos métodos a nuestra clase. Escribe los siguientes comentarios como prompts para GitHub Copilot:

```javascript
// Método para agregar una canción al artista
// Método para listar todas las canciones del artista
```

GitHub Copilot sugerirá métodos como estos:

```javascript
agregarCancion(cancion) {
    this.canciones.push(cancion);
    console.log(`Canción "${cancion}" agregada a ${this.nombre}`);
}

listarCanciones() {
    console.log(`Canciones de ${this.nombre}:`);
    this.canciones.forEach((cancion, index) => {
        console.log(`${index + 1}. ${cancion}`);
    });
}
```

## Paso 4: Crear una lista de artistas

Vamos a crear una lista de artistas uruguayos. Escribe el siguiente comentario como prompt:

```javascript
// Crear una lista de artistas uruguayos famosos
```

GitHub Copilot probablemente sugerirá algo como esto:

```javascript
let artistas = [
    new Artista("Jorge Drexler", "Canto popular"),
    new Artista("El Cuarteto de Nos", "Rock"),
    new Artista("No Te Va Gustar", "Rock"),
    new Artista("La Vela Puerca", "Rock")
];
```

## Paso 5: Crear una función para agregar canciones a los artistas

Ahora, vamos a crear una función que agregue canciones a los artistas. Usa este prompt:

```javascript
// Función para agregar canciones a los artistas
```

GitHub Copilot podría sugerir algo como esto:

```javascript
function agregarCanciones() {
    artistas[0].agregarCancion("Al otro lado del río");
    artistas[1].agregarCancion("Yendo a la casa de Damián");
    artistas[2].agregarCancion("A las nueve");
    artistas[3].agregarCancion("El viejo");
}
```

## Paso 6: Ejecutar el programa

Finalmente, agreguemos el código para ejecutar nuestro programa. Usa este prompt:

```javascript
// Ejecutar el programa: agregar canciones y listar canciones de cada artista
```

GitHub Copilot sugerirá algo como:

```javascript
agregarCanciones();
artistas.forEach(artista => artista.listarCanciones());
```

