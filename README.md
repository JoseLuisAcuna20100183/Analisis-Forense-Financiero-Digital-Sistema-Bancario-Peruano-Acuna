<h1 align="center">Análisis Forense Financiero Digital del Sistema Bancario Peruano</h1>
<p align="center"><i>Huellas en el Balance · 2018–2025</i></p>

<p align="center">
  <img src="https://img.shields.io/badge/Tipo-Investigaci%C3%B3n%20Forense%20Financiera-1a2b4a">
  <img src="https://img.shields.io/badge/Fuente-BCRPData%20%C2%B7%20SBS-c9a227">
  <img src="https://img.shields.io/badge/Periodo-2018--2025-444">
  <img src="https://img.shields.io/badge/Licencia-CC%20BY%204.0-green">
</p>

<p align="center">
  <b>
  📄 <a href="https://joseluisacuna20100183.github.io/Analisis-Forense-Financiero-Digital-Sistema-Bancario-Peruano-Acuna/">Paper en vivo</a> ·
  📊 <a href="https://app.powerbi.com/view?r=eyJrIjoiNzEwZDczMjctODdjNC00NzYyLWEzZTgtNWUxYWI3MzgzMGVmIiwidCI6Ijc1MDRlMzE4LThlMWUtNGQ1NS1iZmZkLTg3NWI0ZGVlODI2MCIsImMiOjR9&pageName=052e735fae12a0a7e0a8">Dashboard interactivo</a> ·
  🖥️ <a href="https://fibs-studio.ai.studio/">FIBS (app en vivo)</a> ·
  📑 <a href="presentacion/">Deck</a>
  </b>
</p>

---

## Resumen ejecutivo

En 2021, el sistema bancario peruano registró un crecimiento de activos de **+44.93% interanual** — una cifra que no responde a dinámica de mercado, sino a una inyección exógena de liquidez estatal a través del programa **Reactiva Perú**. Este proyecto aplica **metodología forense financiera** al balance del sistema bancario peruano para aislar ese tipo de anomalías estructurales, usando exclusivamente **datos públicos** de BCRPData y SBS (Balance de Comprobación mensual) para el periodo **2018–2025**.

El análisis se organiza en cuatro ejes —**Tamaño, Estructura de Mercado, Concentración y Dinámica Competitiva**— y se materializa en cuatro entregables: un **paper técnico**, un **dashboard interactivo en Power BI**, una **herramienta de simulación forense (FIBS)** y un **deck de exposición**.

---

## Hallazgos clave

- **Shock exógeno 2021.** El +44.93% interanual de activos coincide con el desembolso de Reactiva Perú, no con crecimiento orgánico del sistema.
- **Oligopolio estructural.** El índice **HHI se mantiene por encima de 3.000 puntos** en ambos mercados (MN y ME), superando de forma sostenida el umbral de **2.500 puntos** que el DOJ/FTC clasifica como mercado altamente concentrado.
- **Asimetría MN/ME persistente.** La Banca Grande concentra sistemáticamente más cuota en moneda extranjera que en moneda nacional, sosteniendo **más del 80% del TOSE ME** a lo largo del periodo.
- **Dinámica competitiva desigual.** El reparto de Reactiva Perú fue heterogéneo: **Interbank** emerge como principal beneficiario en cuota de mercado (**+2.1pp**), mientras **Scotiabank** documenta el mayor retiro estratégico.
- **Crecimiento orgánico no desconcentra.** Tras remover el ciclo artificial de Reactiva, la relación entre crecimiento y desconcentración es débil (**R² genuino ≈ 0.15–0.25**), evidencia de que el sistema no se desconcentra por dinámica propia.
- **Subsistema dolarizado paralelo.** Se identifica un bloque de banca dolarizada de nicho (ICBC, Bank of China, BCI Perú) con comportamiento diferenciado del resto del sistema.

> Las capturas del dashboard que ilustran cada hallazgo están en [`dashboard/capturas/`](dashboard/capturas/).

---

## Metodología

El proyecto sigue un **proceso forense de 7 fases**, con **bandas de control estadístico a ±2σ** para detectar valores atípicos y **análisis de concentración HHI** por mercado y moneda. La comparación de referencia es **2018 vs. 2024** (se excluye 2025 de las tablas comparativas porque el año solo corre hasta septiembre).

Detalle completo en [`metodologia/metodologia-forense.md`](metodologia/metodologia-forense.md).

---

## Entregables

| Entregable | Descripción | Ubicación |
|---|---|---|
| **📄 Paper técnico** | Informe forense completo con diseño institucional, 4 ejes analíticos, preguntas forenses y conclusiones de primer orden. [Leer en vivo](https://joseluisacuna20100183.github.io/Analisis-Forense-Financiero-Digital-Sistema-Bancario-Peruano-Acuna/). | [`paper/`](paper/) |
| **📊 Dashboard Power BI** | 5 páginas interactivas: Tamaño, Estructura, Concentración, Dinámica Competitiva y Asimetría Regulatoria. [Ver en vivo](https://app.powerbi.com/view?r=eyJrIjoiNzEwZDczMjctODdjNC00NzYyLWEzZTgtNWUxYWI3MzgzMGVmIiwidCI6Ijc1MDRlMzE4LThlMWUtNGQ1NS1iZmZkLTg3NWI0ZGVlODI2MCIsImMiOjR9&pageName=052e735fae12a0a7e0a8). | [`dashboard/`](dashboard/) |
| **🖥️ FIBS** | *Forensics Intelligence Banking System* — herramienta de simulación y stress-testing forense. [App en vivo](https://fibs-studio.ai.studio/). | [Repositorio FIBS →](https://github.com/JoseLuisAcuna20100183/FIBS-Forensics-Intelligence-Banking-System-Acuna) |
| **📑 Deck de exposición** | Versión LinkedIn (13 slides) y versión concurso (6 slides). | [`presentacion/`](presentacion/) |

---

## Fuente de datos

Todos los datos provienen de fuentes **públicas y oficiales**:

- **BCRPData** — Banco Central de Reserva del Perú (fuente primaria).
- **SBS** — Superintendencia de Banca, Seguros y AFP: Balance de Comprobación mensual.

No se utiliza ningún dato confidencial, propietario ni de acceso restringido. Diccionario de tablas y detalle en [`data/README.md`](data/README.md).

---

## Estructura del repositorio

```
.
├── paper/            → Paper HTML + PDF
├── dashboard/        → Capturas de las 5 páginas + archivo .pbix (o enlace)
├── presentacion/     → Decks (LinkedIn 13 slides / concurso 6 slides)
├── metodologia/      → Proceso forense de 7 fases, ±2σ, HHI
└── data/             → Datasets BCRPData/SBS + diccionario
```

---

## Aviso legal

Este es un trabajo de investigación académica desarrollado bajo el marco de **IISE – Data Analytics & Financial Forensics**. Las conclusiones son de carácter analítico y no constituyen asesoría financiera, legal ni de inversión. Los hallazgos se basan en datos públicos y en interpretaciones metodológicas propias del autor.

## Autoría

**José Luis Acuña León** — *IISE, Data Analytics & Financial Forensics*
[LinkedIn](https://www.linkedin.com/in/jose-luis-acuna) · [GitHub](https://github.com/JoseLuisAcuna20100183)

## Licencia

Contenido bajo [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE). Puedes compartir y adaptar el material dando crédito apropiado.
