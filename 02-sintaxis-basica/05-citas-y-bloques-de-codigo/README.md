# Citas y Bloques de Código

En la documentación técnica y en artículos, es muy común tener que citar a otros autores o mostrar ejemplos de código fuente. Markdown nos ofrece herramientas específicas para que ambos elementos destaquen visualmente del resto del texto.

## 1. Citas (Blockquotes)

Las citas se utilizan para resaltar textos citados o destacados. Para crear una cita, simplemente añade el símbolo mayor que (`>`) seguido de un espacio al principio de la línea.

Además, las citas pueden llegar a anidarse (colocar una cita dentro de otra) añadiendo más símbolos `>`.

**Sintaxis:**
```text
> Cita de primer nivel
>> Cita de segundo nivel dentro de la anterior
>>> Cita de tercer nivel
```

## 2. Código y fragmentos de código

Markdown permite incluir código fuente como una línea dentro de un párrafo o como bloques multilínea.

### Código en línea (Inline code)
Para resaltar un comando, nombre de archivo o un pequeño fragmento de código dentro de un párrafo, envuélvelo entre comillas invertidas simples (`` ` ``).

**Sintaxis:**
```text
Para ver los cambios en tu repositorio, ejecuta el comando `git status`.
```

### Bloques de código multilínea
Si necesitas mostrar varias líneas de código, debes envolver el bloque usando tres comillas invertidas tanto en la línea anterior como en la posterior al código.

**Sintaxis:**
````text
```html
<html>
<head>
  <title>Ejemplo</title>
</head>
<body>
  <h1>Hola Mundo</h1>
</body>
</html>
```
````

> **🔥 Truco Pro (Resaltado de sintaxis):** Cuando creas un bloque multilínea, puedes escribir el nombre del lenguaje de programación justo después de las tres primeras comillas (por ejemplo, ```` ```html ````, ```` ```javascript ```` o ```` ```python ````). GitHub y otros visores leerán esto y colorearán automáticamente tu código con la sintaxis correcta, ¡haciéndolo mucho más profesional y fácil de leer!