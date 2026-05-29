# Evaluación de Diseño Responsivo y Rejillas CSS

---

Analice las siguientes reglas CSS

```css

.personajes-grid {
    grid-template-columns: repeat(3, 1fr);
}

.reparto-grid {
    grid-template-columns: repeat(4, 1fr);
}

.opiniones-grid {
    grid-template-columns: repeat(3, 1fr);
}

@media (max-width: 900px) {

    .personajes-grid,
    .reparto-grid,
    .opiniones-grid {
        grid-template-columns: 1fr 1fr;
    }

    .hero-content h1 {
        font-size: 3.5rem;
    }

    .navbar {
        flex-direction: column;
        gap: 15px;
    }
}

@media (max-width: 600px) {

    .personajes-grid,
    .reparto-grid,
    .opiniones-grid {
        grid-template-columns: 1fr;
    }

    .navbar ul {
        flex-direction: column;
        text-align: center;
    }

    .hero-content h1 {
        font-size: 2.5rem;
    }

    .section {
        padding: 50px 5%;
    }
}
```

Identifique:

* ¿Cuántas columnas utiliza la página se muestra en un monitor de escritorio?

En un monitor de escritorio, las rejillas usan la distribución base definida antes de las media queries. La sección de personajes utiliza 3 columnas con .personajes-grid. La sección de reparto utiliza 4 columnas con .reparto-grid. La sección de opiniones utiliza 3 columnas con .opiniones-grid.

* ¿Qué ocurre cuando el ancho de pantalla es menor a 900px?

Cuando la pantalla es menor a 900px, las rejillas de personajes, reparto y opiniones cambian a 2 columnas. El título principal .hero-content h1 reduce su tamaño a 3.5rem. La barra de navegación .navbar cambia su dirección a columna. Además, se agrega una separación de 15px entre los elementos del menú.

* ¿Qué ocurre cuando el ancho de pantalla es menor a 600px?

Cuando la pantalla es menor a 600px, las rejillas cambian a una sola columna. Esto permite que los elementos se muestren uno debajo de otro en pantallas pequeñas. El menú de navegación también se organiza verticalmente y centra su texto. Además, el título principal baja a 2.5rem y las secciones reducen su padding a 50px 5%