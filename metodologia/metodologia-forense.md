# Metodología Forense

## Enfoque general

El proyecto aplica **metodología forense financiera** al análisis macroprudencial del sistema bancario peruano. A diferencia de un análisis descriptivo tradicional, el enfoque forense parte de una pregunta de investigación por eje y busca **aislar anomalías estructurales** —valores que no responden a dinámica de mercado natural— mediante control estadístico y análisis de concentración.

## Proceso de 7 fases

1. **Recolección** — Extracción de datos públicos de BCRPData y del Balance de Comprobación mensual de la SBS (2018–2025).
2. **Normalización** — Homogeneización de series por institución, moneda (MN/ME) y periodo.
3. **Establecimiento de línea base** — Definición del comportamiento esperado del sistema en condiciones normales.
4. **Detección de anomalías** — Aplicación de **bandas de control estadístico a ±2σ** para identificar valores atípicos.
5. **Análisis de concentración** — Cálculo del **índice HHI** por mercado y moneda, contrastado contra el umbral de referencia DOJ/FTC de 2.500 puntos.
6. **Análisis causal** — Cruce de las anomalías detectadas con eventos exógenos (p. ej., Reactiva Perú) y políticas regulatorias (encaje diferenciado BCRP).
7. **Conclusiones forenses** — Formulación de hallazgos de primer orden y de implicancias regulatorias.

## Instrumentos estadísticos

- **Bandas de control ±2σ.** Cualquier observación fuera de dos desviaciones estándar de la media histórica se marca como anomalía candidata a análisis causal.
- **Índice Herfindahl-Hirschman (HHI).** Medida de concentración de mercado. Umbrales de referencia: <1.500 desconcentrado, 1.500–2.500 moderadamente concentrado, >2.500 altamente concentrado.
- **Análisis de regresión.** Se evalúa la relación entre crecimiento de activos y desconcentración, controlando por el ciclo artificial de Reactiva Perú.

## Convenciones del proyecto

- **Par de referencia comparativo: 2018 vs. 2024.** Se excluye 2025 de las tablas comparativas porque el año solo corre hasta septiembre.
- **Separación MN / ME.** Todo el análisis distingue moneda nacional de moneda extranjera, ya que la asimetría entre ambas es un hallazgo central.
- **Cuatro ejes analíticos:** Tamaño, Estructura de Mercado, Concentración y Dinámica Competitiva.

## Fuentes

- **BCRPData** — Banco Central de Reserva del Perú.
- **SBS** — Superintendencia de Banca, Seguros y AFP (Balance de Comprobación mensual).
