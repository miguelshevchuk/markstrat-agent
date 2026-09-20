# Producción — Período 01

## Inventario del período anterior — datos EXACTOS del simulador (P0)

| Marca | Plan P0 (decisión) | Producción real P0 | Ventas P0 | Inventario final P0 |
|-------|-------------------|-------------------|-----------|---------------------|
| MOST  | 150,000 u         | **141,419 u**     | 141,419 u | **0 u** |
| MOVE  | 120,000 u         | **96,000 u**      | 43,841 u  | **52,159 u** |

## Decisiones de producción Ronda 1

| Marca | Inventario inicial R1 | Producción decidida | Stock disponible | Ventas esperadas | Inventario proyectado |
|-------|-----------------------|--------------------|--------------------|-----------------|----------------------|
| MOST  | 0                     | **200,000 u**       | 200,000 u          | ?               | ? |
| MOVE  | 52,159                | **10,000 u**        | 62,159 u disponibles | ?             | ? |

## Restricciones y advertencias

- 🔴 **MOST 200k vs. 141k producidos en P0 = +41.7%**: supera el ±20% automático.
  - Costo de ajuste de capacidad garantizado.
  - Justificación: bajada de precio a $182 debe generar mucho más demanda en Gen-Z.

- 🔴 **MOVE 10k vs. 96k producidos en P0 = −89.6%**: supera ENORMEMENTE el −20% automático.
  - También genera costo de ajuste de capacidad (en este caso, reducción de capacidad).
  - Ambas marcas tienen costo de ajuste en R1 — impacto financiero doble.
  - Costo de inventario sobrante: 8% del Transfer Cost por año = $120 × 8% = $9.6/u/año.
  - Si quedan 30k sin vender: costo adicional ≈ $288,000.

## Razonamiento de producción

**MOST:** La apuesta es fuerte — bajamos precio a $182 para disparar volumen en Gen-Z. Con el mercado Gen-Z de 261k unidades y un 43% de share, MOST vende ~112k en ese segmento. Si el precio bajo atrae más compradores Gen-Z y algunos Millennials, 200k puede ser alcanzable. Riesgo: si la demanda no acompaña, tendremos inventario de unidades a precio de producción $69/u.

**MOVE:** Decisión conservadora para no acumular más inventario. Con 62k disponibles, necesitamos que los Millennials las compren. El precio $390 sigue siendo alto para el segmento (que es más sensible al precio que los Profesionales). Análisis post-ronda: ver si tiene sentido bajar más el precio en R2 para liquidar y luego reformular.
