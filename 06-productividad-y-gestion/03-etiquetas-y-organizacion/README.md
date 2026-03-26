# Etiquetas (Tags) y Organización

A medida que tu "Segundo Cerebro" crece y acumulas cientos o miles de archivos Markdown, las carpetas tradicionales se quedan cortas. Un archivo solo puede vivir en una carpeta, pero una idea puede pertenecer a múltiples categorías.

Para solucionar esto, las herramientas de Gestión del Conocimiento Personal (PKM) como Obsidian, Logseq o Notion utilizan **Etiquetas (Tags)**.

## 1. La Sintaxis Básica: El Símbolo Almohadilla `#`

Para crear una etiqueta, simplemente escribimos el símbolo de almohadilla (`#`) seguido de una palabra, **sin espacios**. 

**Sintaxis:**
```markdown
Hoy he estado practicando cómo hacer tablas en #markdown para mejorar mi #productividad en el #trabajo.
```

Al hacer clic en cualquiera de esas etiquetas, tu aplicación buscará instantáneamente todos los archivos `.md` de tu ordenador que contengan esa misma etiqueta, sin importar en qué carpeta estén guardados.

> **⚠️ ¡Cuidado con los Títulos!**
> Recuerda que en Markdown estándar, la almohadilla se usa para los encabezados (Títulos). La diferencia clave es el **espacio**.
> * `# Título 1` (Lleva espacio = Es un encabezado).
> * `#etiqueta` (No lleva espacio = Es una etiqueta).

## 2. Etiquetas Anidadas (Jerarquía)

Una de las características más potentes de las herramientas PKM modernas es el soporte para etiquetas anidadas. Esto te permite crear "sub-etiquetas" utilizando la barra inclinada (`/`).

**Sintaxis:**
```markdown
Este artículo es sobre el nuevo framework de JavaScript: #tecnologia/programacion/javascript
```

La ventaja de esto es que, si buscas `#tecnologia`, la aplicación te mostrará todos los archivos que tengan esa etiqueta general, pero también los que tengan etiquetas más específicas derivadas de ella.

## 3. ¿Dónde colocar las etiquetas? (Inline vs Frontmatter)

Existen dos formas principales de añadir etiquetas a tus documentos:

1. **Inline (En el texto):** Las escribes directamente en medio de tus párrafos, como hemos visto en los ejemplos anteriores. Es genial para tomar apuntes rápidos.
2. **YAML Frontmatter (Metadatos):** Como aprendimos en el Módulo 4, puedes colocar tus etiquetas en el bloque oculto al principio del documento. Esto mantiene tu texto limpio y es la forma más profesional de clasificar artículos.

```markdown
---
title: "Guía de Etiquetas"
tags: [markdown, organizacion, pkm]
status: terminado
---
# El contenido de mi nota empieza aquí...
```

## 4. Buenas Prácticas para no volverse loco

* **Menos es más:** No crees etiquetas para cada palabra. Usa las etiquetas para **categorías amplias** (`#reuniones`, `#ideas`, `#libros`) y usa los enlaces bidireccionales (`[[ ]]`) para conceptos específicos.
* **Etiquetas de Estado:** Mucha gente usa las etiquetas para definir en qué fase está un documento (ej. `#estado/borrador`, `#estado/revision`, `#estado/publicado`).