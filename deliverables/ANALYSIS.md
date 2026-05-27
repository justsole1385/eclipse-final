# Análisis de Requerimientos

---

## Mapeo de intrucciones técnicas y elementos html

Tabla con el mapeo de las instrucciones técnica del CHANGELOG.md con los elementos del `index.html`.

| Versión |   Fecha    |       Instrucción del CHANGELOG.md         | Elemento HTML en `index.html` | 
|---------|------------|--------------------------------------------|-------------------------------|
| [1.0.0] | 2026-03-04 | Reinicia todos los elementos del documento.|   Todos los elementos HTML    |
| [1.0.0] | 2026-03-04 | Define el estilo base del cuerpo de la página | Elemento `<body>`. |
| [1.1.0] | 2026-03-11 | Modifica el selector `.logo` para aplicar color dorado al texto. | `<h2 class="logo">Eclipse Final</h2>`. |
| [1.2.0] | 2026-03-18 | Modifica el selector `.navbar` para convertirlo en un contenedor flexible horizontal. | `<nav class="navbar">`. |
| [1.3.0] | 2026-03-25 | Modifica el selector descendiente `.navbar a` para quitar el subrayado de los enlaces y aplicar texto en negrita. | Los enlaces dentro de `<nav class="navbar">`. |
| [1.4.0] | 2026-04-01 | Agrega el selector `.navbar a:hover` para cambiar el color de los enlaces a dorado cuando el usuario pase el cursor. | Los enlaces `<a>` dentro de la barra de navegación. |
| [1.5.0] | 2026-04-08 | Modifica el selector `.btn` para aplicar fondo dorado, margen superior, relleno interno y bordes redondeados. | `<a href="#trailer" class="btn">Ver trailer</a>`. |
| [1.5.0] | 2026-04-08 | Agrega el selector `.btn:hover` para cambiar el fondo del botón a blanco cuando el usuario pase el cursor. | El enlace con clase `.btn`: `<a href="#trailer" class="btn">Ver trailer</a>`. |
| [1.6.0] | 2026-04-15 | Modifica el selector `.section` para definir espaciado general arriba, abajo, y a los lados. | Las secciones con clase `.section`: `<section id="trailer" class="section">`, `<section id="sinopsis" class="section sinopsis">`, etc. |
