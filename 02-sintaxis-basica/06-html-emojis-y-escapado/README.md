# HTML, Emojis y Escapado de Caracteres

Markdown está diseñado para ser sencillo y cubrir el 90% de las necesidades de formato. Pero, ¿qué pasa cuando necesitas ese 10% extra o quieres evitar que Markdown formatee un texto por error? Aquí entran en juego el HTML, los emojis y el escapado de caracteres.

## 1. Soporte para HTML puro

Una de las grandes ventajas de Markdown es que es totalmente compatible con HTML. Si necesitas un formato que Markdown no soporta de forma nativa (como cambiar el color del texto, centrar elementos o usar etiquetas específicas), puedes escribir la etiqueta HTML directamente en tu documento.

**Ejemplos útiles:**
```html
<p align="center">Este texto estará centrado.</p>

Pulsa la tecla <kbd>Ctrl</kbd> + <kbd>C</kbd> para copiar.

<span style="color:red;">Este texto aparecerá en color rojo.</span>
```
> **💡 Buena Práctica:** Usa HTML solo cuando sea estrictamente necesario. Abusar del HTML rompe la principal ventaja de Markdown: que el texto fuente sea fácil de leer.

## 2. Emojis

Los emojis son fantásticos para dar un tono más amigable a la documentación, estructurar ideas o simplemente llamar la atención sobre un punto crítico. Tienes dos formas de usarlos:

1. **Copiando y pegando:** Puedes copiar un emoji directamente desde cualquier sitio web o usar el teclado de emojis de tu sistema operativo (`Win + .` en Windows o `Cmd + Ctrl + Espacio` en Mac).
2. **Shortcodes (Códigos cortos):** Muchas plataformas (como GitHub o Slack) soportan códigos entre dos puntos.

**Sintaxis de Shortcodes:**
```text
¡Hola mundo! :wave:
Esto es un cohete :rocket:
Atención a este bug :bug:
```

## 3. Escapado de Caracteres

A veces necesitas escribir un símbolo que Markdown usa para formatear (como un asterisco `*` o un hashtag `#`), pero quieres que se vea como texto normal en lugar de aplicar negrita o crear un encabezado. 

Para lograrlo, debes "escapar" el carácter colocando una barra invertida (`\`) justo delante de él.

**Sintaxis:**
```text
\*Este texto está rodeado de asteriscos literales, no está en cursiva\*

\# Esto no es un encabezado, es solo una almohadilla.

Sin la barra invertida, el símbolo \> crearía una cita.
```
Markdown permite escapar la mayoría de sus caracteres especiales:
`\` `*` `_` `{}` `[]` `()` `#` `+` `-` `.` `!` `|`