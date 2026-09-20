# Reglas de la Simulación

## Entorno económico
- **Inflación:** 2% anual
- **Crecimiento del PIB:** 4% anual

## Producción
- Se puede ajustar ±20% automáticamente respecto al período anterior sin costo adicional
- El inventario sobrante genera **costos de almacenamiento**
- Inventario no vendido pasa al siguiente período
- Si la demanda supera la producción, se pierde venta (stockout)
- El **transfer cost** comienza igual al base cost; puede bajar con proyectos I+D exitosos

## Precios
- El precio recomendado al consumidor es orientativo; los canales aplican sus márgenes
- Precio al distribuidor = Retail price / (1 + margen del canal)

## Fuerza de ventas
- Contratar o despedir vendedores tiene **costos de transición** y **demora de 1 período**
- La asignación de vendedores por canal afecta la distribución ponderada

## I+D
- Los proyectos I+D llevan al menos **1 período** en completarse
- Un proyecto exitoso puede lanzarse en el siguiente período
- El nombre del proyecto empieza con "P" (ej: P-TONIC2)
- La especificación debe estar dentro de los rangos válidos de atributos

## Vodites
- El mercado Vodite **no existe desde el inicio**; se crea cuando alguna empresa lanza el primer Vodite
- Segmentos Vodite: Innovadores → Pioneros → Seguidores (adopción secuencial)

## Estudios de mercado
- Se solicitan **antes** del período; los resultados llegan con el informe anual
- Hay 14 tipos disponibles en esta simulación; elegir estratégicamente según decisiones pendientes

## Inventario — Costos de cargar stock entre períodos

```
Costo de almacenamiento = Inventario final × Transfer Cost × 8% por año

Eliminación forzada de inventario = Inventario a eliminar × Transfer Cost × 20%
```

**Ejemplos con datos reales:**

| Marca | Transfer Cost | Unidades inventario | Costo anual de cargarlo |
|-------|--------------|--------------------|-----------------------|
| MOST  | $69/u        | 0 (P0 cerró limpio) | $0 |
| MOVE  | $120/u       | **52,000 u**       | **$499,200/año** ⚠️ |

> Si en R1 MOVE vende solo 30k de las 62k disponibles → 32k unidades sobrantes → costo de inventario R1: 32,000 × $120 × 8% = **$307,200**

> Si se decide **eliminar** el inventario de MOVE en vez de venderlo: 52,000 × $120 × 20% = **$1,248,000** (costo único)

**Regla práctica:** Cargar inventario es más barato que eliminarlo, pero si el producto no tiene demanda futura (por quedar obsoleto o mal posicionado), conviene eliminar para liberar cash.

## Empresas competidoras
- **5 empresas** en esta industria (Albatross): L, M, R, S, T
- Cada empresa comienza con 2 marcas Sonite
- Convención de nombres — Sonites: [Letra]O[xxx] | Vodites: [Letra]E[xxx]
- **No existe empresa N** en esta industria
