# Exportación Universal con Pandoc

Escribir en Markdown es un placer porque te permite concentrarte al 100% en el texto, sin pelearte con los márgenes o las fuentes. Pero, ¿qué pasa si tu profesor o tu jefe te pide el documento final en Word o en PDF?

La solución profesional a este problema es **Pandoc**.

## 1. ¿Qué es Pandoc?

Pandoc es una herramienta de línea de comandos (CLI) gratuita y de código abierto que funciona como un traductor universal de documentos. Es capaz de leer un archivo escrito en un formato (como nuestro `.md`) y reescribirlo en decenas de formatos diferentes (HTML, DOCX, PDF, ePub, LaTeX, etc.) sin perder la estructura lógica: los títulos seguirán siendo títulos y las negritas seguirán siendo negritas.

## 2. Instalación

A diferencia de los editores de texto, Pandoc no tiene una interfaz gráfica con botones; se instala y se ejecuta desde la terminal de tu ordenador.

* **Windows:** Puedes instalarlo bajando el instalador desde su [página oficial](https://pandoc.org/installing.html) o usando el gestor de paquetes Winget: `winget install pandoc`.
* **macOS:** Usando Homebrew: `brew install pandoc`.
* **Linux (Ubuntu/Debian):** `sudo apt install pandoc`.

## 3. Comandos Básicos de Conversión

Una vez instalado, abre tu terminal en la carpeta donde tienes tu archivo `apuntes.md`. La sintaxis básica siempre sigue esta lógica: 
`pandoc archivo_origen -o archivo_destino`

Aquí tienes los casos de uso más comunes:

### De Markdown a Microsoft Word (.docx)
```bash
pandoc apuntes.md -o apuntes.docx
```
¡Magia! Pandoc creará un archivo Word donde tus `#` se habrán convertido en "Título 1" y tus `##` en "Título 2" nativos de Word.

### De Markdown a HTML
```bash
pandoc apuntes.md -o pagina.html
```

### De Markdown a PDF
Para exportar a PDF, Pandoc necesita un "motor" adicional que dibuje el documento (normalmente LaTeX o un conversor de HTML a PDF). Si tienes instalado `wkhtmltopdf` o `pdflatex`, el comando es igual de sencillo:
```bash
pandoc apuntes.md -o documento.pdf
```

## 4. El Poder de las Plantillas

La verdadera magia de Pandoc es que separa el **contenido** (tu archivo Markdown) de la **presentación** (el archivo final). 

Puedes decirle a Pandoc que use un archivo de Word vacío (con los colores y tipografías de tu empresa) como plantilla. Así, Pandoc inyectará tu texto Markdown en esa plantilla, generando un informe corporativo perfecto en segundos.

> **🔥 Truco Pro:** Si te da un poco de miedo usar la terminal, existen extensiones para Visual Studio Code (como *Markdown PDF* o *Pandoc Citer*) que integran estas conversiones directamente en un atajo de teclado, combinando lo mejor de ambos mundos.