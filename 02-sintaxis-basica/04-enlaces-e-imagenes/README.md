# Enlaces e Imágenes

En este tema aprenderemos a conectar nuestro documento con el resto de internet y a enriquecerlo visualmente insertando imágenes.

## 1. Enlaces (Hipervínculos)

Markdown soporta varias formas de crear enlaces. La forma más común es utilizando corchetes para el texto que queremos que sea visible (el texto ancla) y paréntesis pegados para la URL de destino.

**Sintaxis clásica:**
```text
[Ir a Google](https://google.com)
```

**Sintaxis de enlace automático (Autolink):**
Si solo quieres mostrar la URL tal cual y que sea clicable directamente, puedes envolverla entre signos de menor y mayor.
```text
<https://google.com>
```

> **💡 Buena Práctica (Accesibilidad):** Siempre que sea posible, es recomendable usar la sintaxis clásica `[Texto descriptivo](URL)`. Un texto descriptivo como "Ver la documentación oficial" es mucho más accesible y amigable para el usuario que simplemente dejar un enlace suelto como `https://...`.

## 2. Imágenes

La sintaxis de las imágenes es muy similar a la de los enlaces, con la única diferencia de que comienza con un signo de exclamación (`!`).

**Sintaxis:**
```text
![Texto alternativo](https://moure.dev/logo.svg "Título opcional")
```

Vamos a desglosar sus partes para entenderlo mejor:
* `!`: Le indica al motor de Markdown que debe incrustar y renderizar una imagen, no simplemente crear un enlace.
* `[Texto alternativo]`: Describe lo que se ve en la imagen. Es fundamental para el SEO, para los lectores de pantalla (accesibilidad) o por si el enlace de la imagen se rompe.
* `(URL)`: Es la ruta donde se encuentra el archivo de imagen. La URL puede ser absoluta o relativa al documento.
* `"Título opcional"`: Es el texto que aparecerá en un pequeño globo (tooltip) cuando el usuario pase el ratón por encima de la imagen.

> **🔥 Truco Pro (Rutas Relativas en GitHub):** Cuando creas repositorios, es muy común guardar las imágenes en una subcarpeta (por ejemplo, llamada `assets` o `images`). Puedes enlazar esas imágenes usando rutas relativas así: `![Mi captura](./assets/captura.png)`. De esta forma, las imágenes siempre cargarán correctamente, incluso si alguien descarga tu código a su ordenador.