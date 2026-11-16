# Datos

## Fuente

Todos los datos de esta carpeta provienen de fuentes **públicas y oficiales**:

- **BCRPData** — Banco Central de Reserva del Perú (fuente primaria).
- **SBS** — Superintendencia de Banca, Seguros y AFP: Balance de Comprobación mensual.

**Periodo:** 2018–2025 (2025 disponible hasta septiembre).
**Frecuencia:** mensual.
**Cobertura:** empresas bancarias y empresas financieras del sistema peruano.

No se incluye ningún dato confidencial, propietario o de acceso restringido.

## Archivos de esta carpeta

| Archivo | Contenido |
|---|---|
| **`Datasets_BCRPData_SBS_consolidado.xlsx`** | Libro único con **una hoja por dataset** (21 datasets) más una hoja **Índice** que mapea cada hoja a su archivo original, código de serie y descripción. Es el archivo recomendado para explorar los datos. |
| **`BCRPData_SBS_originales.zip`** | Los **21 archivos `.xlsx` originales** tal cual se exportaron de BCRPData, con su estructura completa (hoja `Metadatos` + hojas de datos). Para quien quiera la fuente sin procesar. |

> El consolidado omite las hojas-fragmento redundantes (`_p1`, `_p2`, …) que algunos
> archivos originales traían partidas; conserva la serie completa de cada dataset.

## Datasets incluidos

Los 21 datasets cubren crédito al sector privado (MN y ME), encaje de las empresas bancarias (MN, ME y promedios diarios), encaje/depósitos overnight y liquidez por institución (bancarias y financieras, MN y ME), cuentas monetarias, indicadores bancarios, liquidez del sistema y tipo de cambio. El detalle completo con códigos de serie está en la hoja **Índice** del consolidado.

## Notas de uso

- Las series se normalizaron por institución, moneda y periodo antes del análisis.
- Los cálculos de HHI, bandas ±2σ y regresiones se documentan en
  [`../metodologia/metodologia-forense.md`](../metodologia/metodologia-forense.md).
- Convención comparativa: **2018 vs. 2024** (2025 excluido de tablas comparativas).
