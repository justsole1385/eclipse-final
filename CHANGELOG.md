# Changelog

Este archivo proporciona una descripción conceptual y organizativa de las reglas de diseño a implementar en la hoja de estilos, 
detallando el propósito de cada sección sin duplicar el código técnico de los selectores, propiedades o valores.

El formato se basa en [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), y este proyecto cumple con [Versionado Semántico](https://semver.org/spec/v2.0.0.html).

---

## [1.0.0] - 2026-03-04

### Agregado

- Reinicia **todos los elementos del documento**. Configura `box-sizing: border-box` para que el ancho y alto incluyan el contenido, el relleno y el borde. Además, elimina los márgenes y rellenos predeterminados con `box-sizing: border-box` y `padding: 0`.

- Define el estilo base del **cuerpo de la página**. Usa una tipografía `Georgia, 'Times New Roman', serif` como fuente principal. Establece un fondo casi negro `#080808`, usa color del texto claro `#f2f2f2` y una altura de línea de `1.6` para mejorar la lectura.

## [1.1.0] - 2026-03-11

### Modificado

- Modifica el selector por clase `.logo`.
    - Estiliza el texto del logo con color dorado, con`color: #e2b450;`.

## [1.2.0] - 2026-03-18

### Modificado

- Modifica el selector por clase `.navbar`.
    - Como un contenedor flexible horizontal, con `display: flex;`.
    - Distribuye el espacio entre el logo y el menú, con `justify-content: space-between`.
    - Centra verticalmente los elementos y agrega espacio interno, con `align-items: center;`.

## [1.3.0] - 2026-03-25

### Modificado

- Modifica el selector por descendientes `.navbar a`.
    - Estiliza los enlaces del menú sin subrayado, con `text-decoration: none;`.
    - Con texto en negrita para mejorar su visibilidad, con `font-weight: bold;`.

## [1.4.0] - 2026-04-01

### Agregado

- Agrega el selector cuando el usuario pasa el cursor sobre los enlaces del menú, con `.navbar a:hover`
    - Cambia el color del texto de los enlaces a dorado (`#e2b450`), generando retroalimentación visual.

## [1.5.0] - 2026-04-08

### Modificado

- Modifica el selector por clase `.btn`.
    - Color dorado de fondo, con `background-color: #e2b450;`.
    - Establece un margen superior de 20 píxeles para separar el elemento de lo que tenga arriba. 
    - Añade un espacio interno o relleno de 14 píxeles en la parte superior e inferior, y de 30 píxeles en los lados izquierdo y derecho. 
    - Por último, redondea completamente las esquinas del elemento aplicando un radio de borde de 30 píxeles para darle un aspecto de botón o píldora.

### Agregado

- Agrega el selector cuando el usuario pasa el cursor sobre los elementos con la clase `.btn`
    - Color blanco de fondo, con `background-color: #ffffff;`.

## [1.6.0] - 2026-04-15

- Para el selector por clase `.section`, define el espaciado general con 70px arriba y abajo, y 8% a los lados.
