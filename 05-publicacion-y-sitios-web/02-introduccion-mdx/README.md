# Introducción a MDX

Markdown tradicional es fantástico para contenido estático (texto, listas, imágenes). Pero la web moderna es interactiva. Si intentas poner un componente de React, Vue o un botón con lógica compleja dentro de un archivo `.md` normal, simplemente no funcionará.

Para solucionar esta limitación nació **MDX**.

## 1. ¿Qué es MDX?

MDX es una evolución de Markdown que te permite escribir **JSX** (el formato que usa React para crear componentes web) directamente dentro de tus documentos Markdown. 

La extensión de estos archivos pasa a ser `.mdx` en lugar de `.md`. 

Con MDX puedes importar componentes programados a medida y mezclarlos con tus párrafos y encabezados normales de forma totalmente fluida.

## 2. Sintaxis de Ejemplo

Imagina que has programado un componente de React llamado `<BotonMagico />` o un gráfico de barras llamado `<GraficoVentas />`. En un archivo MDX, puedes importarlos y usarlos así:

```mdx
---
title: Mi artículo interactivo
date: 2024-11-01
---

import { BotonMagico } from '../components/BotonMagico.jsx';
import { GraficoVentas } from '../components/GraficoVentas.jsx';

# Bienvenidos al futuro del contenido

El texto normal de Markdown sigue funcionando exactamente igual. Puedes usar **negritas**, crear listas o poner imágenes.

Pero ahora, si quiero que el usuario interactúe, puedo incrustar mi componente directamente:

<BotonMagico texto="¡Haz clic para una sorpresa!" />

Y justo debajo, puedo mostrar datos en tiempo real:

<GraficoVentas año="2024" />
```

## 3. ¿Por qué es tan revolucionario?

Plataformas gigantes como *Stripe*, *Tailwind CSS* o *React* utilizan MDX (o tecnologías muy similares) para su documentación oficial por varias razones:

* **Documentación Viva:** Puedes escribir un tutorial de código y justo debajo renderizar el componente real funcionando, en lugar de poner una simple captura de pantalla.
* **Reutilización:** Si actualizas el diseño de tu `<BotonMagico />` en el código de tu web, se actualizará automáticamente en todos los artículos `.mdx` donde lo hayas usado.
* **Diseño sin límites:** Ya no estás restringido a las etiquetas HTML básicas que permite Markdown.

> **⚠️ Nota Importante:** MDX **no** está soportado de forma nativa por GitHub en su visualizador estándar. Es una tecnología diseñada específicamente para ser procesada por Generadores de Sitios Estáticos (SSG) como Astro, Docusaurus, Next.js o Gatsby.