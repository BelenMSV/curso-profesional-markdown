# Encabezados y Párrafos

En este primer tema de sintaxis básica, vamos a aprender cómo estructurar el esqueleto de cualquier documento: los títulos y los bloques de texto.

## Encabezados (Headings)

Los encabezados nos ayudan a organizar el contenido jerárquicamente, igual que en un libro o en una página web. Markdown admite hasta seis niveles de encabezado. Para crearlos, utilizamos el símbolo de la almohadilla (`#`); la cantidad de almohadillas establece el nivel jerárquico del título.

**Sintaxis principal:**

```text
# Título de nivel 1 (Equivale a <h1> en HTML)
## Título de nivel 2 (Equivale a <h2>)
### Título de nivel 3 (Equivale a <h3>)
#### Título de nivel 4 (Equivale a <h4>)
##### Título de nivel 5 (Equivale a <h5>)
###### Título de nivel 6 (Equivale a <h6>)
```

> **💡 Buena Práctica (SEO y Accesibilidad):** Aunque puedes usar los niveles como quieras, lo ideal es usar un único `#` (H1) por documento para el título principal, y usar `##` y `###` para estructurar el resto del contenido de forma lógica. Además, recuerda siempre dejar un espacio entre el símbolo `#` y el texto.

**Sintaxis alternativa:**
Para los niveles 1 y 2, Markdown también permite una sintaxis alternativa "subrayando" el texto con signos de igual (`=`) o guiones (`-`):

```text
Título de nivel 1
=================

Título de nivel 2
-----------------
```

## Párrafos y Saltos de línea

El manejo de los párrafos en Markdown a veces confunde a los principiantes porque no funciona exactamente igual que un procesador de texto tradicional.

### 1. Crear un párrafo nuevo
Para separar párrafos, se debe dejar una línea completamente en blanco entre ellos. Si no se deja esta línea en blanco, Markdown considerará que las líneas de texto pertenecen al mismo párrafo y las unirá.

**Ejemplo incorrecto (se verá todo en la misma línea):**
```text
Este es el primer párrafo.
Y este texto se unirá al anterior porque no hay línea en blanco.
```

**Ejemplo correcto:**
```text
Este es el primer párrafo.

Este es el segundo párrafo, ahora sí, correctamente separado.
```

### 2. Forzar un salto de línea (Soft Break)
A veces quieres bajar a la siguiente línea, pero sin crear un párrafo nuevo (útil en poemas, direcciones postales, etc.). Para forzar un salto de línea dentro de un mismo párrafo puedes terminar con dos espacios en blanco y pulsar enter.

También puedes usar la etiqueta HTML `<br>` si quieres que el código sea más visual para otros desarrolladores.

**Ejemplo:**
```text
Primera línea del texto.  
Segunda línea del texto justo debajo.

O también:
Primera línea del texto.<br>
Segunda línea del texto justo debajo.
```
