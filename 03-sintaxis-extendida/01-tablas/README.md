# Tablas en Markdown

¡Bienvenido al Módulo 3! En este módulo daremos un paso más allá de la sintaxis básica para explorar características de la **Sintaxis Extendida** (muy popularizadas por GitHub). La primera y más utilizada de estas características son las tablas.

Las tablas son perfectas para presentar datos estructurados, comparar características o listar atajos de teclado en tu documentación.

## 1. Crear una Tabla Básica

Para construir una tabla, utilizamos barras verticales (`|`) para separar las columnas, y guiones (`-`) para separar la fila principal (los encabezados) del resto de los datos.

**Sintaxis:**
```text
| Encabezado 1 | Encabezado 2 | Encabezado 3 |
| ------------ | ------------ | ------------ |
| Fila 1, Col 1| Fila 1, Col 2| Fila 1, Col 3|
| Fila 2, Col 1| Fila 2, Col 2| Fila 2, Col 3|
```

> **💡 Buena Práctica:** Aunque el motor de Markdown renderizará la tabla correctamente aunque las barras verticales `|` no estén perfectamente alineadas en tu código, intentar alinearlas (añadiendo espacios) hace que tu archivo fuente sea muchísimo más fácil de leer. Existen extensiones en editores como VS Code que formatean las tablas automáticamente al guardar.

## 2. Alinear el Contenido

Por defecto, el texto dentro de las columnas se alinea a la izquierda. Sin embargo, puedes controlar la alineación añadiendo dos puntos (`:`) en la fila de guiones separadores.

* **Alinear a la izquierda:** Dos puntos al principio (suele ser el comportamiento por defecto). `| :--- |`
* **Alinear a la derecha:** Dos puntos al final. `| ---: |`
* **Centrar:** Dos puntos a ambos lados. `| :---: |`

**Sintaxis:**
```text
| Producto | Cantidad (Centrado) | Precio (Derecha) |
| :------- | :-----------------: | ---------------: |
| Teclado  | 2                   | 150.00 €         |
| Ratón    | 5                   | 45.50 €          |
| Monitor  | 1                   | 320.00 €         |
```

## 3. Formato dentro de las Tablas

Las celdas de una tabla soportan la mayoría de la sintaxis básica que aprendimos en el Módulo 2. Puedes incluir negritas, cursivas, código en línea (`inline code`), e incluso enlaces o imágenes pequeñas (como emojis o iconos).

**Sintaxis:**
```text
| Elemento | Descripción | Ejemplo visual |
| :--- | :--- | :---: |
| **Negrita** | Resalta el texto de forma fuerte | `**texto**` |
| *Cursiva* | Énfasis suave | `*texto*` |
| Enlace | Visita [MoureDev](https://moure.dev) | 🔗 |
```

> **⚠️ Importante (Limitaciones):** Las celdas de una tabla en Markdown están pensadas para contener texto en una sola línea. Por lo general, **no puedes** incluir bloques de código multilínea (con las tres comillas invertidas), citas (`>`) o listas estructuradas dentro de una celda de tabla convencional.