# Tachado y Resaltado

En ocasiones, redactar buena documentación no solo consiste en añadir información, sino en indicar de forma visual qué datos ya no son válidos o qué palabras son absolutamente críticas. Para eso utilizamos el tachado y el resaltado.

## 1. Tachado (Strikethrough)

El tachado es muy útil para corregir errores manteniendo el contexto original visible (por ejemplo, cuando actualizas un precio, una fecha o un requisito). 

Para tachar un texto en la sintaxis extendida (plenamente soportada por GitHub), debes envolver la palabra o frase con dos virgulillas (`~~`). 
*(Nota: La virgulilla es el símbolo de la onda que lleva la letra "ñ" encima).*

**Sintaxis:**
```text
El precio de lanzamiento era de ~~45.00 €~~, pero ahora está en oferta a **30.00 €**.

~~Esta característica ha sido deprecada en la versión 2.0.~~
```

## 2. Resaltado (Highlight)

El resaltado simula el efecto de marcar el texto con un rotulador fluorescente (generalmente con un fondo amarillo). Es ideal para destacar términos clave dentro de un párrafo denso.

Aquí hay que tener en cuenta un pequeño detalle técnico: **no todos los motores de Markdown soportan el resaltado nativo de la misma manera**.

1. **En editores modernos (como Obsidian, Typora o Markdoc):** La sintaxis extendida habitual es envolver el texto con dos signos de igual (`==`).
2. **En GitHub y sitios estándar:** Como GitHub no soporta los signos de igual para esto, la forma más segura y universal de hacerlo es usando la etiqueta HTML `<mark>`.

**Sintaxis:**
```text
Sintaxis en Obsidian/Typora: ==Este texto aparecerá resaltado en amarillo==.

Sintaxis universal (GitHub): <mark>Este texto aparecerá resaltado en amarillo</mark>.
```

> **🔥 Truco Pro:** ¡Puedes combinar estos formatos con la sintaxis básica que aprendiste en el Módulo 2! Por ejemplo, puedes tener un texto que esté tachado y en cursiva al mismo tiempo (`~~*texto*~~`), o resaltar algo que además es un enlace (`<mark>[Google](https://google.com)</mark>`).