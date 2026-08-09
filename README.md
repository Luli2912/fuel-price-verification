# Verificación de Precios de Carburantes — Análisis Comparativo

Análisis comparativo de precios de carburantes en Santanyí (Islas Baleares), contrastando datos de campo (fuente primaria) con datos oficiales obtenidos vía API pública (fuente secundaria).

## Objetivo
Verificar la fiabilidad y actualización de precios publicados por estaciones de servicio (Repsol, Cepsa), cruzando evidencia fotográfica propia con los datos oficiales del Ministerio para la Transición Ecológica.

## Metodología
- **Recogida de datos de campo:** captura fotográfica de precios en tótems de estaciones de servicio
- **Obtención de datos oficiales:** consulta a la API REST de Precios de Carburantes del Ministerio, en formato JSON
- **ETL:** importación, limpieza y normalización de datos con Power Query (Excel) — corrección de formatos numéricos y mapeo de denominaciones comerciales vs oficiales
- **Análisis de variabilidad:** estudio de patrones de actualización de precios por operador, usando fuente adicional (Precioil)

## Resultados clave
- Se detectaron diferencias de hasta 0.02€/L entre los datos de campo y los datos actuales, explicadas por el patrón de actualización horaria de cada operador
- REPSOL actualiza precios por la noche (~21:15); CEPSA de madrugada (~00:15)
- La estandarización de denominaciones oficiales permite detectar variaciones mínimas de precio que pasarían desapercibidas bajo nombres comerciales

## Herramientas
Excel (Power Query) · API REST · JSON

## Contexto académico
Proyecto desarrollado para la asignatura *Captura y Preparación de Datos* — Grado en Ciencia de Datos e IA, VIU.
