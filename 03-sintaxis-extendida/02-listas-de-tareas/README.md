# Listas de Tareas (Task Lists)

Las listas de tareas son una de las extensiones más útiles y populares de Markdown, especialmente en plataformas de gestión de proyectos y repositorios de código como GitHub o GitLab. 

Nos permiten crear *checklists* interactivos para llevar el control de subtareas, organizar el trabajo diario o marcar los requisitos de un proyecto.

## 1. Sintaxis Básica

Para crear una lista de tareas, partimos de una lista desordenada normal (usando guiones `-` o asteriscos `*`) y le añadimos unos corchetes. 

Usamos `[ ]` (con un espacio en blanco en medio) para una tarea pendiente, y `[x]` para una tarea completada.

**Sintaxis:**
```text
- [ ] Tarea pendiente (requiere un espacio entre los corchetes).
- [x] Tarea completada (puedes usar la 'x' en minúscula o mayúscula).
- [ ] Tercera tarea pendiente.
```

> **⚠️ Importante:** La sintaxis es muy estricta con los espacios. Asegúrate de dejar un espacio después del guion inicial, y otro espacio después del cierre del corchete antes de empezar a escribir el texto.

## 2. Listas de Tareas Anidadas

Al igual que las listas normales que vimos en el Módulo 2, las listas de tareas se pueden anidar usando la indentación (tabulador o cuatro espacios) y se pueden combinar con estilos de texto.

**Sintaxis:**
```text
### Preparativos para el lanzamiento 🚀

- [x] Revisar el **código fuente**.
- [x] Escribir la documentación técnica:
    - [x] Completar Módulo 1.
    - [x] Completar Módulo 2.
    - [ ] Redactar Módulo 3.
- [ ] Publicar la versión `1.0.0`.
```

> **🔥 Truco Pro (Interactividad en GitHub):** Cuando visualizas un archivo Markdown con listas de tareas en la web de GitHub (por ejemplo, en la descripción de un *Issue* o un *Pull Request*), los corchetes se renderizan como casillas de verificación clicables. Si haces clic en la casilla para marcarla, ¡GitHub actualizará automáticamente el código fuente de tu archivo Markdown cambiando el `[ ]` por un `[x]` por detrás!