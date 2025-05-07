# 📘 Índice de la Guía Completa de HTML

## Tabla de Contenidos

- [📘 Índice de la Guía Completa de HTML](#-índice-de-la-guía-completa-de-html)
  - [Tabla de Contenidos](#tabla-de-contenidos)
- [🔰 Nivel 0 - Fundamentos](#-nivel-0---fundamentos)
  - [Tema 1: ¿Qué es HTML y cómo funciona?](#tema-1-qué-es-html-y-cómo-funciona)
    - [¿Cómo funciona?](#cómo-funciona)
    - [Etiquetas HTML asociadas a este tema](#etiquetas-html-asociadas-a-este-tema)
    - [Advertencias clave](#advertencias-clave)
  - [Tema 2: Estructura básica de un documento HTML](#tema-2-estructura-básica-de-un-documento-html)
    - [Etiquetas HTML asociadas a este tema](#etiquetas-html-asociadas-a-este-tema-1)
    - [Advertencias clave](#advertencias-clave-1)
  - [Tema 3: Etiquetas de texto (títulos, párrafos, saltos de línea, etc.)](#tema-3-etiquetas-de-texto-títulos-párrafos-saltos-de-línea-etc)
    - [Etiquetas HTML asociadas a este tema](#etiquetas-html-asociadas-a-este-tema-2)
    - [Advertencias clave](#advertencias-clave-2)
  - [Tema 4: Comentarios y espaciado en HTML](#tema-4-comentarios-y-espaciado-en-html)
    - [Etiquetas y elementos relacionados](#etiquetas-y-elementos-relacionados)
    - [Advertencias clave](#advertencias-clave-3)
  - [Tema 5: Atributos globales y estructura de una etiqueta](#tema-5-atributos-globales-y-estructura-de-una-etiqueta)
    - [Estructura de una etiqueta HTML](#estructura-de-una-etiqueta-html)
      - [Partes de una etiqueta](#partes-de-una-etiqueta)
    - [Atributos globales más comunes](#atributos-globales-más-comunes)
    - [Advertencias clave](#advertencias-clave-4)
- [🧱 Nivel 1 - Estructura y Organización](#-nivel-1---estructura-y-organización)
  - [Tema 6: Listas ordenadas, desordenadas y de definición](#tema-6-listas-ordenadas-desordenadas-y-de-definición)
    - [Etiquetas HTML asociadas a este tema](#etiquetas-html-asociadas-a-este-tema-3)
    - [Advertencias clave](#advertencias-clave-5)
  - [Tema 7: Etiquetas semánticas de sección](#tema-7-etiquetas-semánticas-de-sección)
    - [Etiquetas HTML asociadas a este tema](#etiquetas-html-asociadas-a-este-tema-4)



# 🔰 Nivel 0 - Fundamentos

## Tema 1: ¿Qué es HTML y cómo funciona?

HTML (HyperText Markup Language) es el lenguaje de marcado estándar de la web. Su función principal es dar forma y estructura al contenido que aparece en la web, como textos, imágenes, enlaces, formularios, etc.

### ¿Cómo funciona?

HTML funciona a través de **etiquetas** (tags) que el navegador interpreta para mostrar el contenido de manera estructurada. Estas etiquetas están encerradas entre signos de menor y mayor que (`< >`), y suelen tener una **etiqueta de apertura** (`<p>`) y una **etiqueta de cierre** (`</p>`), aunque algunas etiquetas son **autocontenidas** (como `<img>`).

Cuando escribes código HTML, estás diciendo al navegador:

> “Esto es un párrafo”, “esto es un título”, “esto es una imagen”, etc.

El navegador entonces **interpreta y renderiza** ese contenido en pantalla.

### Etiquetas HTML asociadas a este tema

En este tema introductorio, hay **dos etiquetas clave** que debes conocer:

1. `<html>`

   - **Uso**: Es la raíz de todo documento HTML. Contiene todo el contenido visible e invisible (metadatos).

   - **Atributos principales**:
     - `lang`: Define el idioma del contenido (ej. `lang="es"` para español).

2. `<!DOCTYPE html>`

   - **Uso**: No es una etiqueta HTML como tal, sino una **declaración obligatoria** que le dice al navegador que estamos usando HTML5, la versión moderna.

   - **Atributos**: No tiene atributos. Siempre se escribe como:

     ```html
     <!DOCTYPE html>
     ```

### Advertencias clave

- **Nunca olvides** `<!DOCTYPE html>`, ya que si no está, el navegador podría usar un "modo de compatibilidad" que no sigue las reglas modernas.

- Aunque el contenido visible no cambia sin `lang`, este atributo es **fundamental para la accesibilidad** y el SEO.

- Todo documento HTML debe comenzar con `<!DOCTYPE html>` seguido por una etiqueta `<html>`.


## Tema 2: Estructura básica de un documento HTML

La estructura básica de un archivo HTML sigue un orden estricto que define qué se muestra y cómo debe interpretarse la información. Esta estructura está compuesta por etiquetas clave, que organizan el contenido y los metadatos del sitio.

A continuación, se muestra la **estructura mínima recomendada en HTML5**:

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8" />
    <title>Mi primera página</title>
  </head>
  <body>
    <h1>¡Hola, mundo!</h1>
    <p>Bienvenido a tu primera página web.</p>
  </body>
</html>
```
Esta estructura tiene **tres grandes bloques**:

1. `<!DOCTYPE html>` → Declaración del tipo de documento (HTML5).
2. `<html>` → Raíz del documento.
3. `<head>` → Contiene metadatos (no visibles por el usuario).
4. `<body>` → Contiene todo el contenido visible de la página.

### Etiquetas HTML asociadas a este tema

1. `<html>`

   - **Uso**: Raíz de todo el documento.

   - **Atributos comunes**:
     - `lang`: idioma principal del contenido (`"es"`, `"en"`, etc.).

2. `<head>`

   - **Uso**: Contiene metadatos, enlaces a scripts y estilos, y configuraciones importantes del sitio.

   - **No tiene atributos comunes**, pero puede contener varias etiquetas importantes.

3. `<meta>`

   - **Uso**: Define metadatos como codificación de caracteres, descripción, palabras clave, etc.

   - **Atributos comunes**:
     - `charset`: define la codificación de caracteres (`UTF-8` es la más usada).
     - `name`: tipo de información (ej. `"description"`, `"keywords"`).
     - `content`: valor del metadato.

4. `<title>`

   - **Uso**: Define el título de la pestaña del navegador.

   - **Atributos**: no tiene atributos comunes.

5. `<body>`

   - **Uso**: Contiene el contenido visible del sitio (texto, imágenes, botones, etc.).

   - **Atributos comunes**:
     - `class`, `id`, `style`.

### Advertencias clave

- **Nunca pongas contenido visible dentro del** `<head>`: todo contenido visible debe ir en `<body>`.

- Usa siempre `<meta charset="UTF-8">` para evitar errores con acentos o caracteres especiales.

- La etiqueta `<title>` es **fundamental para SEO y usabilidad**: no la omitas.

- El orden correcto de etiquetas importa, especialmente en el `<head>`.


## Tema 3: Etiquetas de texto (títulos, párrafos, saltos de línea, etc.)

HTML proporciona un conjunto de etiquetas fundamentales para estructurar el contenido textual de una página. Estas etiquetas permiten dividir el contenido en títulos jerárquicos, párrafos, líneas separadas y comentarios. Esta estructura es esencial para la legibilidad, accesibilidad y SEO.

### Etiquetas HTML asociadas a este tema

A continuación, se detallan todas las etiquetas clave para estructurar texto:

1. **Títulos** ( `<h1>` a `<h6>` )

  - **Uso**: Representan títulos jerárquicos. `<h1>` es el más importante (solo debe usarse una vez por página), y `<h6>` el menos importante.

  - **Jerarquía**:

    ```html
    <h1>Título principal</h1>
    <h2>Subtítulo</h2>
    <h3>Subsección</h3>
    ...
    <h6>Detalle mínimo</h6>
    ```
  - **Atributos comunes**

    - `id`: para navegación o estilos específicos.
    - `class`: para aplicar estilos CSS.
    - `style`: estilos en línea (no recomendado).

2. **Párrafo** ( `<p>` )

  - **Uso**: Contiene bloques de texto. Representa ideas completas.

    ```html
    <p>Este es un párrafo de ejemplo.</p>
    ```
  - **Atributos comunes**

    - `id`: para navegación o estilos específicos.
    - `class`: para aplicar estilos CSS.
    - `style`: estilos en línea (no recomendado).

3. **Salto de línea** ( `<br>` )

- **Uso**: Inserta un salto de línea. No debe usarse para separar párrafos enteros.

```html
Línea 1<br>
Línea 2
```
- **Ojo**: Es una etiqueta autocontenida (no lleva cierre).
  
- **Atributos comunes**
  - `id`: para navegación o estilos específicos.
  - `class`: para aplicar estilos CSS.
  - `style`: estilos en línea (no recomendado).

4. **Línea horizontal** ( `<hr>` )

- **Uso**: Representa una separación temática (no visual decorativa).

```html
<p>Primera sección</p>
<hr>
<p>Segunda sección</p>
```
- **Atributos comunes**
  - `id`: para navegación o estilos específicos.
  - `class`: para aplicar estilos CSS.
  - `style`: estilos en línea (no recomendado).

5. **Comentarios** ( `<!-- comentario -->` )

- **Uso**: No visible al usuario. Sirve para dejar notas en el código.

```html
<!-- Este es un comentario -->
```
### Advertencias clave

- **No uses múltiples** `<h1>` en una sola página. Debe haber solo uno, representando el título principal.
- Usa `<br>` **solo** cuando realmente necesites un salto puntual. Para separar bloques usa `<p>` o CSS.
- No uses títulos solo para agrandar texto. Usa CSS para estilos y HTML para significado.
- Los comentarios no deben estar dentro de otras etiquetas (excepto en `<head>` o `<body>`).

## Tema 4: Comentarios y espaciado en HTML

En HTML, los comentarios y el espaciado no afectan directamente lo que se muestra en el navegador, pero son esenciales para la organización, legibilidad y mantenimiento del código.

- Los comentarios sirven para documentar partes del código que no deseas que se vean en la página.

- El espaciado en blanco (saltos de línea, sangrías y tabulaciones) no altera el resultado visual, pero hace que el código sea mucho más fácil de leer.

### Etiquetas y elementos relacionados

1. **Comentarios en HTML** ( `<!-- comentario -->` )

- **Uso**: Insertar anotaciones o descripciones invisibles al navegador y al usuario final.

```html
<!-- Este es un comentario -->
<p>Hola mundo</p>
```
- **Atributos**: No tiene atributos.

- **Advertencia**: Nunca uses `//` o `/* */` como en otros lenguajes. En HTML solo se usa `<!-- -->`.

2. Espaciado en blanco (espacios, tabulaciones, saltos de línea)

- **HTML ignora múltiples espacios, saltos de línea y tabulaciones.** Es decir:

```html
<p>Hola     mundo</p>
```
Se verá igual que:

```html
<p>Hola mundo</p>
```
- Para insertar **espacios adicionales intencionales**, se usa **la entidad HTML**:

  - `&nbsp;` → espacio no separable (*non-breaking space*)

```html
Hola&nbsp;&nbsp;&nbsp;mundo
```
- Para mostrar texto tal como fue escrito (con espacios y saltos de línea respetados), se puede usar la etiqueta `<pre>`:

```html
<pre>
Línea 1
  Línea 2 con espacio
</pre>
```
### Advertencias clave

- **Nunca pongas código HTML dentro** de los comentarios. Aunque algunos navegadores lo ignoren, puede causar errores inesperados.
- **No confíes en los comentarios** para ocultar información confidencial. El código fuente puede ser inspeccionado fácilmente por cualquier usuario.
- **Evita comentarios innecesarios o excesivos**; usa solo los que agregan claridad.
- Para separar visualmente partes del código, **usa líneas en comentarios**:

```html
<!-- ========= Sección de Contacto ========= -->
```

## Tema 5: Atributos globales y estructura de una etiqueta

En HTML, cada **etiqueta** sigue una estructura general:

```html
<!-- todo esto es llamado elemento -->
<etiqueta atributo="valor">Contenido</etiqueta>
```
Hay atributos que son específicos de una etiqueta, pero también existen atributos globales que pueden usarse en casi todas las etiquetas HTML. Estos atributos permiten dar identidad, estilo, contexto, accesibilidad y funcionalidad al contenido.

### Estructura de una etiqueta HTML

#### Partes de una etiqueta

```html
<p class="intro" id="parrafo1" style="color:red;">Hola</p>
```

1. `<p>` → **Etiqueta de apertura** (indica que comienza un párrafo)

2. `class="intro"` → Atributo global (clase CSS asociada)

3. `id="parrafo1"` → Atributo global (identificador único)

4. `style="color:red;"` → Atributo global (estilo en línea)

5. `Hola` → Contenido del elemento

6. `</p>` → **Etiqueta de cierre**

### Atributos globales más comunes

Estos atributos pueden aplicarse a **casi cualquier etiqueta** en HTML5:

| **Atributo**      | **Uso**                                                             |
| ----------------- | ------------------------------------------------------------------- |
| `id`              | Identificador único del elemento en el documento.                   |
| `class`           | Permite agrupar elementos con un nombre común. Se usa con CSS y JS. |
| `style`           | Define estilos en línea (color, tamaño, márgenes).                  |
| `title`           | Muestra un texto emergente al pasar el mouse.                       |
| `lang`            | Idioma del contenido del elemento (ej. `es`, `en`).                 |
| `hidden`          | Oculta el elemento visualmente.                                     |
| `tabindex`        | Controla el orden de navegación con el teclado.                     |
| `draggable`       | Define si el elemento puede ser arrastrado.                         |
| `contenteditable` | Permite editar el contenido directamente desde el navegador.        |
| `data-*`          | Define atributos personalizados para JS. Ej: `data-user="juan"`     |

### Advertencias clave

- Nunca repitas un mismo `id` en diferentes elementos del mismo documento.
- Evita abusar de `style`. Se recomienda usar CSS externo o interno.
- Usa `class` para agrupar estilos comunes; no pongas estilos directos si puedes evitarlo.
- Los atributos `data-*` no tienen efecto visual por sí solos, pero son útiles en JavaScript.
- `hidden` solo oculta visualmente, pero sigue existiendo en el DOM.


# 🧱 Nivel 1 - Estructura y Organización

## Tema 6: Listas ordenadas, desordenadas y de definición
Las **listas** en HTML permiten organizar contenido relacionado de forma estructurada. Existen tres tipos principales:

1. **Listas ordenadas** (`<ol>`): enumeran los ítems con números o letras.
2. **Listas desordenadas** (`<ul>`): enumeran los ítems con viñetas.
3. **Listas de definición** (`<dl>`): muestran pares de términos y descripciones.

### Etiquetas HTML asociadas a este tema

1. **Lista desordenada** ( `<ul>` )

- **Uso**: Lista de ítems sin orden específico (usualmente con viñetas).

- **Atributos comunes**:
  - `type` *(obsoleto)*: define el tipo de viñeta (circle, square, disc). Mejor usar CSS.
  - `class`, `id`, `style`.
  
```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```
2. **Lista ordenada** ( `<ol>` )

- **Uso**: Lista con ítems numerados (1, 2, 3...) o con letras.

- **Atributos comunes**:
  - `type`: tipo de marcador (`1`, `a`, `A`, `i`, `I`).
  - `start`: número inicial.
  - `reversed`: invierte el orden (de mayor a menor).

```html
<ol type="A" start="3">
  <li>Inicio</li>
  <li>Medio</li>
  <li>Fin</li>
</ol>
```

3. **Elemento de lista** ( `<li>` )

- **Uso**: Representa cada ítem dentro de `<ul>` o `<ol>`.

- **Atributos comunes**: `value` (sólo en `<ol>`, permite personalizar el número).

```html
<ol>
  <li value="10">Diez</li>
  <li>Once</li>
</ol>
```
4. **Lista de definición** ( `<dl>` )

- **Uso**: Lista de términos y definiciones ( pares término-descripción/pregunta-respuesta ).

- **Elementos relacionados**:
  - `<dt>`: término a definir.
  - `<dd>`: definición del término.

```html
<dl>
  <dt>HTML</dt>
  <dd>Lenguaje de marcado para la web.</dd>
  <dt>CSS</dt>
  <dd>Lenguaje de estilo para la web.</dd>
</dl>
```
### Advertencias clave

- **Nunca pongas texto suelto directamente dentro de** `<ul>` o `<ol>`. Siempre debe estar dentro de `<li>`.
- Evita abusar de listas solo por sangrar contenido. Usa listas solo si los elementos realmente son ítems.
- Para listas complejas (ej. con imágenes o botones dentro), sigue usando `<li>` para mantener la estructura semántica.
- `<ul>` y `<ol>` no deben mezclarse dentro de la misma jerarquía sin cerrar correctamente las etiquetas.
- Si solo tienes una lista de ítems sin una relación directa de término-descripción, usa `<ul>` (lista no ordenada) o `<ol>` (lista ordenada).
- siempre que tengas contenido que se organice naturalmente en pares donde un elemento define, describe o da valor a otro, la etiqueta `<dl>` junto con `<dt>` y `<dd>` es la elección semánticamente correcta

## Tema 7: Etiquetas semánticas de sección

HTML5 introdujo etiquetas semánticas que permiten describir claramente las distintas secciones de una página web. Estas etiquetas no solo organizan mejor el contenido, sino que también mejoran el SEO, la accesibilidad y la legibilidad del código.

En lugar de usar <div> para todo, estas etiquetas semánticas indican la función del contenido que contienen, lo cual ayuda tanto a los desarrolladores como a los motores de búsqueda.

### Etiquetas HTML asociadas a este tema

1. `<header>`

- **Uso:** Representa el encabezado de una página o sección. Puede contener logos, menús, títulos, etc.

- **Atributos comunes:** `class`, `id`, `style`

```html
<header>
  <h1>Mi sitio web</h1>
  <nav>...</nav>
</header>
```