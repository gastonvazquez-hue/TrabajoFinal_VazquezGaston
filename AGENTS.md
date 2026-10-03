# Instrucciones para el Asistente

## Contexto del Proyecto
- Estoy trabajando en la comparación de curvas de crecimiento mediante modelos no lineales (nls) y modelos no lineales de efectos mixtos (nlme).
- El objetivo es comparar curvas de crecimeinto o sea es un estudio longitudinal entre dos tratamientos en dos temporadas  y la publicación de resultados.

## Convenciones de Código y Estilo
- Todo el código de R debe seguir estrictamente las guías de estilo de 'tidyverse'.
- Utiliza exclusivamente el operador de tubería nativo `|>`.
- Manejo de fechas: Usar siempre la librería `lubridate`.
- Modelado estadístico: Uso principal de los paquetes `nlme` (para `nlme` y `gnls`) y `emmeans` para comparaciones de post-hoc y estimación de medias marginales.
- Visualización: Uso de `ggplot2` con un diseño limpio (preferentemente `theme_minimal()`) y paletas de colores accesibles (como Viridis). Las animaciones se realizan con `gganimate`.
- Reportes: Trabajo estrictamente dentro del entorno **Quarto** (`.qmd`). Los chunks de código deben usar la sintaxis de opciones con `#|`.

## Robustez Estadística y Formato
- Si un modelo mixto no lineal tiene problemas de convergencia, sugiere ajustes en `nlmeControl` o el uso de `nlsList` para valores iniciales.
- Para exportar o mostrar tablas de resultados estadísticos en Quarto, utiliza `broom::tidy()` combinado con `gt` o `modelsummary`.

## Idioma y Tono de las Respuestas
- Respóndeme siempre en español.
- El tono debe ser claro, pedagógico, riguroso y orientado a un investigador universitario/científico. Explica el porqué de las decisiones estadísticas (ej. por qué elegir cierta estructura de correlación o varianza en `nlme`).