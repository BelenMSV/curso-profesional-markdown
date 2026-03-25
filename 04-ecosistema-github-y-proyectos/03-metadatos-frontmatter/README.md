# Metadatos (YAML Frontmatter)

A medida que Markdown se convirtió en el estándar para escribir blogs y sitios web estáticos (con herramientas como Jekyll, Hugo, Astro o Next.js), surgió un problema: *¿Cómo le decimos al sistema la fecha de publicación, el autor o las etiquetas del post sin que ese texto aparezca directamente en el artículo?*

La solución a esto se llama **Frontmatter** (que se traduce como "materia frontal" o "preámbulo").

## 1. ¿Qué es el Frontmatter?

El Frontmatter es un bloque especial de metadatos que se coloca **estrictamente en la primera línea** de tu archivo Markdown. 

Sirve para definir variables ocultas sobre el documento. Estas variables no suelen renderizarse como texto normal cuando el usuario lee el archivo, pero son procesadas por el motor o la aplicación que lee el Markdown para organizar el contenido.

## 2. Sintaxis Básica (YAML)

El formato más común para escribir este bloque es **YAML** (un lenguaje de serialización de datos muy legible). 

Para crear un bloque Frontmatter, debes abrirlo con tres guiones (`---`), escribir tus variables en formato `clave: valor`, y cerrarlo con otros tres guiones (`---`).

**Sintaxis:**
```markdown
---
title: "Cómo dominar Markdown en 2024"
author: "Tu Nombre"
date: 2024-10-25
draft: false
tags: [tutorial, productividad, github]
---

# Bienvenido a mi artículo

A partir de aquí, después del segundo bloque de guiones, empiezas a escribir tu documento Markdown normal y corriente...
```

## 3. Casos de Uso Comunes

El Frontmatter no es algo nativo de la especificación original de Markdown, ni es algo que GitHub renderice de forma especial en sus repositorios normales. Sin embargo, es **imprescindible** si utilizas:

* **Gestores de Conocimiento:** Herramientas como *Obsidian* o *Logseq* lo usan para añadir propiedades a tus notas (como el estado de una tarea, alias de la nota o fechas de revisión).
* **Generadores de Sitios Estáticos (SSG):** Motores de blogs como *Astro* o *Gatsby* leen estas variables para saber qué título poner en la pestaña del navegador, qué imagen de portada cargar para redes sociales, o en qué categoría agrupar el artículo.

> **⚠️ Regla de Oro:** Para que el Frontmatter funcione correctamente, **nada** puede ir antes de los primeros tres guiones (`---`). Ni un espacio en blanco, ni un salto de línea, ni un título. Debe ser el carácter número uno de tu archivo.