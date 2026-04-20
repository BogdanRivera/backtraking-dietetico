# Backtracking Dietético

Planificador nutricional interactivo desarrollado en HTML, CSS y JavaScript que utiliza un algoritmo de **backtracking dinámico** para construir combinaciones de alimentos bajo distintas restricciones. El proyecto integra una visualización en tiempo real con `p5.js`, un catálogo de alimentos mexicanos y controles para ajustar variables como la glucosa y los minutos de ejercicio.

## Características principales

- Visualización del proceso de búsqueda en tiempo real.
- Catálogo de alimentos con calorías, categorías y restricciones.
- Ajuste interactivo de glucosa y ejercicio para modificar el comportamiento del algoritmo.
- Aplicación de restricciones nutricionales como sin gluten, sin lácteos y bajo índice glucémico.
- Inclusión de alimentos obligatorios dentro de las soluciones propuestas.
- Interfaz oscura, limpia y pensada para mostrar el proyecto de forma profesional.

## ¿Qué hace este proyecto?

El sistema evalúa alimentos disponibles y genera soluciones compatibles con las condiciones activas. A partir de los parámetros seleccionados por el usuario, el algoritmo filtra opciones, explora combinaciones y muestra resultados válidos en pantalla.

La lógica principal considera:

- un límite calórico dinámico calculado con base en el ejercicio;
- restricciones alimentarias activas según la glucosa;
- alimentos obligatorios que deben aparecer en la solución;
- categorías como desayuno, comida y alimentos de uso general.

## Tecnologías utilizadas

- HTML5
- CSS3
- JavaScript
- [p5.js](https://p5js.org/)

## Estructura general

- `index.html`: contiene la interfaz, el catálogo de alimentos, los controles y la lógica del simulador.
- `README.md`: documentación del proyecto.

## Cómo usarlo

1. Abre el archivo `index.html` en un navegador moderno.
2. Ajusta los controles de glucosa y minutos de ejercicio.
3. Presiona el botón de inicio para ejecutar la búsqueda.
4. Observa la visualización, el catálogo filtrado y las soluciones encontradas.

## Requisitos

- Navegador web moderno con soporte para JavaScript.
- Conexión a Internet para cargar `p5.js` desde CDN.

## Criterios del algoritmo

El proyecto aplica reglas que permiten simular decisiones nutricionales de forma clara:

- Si la glucosa es mayor o igual a 100, se activa la restricción de alto índice glucémico.
- Se excluyen alimentos con harina, lácteos y avena desde el filtro base.
- El límite calórico se calcula dinámicamente con la fórmula:

	`850 + (minutos de ejercicio × 5)`

- El resultado final debe incluir alimentos obligatorios como **Huevos a la Mex** y **Alambre de Res**.

## Propósito académico

Este proyecto es útil para demostrar cómo un algoritmo de búsqueda por backtracking puede aplicarse a un problema de selección de alimentos con restricciones, combinando lógica computacional, visualización e interacción de usuario en una sola interfaz.

## Créditos

Proyecto creado para fines educativos y de demostración visual del algoritmo de backtracking aplicado a nutrición.
