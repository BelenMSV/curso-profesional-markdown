# Listas Ordenadas y Desordenadas

Las listas son fundamentales para organizar información de forma estructurada y fácil de leer. Podemos crear listas no ordenadas (viñetas) como ordenadas (numeradas).

## 1. Listas Desordenadas (Viñetas)

Las listas no ordenadas comienzan cada elemento con `-`, `*` o `+`, seguido de espacio. 

**Sintaxis:**
```text
* Elemento 1
* Elemento 2
* Elemento 3

- Otra forma de crear el elemento 1
- Otra forma de crear el elemento 2

+ Y otra forma más para el elemento 1
+ Y otra forma más para el elemento 2
```

> **💡 Buena Práctica:** Aunque puedes usar cualquiera de los tres símbolos, lo ideal es elegir uno (generalmente el guion `-` o el asterisco `*`) y mantenerlo en todo el documento para que tu código fuente sea uniforme y predecible.

## 2. Listas Ordenadas (Numeradas)

Las listas ordenadas comienzan por un número seguido de un punto y un espacio. También admiten sub-listas.

**Sintaxis:**
```text
1. Primer elemento
2. Segundo elemento
3. Tercer elemento
```
> **🔥 Truco Pro:** En Markdown, no importa qué números escribas explícitamente, el motor siempre los renderizará en orden secuencial comenzando por el primer número. Es muy común escribir siempre `1.` en todos los elementos. Así, si luego añades o eliminas un elemento en medio de la lista, no tienes que reenumerar el resto a mano.

## 3. Listas Anidadas (Sub-listas)

Para anidar sub-listas indentamos los elementos con tabulación o cuatro espacios. Puedes combinar viñetas y números sin problema.

**Sintaxis:**
```text
1. Elemento principal 1
    1. Sub-elemento 1.1
    2. Sub-elemento 1.2
        1. Sub-sub-elemento 1.2.1
2. Elemento principal 2
    * Sub-elemento con viñeta
    * Otro sub-elemento con viñeta
        * Sub-sub-elemento con viñeta anidado
```