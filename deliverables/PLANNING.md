# Planificación Técnica de Estilos CSS

---

# 📌 Identificación de Selectores CSS a Modificar

En esta sección se deberán registrar los selectores CSS que serán intervenidos durante el mantenimiento visual del sitio web.  
El objetivo es identificar claramente qué componentes del archivo `index.html` requieren modificaciones visuales y qué selectores CSS se utilizarán para aplicar dichos cambios.

## Aspectos a identificar

- Selectores de clases (`.class`)
- Selectores de identificadores (`#id`)
- Etiquetas HTML afectadas
- Componentes reutilizables
- Estados visuales (`:hover`, `:focus`, etc.)

## Ejemplo

| Elemento HTML | Selector CSS | Cambio requerido |
|---|---|---|
| `<header>` | `.header` | Cambiar color de fondo |
| Botón principal | `.btn-primary` | Bordes redondeados |
| Tarjetas | `.card` | Agregar sombra |

---

# 🗂 Estructura y Organización del Archivo CSS

En esta sección se describirá cómo estará organizado el archivo `styles.css` para mantener claridad, orden y facilidad de mantenimiento del código.

## Organización sugerida

```css
/* Reset y estilos globales */

/* Tipografía */

/* Layout principal */

/* Navegación */

/* Componentes */

/* Botones */

/* Tarjetas */

/* Footer */

/* Responsive Design */
```

## Aspectos a considerar

- Separación lógica de estilos
- Uso de comentarios descriptivos
- Agrupación de componentes relacionados
- Orden jerárquico de reglas CSS
- Facilidad de lectura y mantenimiento

---

# 🏷 Estrategia de Nomenclatura CSS

En esta sección se definirá la convención de nombres que se utilizará para clases y componentes CSS, con el fin de mantener consistencia y claridad en el proyecto.

## Recomendaciones

- Utilizar nombres descriptivos
- Evitar nombres ambiguos
- Mantener consistencia en el idioma
- Utilizar kebab-case

## Ejemplos

| Correcto | Incorrecto |
|---|---|
| `.main-header` | `.header1` |
| `.product-card` | `.box-red` |
| `.btn-primary` | `.button-new` |

## Convención sugerida

```css
.section-name
.card-product
.btn-primary
.footer-links
```

---

# ♻ Identificación de Estilos Reutilizables

En esta sección se identificarán estilos que puedan reutilizarse en distintos componentes del sitio web para optimizar el código CSS y evitar duplicación innecesaria.

## Aspectos a analizar

- Colores repetidos
- Botones similares
- Espaciados comunes
- Tipografías reutilizables
- Sombras y bordes consistentes

## Ejemplo de reutilización

```css
.btn {
  padding: 10px 20px;
  border-radius: 8px;
  font-weight: bold;
}

.btn-primary {
  background-color: #3498db;
  color: white;
}

.btn-secondary {
  background-color: #2ecc71;
  color: white;
}
```

## Beneficios

- Código más limpio
- Mayor facilidad de mantenimiento
- Consistencia visual
- Reducción de redundancia
- Mejor escalabilidad del proyecto

