# Alertas y Paneles (Callouts/Admonitions)

En la documentación técnica, a menudo necesitamos destacar un consejo, una advertencia de seguridad o una nota importante para que el lector no la pase por alto. Para esto utilizamos las alertas o paneles (también conocidos como *callouts* o *admonitions*).

Aunque no formaban parte del Markdown original, plataformas como GitHub han estandarizado una sintaxis visual muy sencilla basada en las citas de texto (`>`).

## 1. Alertas en GitHub

Recientemente, GitHub introdujo soporte nativo para cinco tipos de alertas de colores. Para crearlas, solo tienes que iniciar una cita normal con el símbolo mayor que (`>`) y añadir una de las etiquetas admitidas entre corchetes, con signo de exclamación y en mayúsculas, en la primera línea.

**Las 5 etiquetas disponibles son:**
* `[!NOTE]` (Nota - Azul): Información útil que aporta contexto adicional.
* `[!TIP]` (Consejo - Verde): Recomendaciones opcionales, atajos o mejores prácticas.
* `[!IMPORTANT]` (Importante - Morado): Información crucial para que el usuario logre su objetivo.
* `[!WARNING]` (Advertencia - Amarillo): Información crítica que avisa de posibles problemas.
* `[!CAUTION]` (Precaución - Rojo): Advierte sobre consecuencias negativas graves (como pérdida de datos).

**Sintaxis:**
```text
> [!NOTE]
> Esta es una nota informativa básica. Puedes incluir **negritas** o `código en línea` aquí dentro.

> [!WARNING]
> Ten mucho cuidado antes de borrar la base de datos de producción.
```

## 2. Compatibilidad en otros entornos

Es importante tener en cuenta que, aunque esta sintaxis (`> [!TIPO]`) es el estándar oficial en GitHub y está soportada por herramientas populares como Obsidian, otros generadores de documentación técnica pueden usar variaciones distintas.

Por ejemplo, herramientas como **MkDocs** o **Docusaurus** suelen usar un formato basado en tres exclamaciones de apertura (`!!! note`) o tres signos de suma. 

> **💡 Buena Práctica:** Si tu archivo `README.md` va a vivir principalmente en tu repositorio de GitHub, usa siempre la sintaxis de corchetes `> [!NOTE]`. Se verá espectacular y profesional.