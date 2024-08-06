# Uso de GitHub Copilot para desarrollar un programa de fútbol Uruguayo en Python

## Introducción

Este tutorial te guiará en el uso de GitHub Copilot para desarrollar un programa en Python que gestione información sobre equipos de fútbol uruguayos. 

## Requisitos Previos

1. Visual Studio Code (VS Code) instalado.
2. Extensión de GitHub Copilot instalada en VS Code.
3. Conocimientos básicos de Python.

## Paso 1: Configuración del Entorno

1. Abre Visual Studio Code.
2. Crea un nuevo archivo y nómbralo `futbol_uruguayo.py`.

## Paso 2: Inicio del Código

Comienza agregando un comentario que describa el propósito del programa:

```python
# Programa para gestionar información sobre equipos de fútbol uruguayos
```

GitHub Copilot generará sugerencias basadas en este comentario. Ahora, define una clase para representar a un equipo de fútbol:

```python
class EquipoUruguayo:
    def __init__(self, nombre, ciudad, fundacion):
        self.nombre = nombre
        self.ciudad = ciudad
        self.fundacion = fundacion
        self.titulos = 0
```

## Paso 3: Adición de Métodos a la Clase

Para añadir métodos a la clase, escribe el siguiente comentario:

```python
# Método para agregar títulos al equipo
```

GitHub Copilot sugerirá un método similar al siguiente:

```python
def agregar_titulo(self):
    self.titulos += 1
    print(f"{self.nombre} ha ganado un nuevo título. Total de títulos: {self.titulos}")
```

## Paso 4: Creación de una Lista de Equipos

A continuación, crea una lista de equipos uruguayos. Agrega el siguiente comentario:

```python
# Lista de equipos uruguayos destacados
```

GitHub Copilot debería sugerir una lista como esta:

```python
equipos_uruguayos = [
    EquipoUruguayo("Peñarol", "Montevideo", 1891),
    EquipoUruguayo("Nacional", "Montevideo", 1899),
    EquipoUruguayo("Defensor Sporting", "Montevideo", 1913),
    EquipoUruguayo("Danubio", "Montevideo", 1932)
]
```

## Paso 5: Implementación de una Función para Simular un Torneo

Para simular un torneo entre los equipos, utiliza el siguiente comentario:

```python
# Función para simular un torneo entre los equipos
```

GitHub Copilot podría sugerir una función como la siguiente:

```python
import random

def simular_torneo(equipos):
    print("¡Comienza el torneo uruguayo!")
    for _ in range(5):  # Simulamos 5 rondas
        ganador = random.choice(equipos)
        ganador.agregar_titulo()
    
    print("\nResultados finales:")
    for equipo in equipos:
        print(f"{equipo.nombre}: {equipo.titulos} títulos")
```

## Paso 6: Ejecución del Programa

Finalmente, agrega el siguiente código para ejecutar el programa:

```python
if __name__ == "__main__":
    simular_torneo(equipos_uruguayos)
```

## Conclusión

En este tutorial, hemos aprendido a usar GitHub Copilot para desarrollar un programa en Python que gestiona información sobre equipos de fútbol uruguayos. GitHub Copilot nos asistió en la escritura de clases, métodos y funciones basándose en nuestros comentarios y el contexto del código.
Es importante recordar que, aunque GitHub Copilot es una herramienta poderosa, siempre debes revisar y comprender el código generado antes de integrarlo en tus proyectos.

