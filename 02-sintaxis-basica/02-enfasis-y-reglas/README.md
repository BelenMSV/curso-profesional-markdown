# Énfasis y Reglas Horizontales

Para que un texto sea fácil de leer, es fundamental saber cómo destacar las ideas más importantes y cómo separar visualmente los distintos bloques de información. Markdown nos permite hacer esto de una forma muy rápida sin tener que apartar las manos del teclado.

## Énfasis: Negrita y Cursiva

Markdown utiliza asteriscos (`*`) o guiones bajos (`_`) para aplicar énfasis al texto. Ambos símbolos funcionan exactamente igual, puedes elegir el que te resulte más cómodo.

### 1. Cursiva (Italic)
Para poner un texto en cursiva, debes envolverlo con **un solo** asterisco o guión bajo.

**Sintaxis:**
```text
*Este texto está en cursiva*
_Este texto también está en cursiva_
```

### 2. Negrita (Bold)
Para destacar un texto en negrita, debes envolverlo con **dos** asteriscos o dos guiones bajos.

**Sintaxis:**
```text
**Este texto resalta en negrita**
__Este texto también resalta en negrita__
```

### 3. Negrita y Cursiva a la vez
Si necesitas el máximo énfasis combinando ambos estilos, simplemente utiliza **tres** asteriscos o guiones bajos.

**Sintaxis:**
```text
***Este texto está en negrita y cursiva***
___Este texto también está en negrita y cursiva___
```

> **💡 Buena Práctica:** La comunidad de desarrolladores suele preferir el uso de asteriscos (`*` y `**`) para cursivas y negritas, ya que los guiones bajos a veces pueden dar problemas si están dentro de una palabra (por_ejemplo_asi). ¡Te recomendamos usar siempre asteriscos!

---

## Reglas Horizontales

Las reglas son divisiones visuales en forma de línea. Son muy útiles para separar secciones de un documento cuando un cambio de encabezado no es suficiente, o para finalizar un artículo.

Para crear una regla horizontal, debes colocar tres o más asteriscos (`***`), guiones (`---`) o guiones bajos (`___`) solos en una línea. 

**Sintaxis:**
```text
***

---

___
```

> **⚠️ Importante:** Para que la regla horizontal con guiones (`---`) funcione correctamente y no se confunda con la sintaxis alternativa de los encabezados de nivel 2, asegúrate siempre de **dejar una línea en blanco** justo antes de los guiones.