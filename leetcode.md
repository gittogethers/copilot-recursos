# Empezando - Resolviendo un rompecabezas de algoritmo - Visual Studio Code

¡Bienvenido a GitHub Copilot! ¿Cuál será la mejor manera de ver el poder de Copilot? Comencemos resolviendo un rompecabezas de algoritmo. Como cualquier estudiante de ciencias de la computación que busca trabajo, se te pedirá que resuelvas rompecabezas de algoritmos durante las entrevistas de trabajo en lugares como Google, Microsoft, Amazon y Facebook. Para prepararse para esto, muchos estudiantes universitarios utilizan sitios de preparación de código como **LeetCode** y **HackerRank** para practicar la resolución de rompecabezas de algoritmos.

Probablemente no sea demasiado sorprendente, pero GitHub Copilot es muy bueno resolviendo rompecabezas de algoritmos. En esta demostración, utilizaremos un ejemplo de rompecabezas encontrado en [LeetCode](https://leetcode.com/) para ver cómo GitHub Copilot puede resolver fácilmente rompecabezas de algoritmos.

> DESCARGO DE RESPONSABILIDAD: Esta demostración está destinada únicamente a mostrar el poder de GitHub Copilot. No está destinada a mostrar cómo hacer trampa en tu entrevista de trabajo de codificación o obtener rangos más altos en LeetCode o HackerRank. Por favor, usa esta demostración de manera responsable.

Aunque puedes usar cualquier editor compatible con Copilot como Visual Studio Code, Visual Studio IDE, NeoVim e IntelliJ, usaremos Visual Studio Code para esta demostración.

## Prerrequisitos

- [Extensión de Copilot para Visual Studio Code](https://code.visualstudio.com/download)
- [Java SDK para ejecutar tu código](https://www.oracle.com/java/technologies/javase-downloads.html)

## Pasos

¡Bienvenido! En esta demostración inicial de Copilot para **Empezando - Resolviendo un rompecabezas de algoritmo - Visual Studio Code**, resolveremos el siguiente problema de Leetcode llamado [Reverse Integer](https://leetcode.com/problems/reverse-integer/). Este es un problema de rango medio en LeetCode donde la tasa de aceptación es de aproximadamente `27.6%`.

![LeetCode - Reverse Integer](./images/1_LeetCodeProblem.jpg)

### Paso 1: Abre Visual Studio Code y crea un nuevo archivo Java

Abre Visual Studio Code y crea o navega a un directorio donde quieras crear un nuevo archivo Java. Asegúrate de que tu GitHub Copilot esté habilitado y activado. En esta demostración, crearemos un nuevo archivo Java llamado `Puzzle.java`.

Haz clic derecho en el directorio y selecciona **Nuevo archivo**.

![Crear un nuevo archivo](./images/2_OpenVSCode.jpg)

Luego, dale un nombre. Lo llamaré `Puzzle.java`.

![Archivo nombrado](./images/3_CreateFile.jpg)

Tu Visual Studio Code debería verse así. Ahora estamos listos para escribir algo de código a través de GitHub Copilot.

![Panel general](./images/4_Overview.jpg)

### Paso 2: Comienza a escribir código a través de GitHub Copilot

Comencemos a escribir código. Empezaremos con una clase Java simple.

```java
public class Puzzle {
    
}
```

Dependiendo de si usaste Copilot, es posible que Copilot te esté sugiriendo cosas diferentes al vuelo. Puedes seguir escribiendo para ignorar lo que Copilot sugiere. Recuerda. Tú eres el piloto principal, y GitHub Copilot es solo una asistencia.

![Agregar clase](./images/5_AddClass.jpg)

Agreguemos una función a continuación. GitHub Copilot puede sugerir basándose en algunas cosas:

- Comentarios que escribes encima de la clase, la línea, función, etc.
- Contexto general de lo que escribiste
- Lo que escribiste anteriormente en el historial
- Nombres de archivos, funciones, etc.

Nombraremos esta función `reverse` que devuelve `int` pero también acepta `int`.

```java
public int reverse(int x) {

}
```

De nuevo, GitHub Copilot te sugerirá lo que escribas. Puedes seguir escribiendo para ignorar lo que Copilot sugiere.

![Agregar función](./images/6_CreateFunction.jpg)

Después de que hayas escrito, te sugerirá códigos como este. Tu resultado puede verse diferente, y lo que realmente queremos no importa.

![Función recomendada](./images/7_SuggestionFunctionReverse.jpg)

Observa que tu icono de Copilot en la esquina inferior derecha gira mientras GitHub Copilot está pensando.

![Copilot pensando](./images/8_CopilotThinking.jpg)

También puedes seleccionar **Salida** en la parte inferior si tienes **Terminal** abierto, y cambiar el menú desplegable a **GitHub Copilot**.

![Salida de Copilot](./images/8_1_CopilotOutput.jpg)

Y se verá así. Puedes ver lo que se genera mientras escribes.

![Copilot pensando](./images/8_2_CopilotPrint.jpg)

Intenta aceptar la solución ahora, y trata de agregar la función principal así. Puedes simplemente comenzar a escribir lo siguiente para que pueda generar el resultado.

```java
public static void main(String[] args) {
    
}
```

![Agregar función principal](./images/9_MainFunction.jpg)

### Paso 3: Ejecutemos y veamos qué sucede

A continuación, probaremos nuestro código. Abre una nueva **Terminal** yendo al menú **Terminal** y seleccionando **Nueva Terminal**.

![Abrir terminal](./images/10_OpenTerminal.jpg)

Luego, tendrás una nueva terminal abierta. Asegúrate de haber instalado un Java SDK como prerrequisito. Puedes verificarlo escribiendo `java -version` en la terminal.

![Terminal abierta](./images/11_TerminalOpened.jpg)

Luego, puedes compilar tu código primero con `javac Puzzle.java` y ejecutarlo con `java Puzzle`. Deberías ver el siguiente resultado.

![Ejecutar el código](./images/12_Output.jpg)

¡Eso es genial! Pero puede que no sea exactamente el resultado que estamos buscando. Intentemos agregar un comentario que se proporcionó desde Leetcode para hacerlo más preciso.

### Paso 4: Corrige el resultado proporcionando un comentario

GitHub Copilot también puede detectar los cambios y sugerirte con nuevo contexto. Ahora, hay un campo llamado **Ingeniería de Prompts**. Para obtener el mejor resultado, realmente necesitas pensar en qué tipo de cosas preguntarle a Copilot y juzgar por ti mismo si está bien o mal. En este caso, agregaremos un comentario que se proporcionó desde Leetcode.

> Dado un entero de 32 bits con signo x, devuelve x con sus dígitos invertidos. Si invertir x hace que el valor salga del rango de enteros de 32 bits con signo [-231, 231 - 1], entonces devuelve 0.

Luego, lo agregaremos como un comentario de función así. Elimina todo dentro de la función.

![Agregar comentario](./images/13_AddComment.jpg)

Entonces, verás que GitHub Copilot te sugerirá una nueva función. Puedes aceptarla.

Tan pronto como hagas una nueva línea, verás que GitHub Copilot está generando un nuevo resultado. Tus códigos pueden verse diferentes a los míos, pero deberían dar el mismo resultado válido.

![Generar nuevo resultado](./images/14_GenerateNewResult.jpg)

Aceptemos el resultado presionando tab.

![Aceptar el resultado](./images/15_AcceptResult.jpg)

### Paso 5: Proporciona el resultado a Leetcode

Finalmente, copiemos el código y peguémoslo en el problema de Leetcode.

[Reverse Integer](https://leetcode.com/problems/reverse-integer/).

Y presiona **Ejecutar código**.

![Ejecutar código](./images/16_LeetCodePass.jpg)

¡Voilà! Puedes ver que Leetcode pasó la prueba con éxito. Puedes enviar tu código a Leetcode y ver si puedes obtener un rango más alto. Por supuesto, eso depende totalmente de ti.
