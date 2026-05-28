# Planificación de Estilos CSS

---

## Mapeo de instrucciones técnicas, elementos HTML y reglas CSS

Mapee cada instrucción técnica con el elemento HTML afectado y la regla CSS que debe implementarse en el archivo `stylesheets/style.css`.

| Versión | Fecha | Instrucción del CHANGELOG.md | Elemento HTML en `index.html` | Selector CSS | Propiedad CSS principal |
|---------|-------|------------------------------|-------------------------------|:------------:|:------------------------:|
| [1.0.0] | 2026-03-04 | Reinicia todos los elementos del documento aplicando `box-sizing: border-box`, eliminando márgenes y rellenos predeterminados. | Todos los elementos HTML del documento. | `*` | `box-sizing`, `margin`, `padding` |
| [1.0.0] | 2026-03-04 | Define el estilo base del cuerpo de la página: tipografía, color de fondo, color de texto y altura de línea. | Elemento `<body>`. | `body` | `font-family`, `background-color`, `color`, `line-height` |
| [1.1.0] | 2026-03-11 | Modifica el selector `.logo` para aplicar color dorado al texto. | `<h2 class="logo">Eclipse Final</h2>`. | `.logo` | `color` |
| [1.2.0] | 2026-03-18 | Modifica el selector `.navbar` para convertirlo en un contenedor flexible horizontal, distribuir el espacio entre el logo y el menú, centrar elementos y agregar espacio interno. | `<nav class="navbar">`, que contiene el logo y la lista de enlaces. | `.navbar` | `display`, `justify-content`, `align-items`, `padding` |
| [1.3.0] | 2026-03-25 | Modifica el selector descendiente `.navbar a` para quitar el subrayado de los enlaces y aplicar texto en negrita. | Enlaces del menú dentro de `<nav class="navbar">`. | `.navbar a` | `text-decoration`, `font-weight` |
| [1.4.0] | 2026-04-01 | Agrega el selector `.navbar a:hover` para cambiar el color de los enlaces a dorado cuando el usuario pase el cursor. | Enlaces `<a>` dentro de la barra de navegación. | `.navbar a:hover` | `color` |
| [1.5.0] | 2026-04-08 | Modifica el selector `.btn` para aplicar fondo dorado, margen superior, relleno interno y bordes redondeados. | `<a href="#trailer" class="btn">Ver trailer</a>`. | `.btn` | `background-color`, `margin-top`, `padding`, `border-radius` |
| [1.5.0] | 2026-04-08 | Agrega el selector `.btn:hover` para cambiar el fondo del botón a blanco cuando el usuario pase el cursor. | Enlace con clase `.btn`. | `.btn:hover` | `background-color` |
| [1.6.0] | 2026-04-15 | Modifica el selector `.section` para definir espaciado general arriba, abajo y a los lados. | Secciones con clase `.section`: Trailer, Sinopsis, Personajes, Reparto y Opiniones. | `.section` | `padding` |

---

# Estructura y Organización del Archivo CSS

En esta sección se describe cómo estará organizado el archivo `stylesheets/style.css` para mantener claridad, orden y facilidad de mantenimiento del código.

La hoja de estilos se organizará por bloques de componentes y secciones del sitio web. Cada grupo de reglas tendrá un comentario descriptivo para identificar rápidamente su propósito dentro del archivo.

## Organización sugerida de CSS


/* Reset y estilos globales */
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: Georgia, 'Times New Roman', serif;
    background-color: #080808;
    color: #f2f2f2;
    line-height: 1.6;
}

/* Portada principal */
.hero {
    min-height: 100vh;
}

/* Navegación */
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    color: #e2b450;
}

.navbar a {
    text-decoration: none;
    font-weight: bold;
}

.navbar a:hover {
    color: #e2b450;
}

/* Contenido de portada */
.hero-content {
    text-align: center;
}

/* Botones */
.btn {
    background-color: #e2b450;
    margin-top: 20px;
    padding: 14px 30px;
    border-radius: 30px;
}

.btn:hover {
    background-color: #ffffff;
}

/* Secciones generales */
.section {
    padding: 70px 8%;
}

/* Multimedia */
.video-container {
    max-width: 900px;
}

/* Grillas y tarjetas */
.grid {
    display: grid;
}

.card {
    border-radius: 15px;
}

/* Sección de reparto */
.actor {
    padding: 25px;
}

/* Sección de opiniones */
.opinion {
    padding: 30px;
}

/* Pie del sitio */
footer {
    text-align: center;
}
```

---

## Estrategia de Nomenclatura CSS

La siguiente tabla define la convención de nombres que se utilizará para las clases y componentes CSS del proyecto, con el propósito de mantener consistencia, claridad y facilidad de mantenimiento del código.

| Regla General | Descripción | Ejemplo Correcto | Ejemplo Incorrecto |
| :------------ | :---------- | :--------------: | :----------------: |
| **Utilizar kebab-case** | Separar palabras con guiones medios y usar letras minúsculas. | `.video-container` | `.videoContainer` |
| **Mantener consistencia en el idioma** | Utilizar un solo idioma para todas las clases CSS del proyecto. En este caso, se mantendrán los nombres existentes del proyecto. | `.hero-content` | `.contenidoHero` |
| **Utilizar nombres descriptivos** | Las clases deben indicar claramente la función o propósito visual del componente. | `.personajes-grid` | `.caja1` |
| **Evitar nombres ambiguos** | No utilizar nombres genéricos o poco claros que no expliquen el uso del elemento. | `.opiniones-grid` | `.bloque` |
| **Mantener nombres reutilizables** | Crear clases que puedan reutilizarse en distintos componentes sin depender de una sola sección. | `.section` | `.seccion-solo-trailer` |
| **Evitar abreviaciones innecesarias** | Usar nombres completos y comprensibles para facilitar el mantenimiento. | `.video-container` | `.vid-cont` |