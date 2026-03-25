# Alojamiento Gratuito: GitHub Pages y Vercel

Una vez que has transformado tus archivos Markdown en una página web real usando un Generador de Sitios Estáticos (SSG) o simplemente quieres mostrar tu documentación técnica, el siguiente paso es que el mundo entero pueda verla.

La mejor noticia del ecosistema web moderno es que alojar estos sitios estáticos (conocidos como arquitectura *Jamstack*) es **100% gratuito**, ultrarrápido y automático. Aquí te presentamos las dos opciones más populares de la industria.

## 1. GitHub Pages

Si ya tienes tu proyecto alojado en GitHub, esta es la opción más natural y directa. GitHub Pages te permite publicar una página web directamente desde un repositorio.

* **Ideal para:** Documentación técnica de repositorios, portafolios personales y blogs básicos (GitHub Pages usa el motor Jekyll por defecto para compilar Markdown).
* **Cómo funciona:** Vas a la pestaña `Settings` de tu repositorio, buscas el menú lateral `Pages` y seleccionas la rama (*branch*) desde la que quieres publicar.
* **URL por defecto:** `https://tu-usuario.github.io/tu-repositorio/`

## 2. Vercel (o Netlify)

Si estás utilizando herramientas modernas como Astro, Docusaurus o Hugo para generar tu sitio web a partir de Markdown, plataformas como **Vercel** o **Netlify** son la opción profesional por excelencia.

* **Ideal para:** Blogs modernos, sitios web muy rápidos y proyectos complejos impulsados por contenido.
* **Cómo funciona:** Te creas una cuenta gratuita en Vercel, la conectas con tu cuenta de GitHub y seleccionas tu repositorio. Vercel detectará automáticamente qué SSG estás usando, compilará todos tus archivos `.md` o `.mdx` en HTML y los publicará en servidores de todo el mundo (CDN).
* **URL por defecto:** `https://nombre-de-tu-proyecto.vercel.app/`

## 3. La Magia del "Despliegue Continuo"

Lo mejor de este flujo de trabajo moderno es que solo tienes que configurarlo una vez. A partir de ahí, el proceso es automático (esto en el mundo del desarrollo se conoce como CI/CD):

1. Escribes un nuevo artículo en Markdown (`nuevo-post.md`) en tu ordenador.
2. Guardas los cambios, haces un `git commit` y un `git push` a tu repositorio en GitHub.
3. Plataformas como Vercel detectan el cambio en el código instantáneamente.
4. Toman tu nuevo Markdown, lo compilan y actualizan tu página web en cuestión de segundos, sin que tú toques ningún servidor.

> **🔥 Truco Pro:** Aunque estas plataformas te dan un subdominio gratuito (como `.github.io`), todas te permiten configurar un **dominio personalizado** (ej. `www.tu-nombre.com`) de forma totalmente gratuita. ¡Solo tienes que comprar el dominio en un registrador y apuntarlo a tu proyecto!