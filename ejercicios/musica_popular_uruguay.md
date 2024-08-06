# Música Popular Uruguaya en TypeScript

## Introducción

En este ejercicio, crearemos un programa en TypeScript que gestione información sobre la música popular uruguaya.

## Requisitos previos

1. Tener instalado Visual Studio Code
2. Tener instalada la extensión de GitHub Copilot en VS Code
3. Tener conocimientos básicos de TypeScript

## Paso 1: Configurar el entorno

Primero, abre Visual Studio Code y crea un nuevo archivo llamado `musica_uruguaya.ts`.

## Paso 2: Comenzar con el código

Empecemos escribiendo un comentario para describir nuestro programa:

```typescript
// Programa para gestionar información sobre artistas y canciones de música popular uruguaya
```

GitHub Copilot comenzará a sugerir código basado en este comentario. Vamos a crear una clase para representar un artista de música:

```typescript
class Artista {
    nombre: string;
    genero: string;
    canciones: string[];

    constructor(nombre: string, genero: string) {
        this.nombre = nombre;
        this.genero = genero;
        this.canciones = [];
    }

    agregarCancion(cancion: string) {
        this.canciones.push(cancion);
        console.log(`Canción "${cancion}" agregada a ${this.nombre}`);
    }
}
```

## Paso 3: Agregar métodos a la clase

Ahora, agreguemos algunos métodos a nuestra clase. Escribe el siguiente comentario:

```typescript
// Método para listar todas las canciones del artista
```

GitHub Copilot sugerirá un método como este:

```typescript
listarCanciones() {
    console.log(`Canciones de ${this.nombre}:`);
    this.canciones.forEach((cancion, index) => {
        console.log(`${index + 1}. ${cancion}`);
    });
}
```

## Paso 4: Crear una lista de artistas

Vamos a crear una lista de artistas uruguayos. Escribe el siguiente comentario:

```typescript
// Lista de artistas uruguayos famosos
```

GitHub Copilot probablemente sugerirá algo como esto:

```typescript
let artistas: Artista[] = [
    new Artista("Jorge Drexler", "Canto popular"),
    new Artista("El Cuarteto de Nos", "Rock"),
    new Artista("No Te Va Gustar", "Rock"),
    new Artista("La Vela Puerca", "Rock")
];
```

## Paso 5: Crear una función para agregar canciones a los artistas

Ahora, vamos a crear una función que agregue canciones a los artistas. Escribe el siguiente comentario:

```typescript
// Función para agregar canciones a los artistas
```

GitHub Copilot podría sugerir algo como esto:

```typescript
function agregarCanciones() {
    artistas[0].agregarCancion("Al otro lado del río");
    artistas[1].agregarCancion("Yendo a la casa de Damián");
    artistas[2].agregarCancion("A las nueve");
    artistas[3].agregarCancion("El viejo");
}
```

## Paso 6: Ejecutar el programa

Finalmente, agreguemos el código para ejecutar nuestro programa:

```typescript
agregarCanciones();
artistas.forEach(artista => artista.listarCanciones());
```

## Código completo

Aquí está el código completo del programa:

```typescript
// Programa para gestionar información sobre artistas y canciones de música popular uruguaya

class Artista {
    nombre: string;
    genero: string;
    canciones: string[];

    constructor(nombre: string, genero: string) {
        this.nombre = nombre;
        this.genero = genero;
        this.canciones = [];
    }

    agregarCancion(cancion: string) {
        this.canciones.push(cancion);
        console.log(`Canción "${cancion}" agregada a ${this.nombre}`);
    }

    listarCanciones() {
        console.log(`Canciones de ${this.nombre}:`);
        this.canciones.forEach((cancion, index) => {
            console.log(`${index + 1}. ${cancion}`);
        });
    }
}

// Lista de artistas uruguayos famosos
let artistas: Artista[] = [
    new Artista("Jorge Drexler", "Canto popular"),
    new Artista("El Cuarteto de Nos", "Rock"),
    new Artista("No Te Va Gustar", "Rock"),
    new Artista("La Vela Puerca", "Rock")
];

// Función para agregar canciones a los artistas
function agregarCanciones() {
    artistas[0].agregarCancion("Al otro lado del río");
    artistas[1].agregarCancion("Yendo a la casa de Damián");
    artistas[2].agregarCancion("A las nueve");
    artistas[3].agregarCancion("El viejo");
}

agregarCanciones();
artistas.forEach(artista => artista.listarCanciones());
```

## Conclusión

En este tutorial, hemos visto cómo usar GitHub Copilot para crear rápidamente un programa en TypeScript relacionado con la música popular uruguaya. GitHub Copilot nos ayudó a escribir clases, métodos y funciones basándose en nuestros comentarios y contexto.
