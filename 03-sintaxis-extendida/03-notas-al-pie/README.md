# Notas al Pie (Footnotes)

Las notas al pie son una herramienta excelente de la sintaxis extendida. Te permiten añadir referencias, aclaraciones o comentarios adicionales sin interrumpir el flujo de lectura principal.

Al usar notas al pie, el motor de Markdown creará automáticamente un enlace con un número en superíndice en tu texto, que al pulsarlo llevará al lector hasta la definición de la nota al final del documento. ¡Además, suele añadir una pequeña flecha de retorno para volver al texto exacto donde se quedó!

## 1. Sintaxis Básica

Crear una nota al pie siempre requiere dos partes:
1. **La referencia en el texto:** Se escribe usando corchetes, un acento circunflejo (`^`) y un identificador (puede ser un número o una palabra). Ejemplo: `[^1]`.
2. **La definición de la nota:** Se escribe generalmente al final del documento, usando la misma referencia seguida de dos puntos (`:`) y el texto explicativo.

**Sintaxis:**
```text
Este es un texto normal que necesita una aclaración técnica.[^1] 
También puedes usar palabras descriptivas como identificadores.[^nota-api]

[^1]: Esta es la explicación técnica que aparecerá al final del documento.
[^nota-api]: Aunque uses una palabra como identificador, Markdown renderizará las referencias como números secuenciales (1, 2, 3...) de forma automática en el resultado final.
```

> **💡 Buena Práctica:** Por convención y para mantener tu código fuente limpio y predecible, te recomendamos agrupar siempre todas las definiciones de las notas al pie en la parte inferior de tu documento, tal y como aparecerían en un libro real.

## 2. Notas Multilínea

Si necesitas que tu nota al pie contenga varios párrafos, código fuente o listas, puedes hacerlo indentando las líneas siguientes con cuatro espacios (o un tabulador).

**Sintaxis:**
```text
Aquí mencionamos un concepto complejo de programación.[^complejo]

[^complejo]: Este es el primer párrafo de la explicación.
    
    Este es el segundo párrafo, indentado con cuatro espacios o un tabulador. 
    Seguirá formando parte de la nota al pie número 1.
```