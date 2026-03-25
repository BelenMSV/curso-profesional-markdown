# Plantillas de GitHub (Templates)

Cuando tu proyecto empieza a crecer y otras personas quieren colaborar, es muy común que abran *Issues* (reportando fallos) o *Pull Requests* (enviando código) sin proporcionar la información necesaria. 
    
Para evitar esto, GitHub nos permite crear plantillas en Markdown. Así, cuando alguien intente crear un *Issue* o un *PR*, el cuadro de texto de GitHub ya vendrá pre-rellenado con la estructura que tú decidas.

## 1. La carpeta mágica `.github`

Para que GitHub detecte tus plantillas automáticamente, estas deben guardarse en un directorio específico. Por convención y buenas prácticas, se crea una carpeta oculta llamada `.github` en la raíz de tu repositorio.

Dentro de esta carpeta es donde guardaremos nuestros archivos Markdown de plantillas.

## 2. Plantilla para Issues (`ISSUE_TEMPLATE.md`)

Esta plantilla se usará cada vez que alguien reporte un bug o sugiera una mejora en la pestaña "Issues".

**Ruta del archivo:** `.github/ISSUE_TEMPLATE.md`

**Ejemplo de contenido:**
```markdown
## Descripción del Problema
<!-- Describe de forma clara y concisa cuál es el error o la sugerencia. -->
## Pasos para reproducirlo
<!-- Si es un bug, enumera los pasos para que podamos verlo nosotros también. -->
1. Ir a '...'
2. Hacer clic en '...'
3. Ver el error

## Comportamiento esperado
<!-- ¿Qué debería haber pasado? -->
## Entorno (por favor, completa esta información)
- **Sistema Operativo:** [ej. Windows 11, macOS]
- **Navegador:** [ej. Chrome, Safari]
- **Versión del proyecto:** [ej. v1.0.2]
```

## 3. Plantilla para Pull Requests (`PULL_REQUEST_TEMPLATE.md`)

Esta plantilla aparecerá cuando alguien envíe código para integrarlo en tu proyecto. Es vital para asegurar que el código nuevo cumple con tus estándares antes de revisarlo.

**Ruta del archivo:** `.github/PULL_REQUEST_TEMPLATE.md`

**Ejemplo de contenido:**
```markdown
## ¿Qué soluciona este PR?
<!-- Enlaza el Issue que resuelve (ej. Fixes #123) o explica el propósito de este código. -->
## Tipo de cambio
<!-- Marca con una 'x' las opciones que correspondan -->
- [ ] 🐛 Bugfix (corrección de un error)
- [ ] ✨ Nueva característica (feature)
- [ ] 📝 Actualización de documentación
- [ ] 🚀 Optimización de rendimiento

## Checklist
<!-- Asegúrate de haber cumplido lo siguiente antes de enviar el PR -->
- [ ] He probado mi código localmente y funciona bien.
- [ ] He añadido comentarios a las partes complejas del código.
- [ ] Mi código no genera nuevas advertencias (warnings).
```

> **🔥 Truco Pro:** ¡Fíjate cómo hemos combinado los comentarios HTML ocultos `<!-- ... -->` con las listas de tareas `[ ]` que aprendimos en el Módulo 3! Los comentarios no se verán en el *Issue* o *PR* final, pero servirán de instrucciones para la persona que está rellenando la plantilla.