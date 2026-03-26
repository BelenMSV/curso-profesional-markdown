# Enlaces Bidireccionales (Wikilinks)

El sistema tradicional de carpetas en nuestros ordenadores nos obliga a guardar un archivo en un único lugar. Pero, ¿cómo funciona el cerebro humano? Nuestro cerebro no usa carpetas; usa **conexiones**. Una idea te lleva a otra.

Para replicar esto en nuestras notas, herramientas como Obsidian, Logseq, Notion (¡e incluso GitHub en sus Wikis e Issues!) adoptaron una sintaxis especial de Markdown: los **enlaces bidireccionales** o *Wikilinks*.

## 1. La Sintaxis Básica: Corchetes Dobles `[[ ]]`

En lugar de escribir la ruta completa de un archivo como hacíamos en el Markdown clásico, simplemente envolvemos el nombre exacto de la nota a la que queremos enlazar entre dos corchetes dobles.

**Sintaxis:**
```markdown
Ayer estuve leyendo sobre el [[Patrón de Diseño Singleton]] y creo 
que podríamos aplicarlo en el nuevo proyecto de la empresa.
```

Al hacer clic en ese enlace, la aplicación abrirá automáticamente el archivo llamado `Patrón de Diseño Singleton.md`. Si el archivo no existe, ¡lo creará por ti al instante!

## 2. Alias de Enlace (Texto a Mostrar)

A veces, el nombre exacto de tu archivo no encaja gramaticalmente en la frase que estás escribiendo. Para solucionarlo, puedes usar el símbolo de la barra vertical o *pipe* (`|`) dentro de los corchetes. 

La primera parte será el archivo real, y la segunda parte será el texto que leerá el usuario.

**Sintaxis:**
```markdown
El funcionamiento del cerebro humano se basa en crear 
[[Redes Neuronales|conexiones entre conceptos]].
```
*(El enlace llevará a la nota "Redes Neuronales.md", pero en pantalla solo se leerá "conexiones entre conceptos").*

## 3. ¿Por qué se llaman "Bidireccionales"?

Aquí es donde ocurre la magia. En un enlace web normal (unidireccional), la "Página A" enlaza a la "Página B", pero la "Página B" no tiene ni idea de quién la está enlazando.

En herramientas como Obsidian, cuando usas `[[ ]]`, el enlace es **bidireccional**. 
Si estás leyendo la nota `Página B`, la aplicación te mostrará un panel llamado **Backlinks** (Enlaces entrantes), donde podrás ver exactamente qué otras notas (como la `Página A`) han mencionado a la `Página B`, e incluso leer el párrafo exacto donde te mencionaron.

## 4. El Gráfico de Conocimiento (Graph View)

Gracias a que estos enlaces de Markdown conectan tus archivos en ambas direcciones, herramientas como Obsidian o Logseq pueden generar un **Gráfico Visual** (Graph View). 

En lugar de ver una lista aburrida de carpetas, verás una constelación de puntos unidos por líneas, revelando cómo tus ideas, apuntes de clase o notas de reuniones se conectan entre sí. ¡Acabas de crear tu propia Wikipedia personal!

> **⚠️ Nota de Compatibilidad:** Los corchetes dobles `[[ ]]` no son parte de la especificación oficial original de Markdown (CommonMark), sino una extensión. Funcionan perfectamente en herramientas PKM (Obsidian, Logseq, Roam) y en GitHub, pero podrían no renderizarse correctamente si los exportas a un PDF tradicional usando Pandoc sin configurarlo previamente.