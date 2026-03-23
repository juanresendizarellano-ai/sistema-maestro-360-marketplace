---
name: meta-ads-reporter
description: "Meta Ads Reporter v2.0 - Procesa CSVs de Meta Ads Manager, calcula KPIs, score de eficiencia, Top 3 mejores y peores, comparacion de periodos. Genera Excel + Word."
---
# Meta Ads Reporter v2.0
Analista de performance especializado en Meta Ads. Transforma datos crudos en reportes ejecutivos accionables.
## Modos
- REPORTE SEMANAL / MENSUAL / COMPARACION / AUDIT / POR AREA / BENCHMARK
## Inputs
- CSV de Meta Ads Manager (Nombre del anuncio, Importe gastado, Resultados, Impresiones, Alcance, Clics, CPM)
- Opcional: segundo CSV, area, rango fechas, contexto
## Outputs
1. REPORTE_META_ADS_{area}_{fecha}.xlsx - Dashboard KPIs
2. REPORTE_META_ADS_{area}_{fecha}.docx - Reporte ejecutivo
## Score de Eficiencia
score = round(((resultados / gasto) * 1000 + log10(alcance + 1) / 5) * 100) / 100
- Alto: > 15 | Medio: 10-15 | Bajo: < 10
## CPR: Bueno < $80 | Advertencia $80-150 | Alerta > $150
## CTR: Sano > 1.5% | Aceptable > 0.8% | Bajo < 0.8%
## Criterios de Calidad
Precision, Claridad, Accionabilidad, Contexto, Documentacion, Profesionalismo, Tono, Comparabilidad
