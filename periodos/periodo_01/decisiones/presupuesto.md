# Presupuesto y Finanzas — Período 01

## ¿De dónde sale el dinero para gastar?

En Markstrat, el presupuesto disponible para decisiones de marketing proviene de la **contribución neta del período anterior** (ingresos - costos de producción - gastos ya comprometidos). Si gastas más de lo que generas, el simulador puede aplicar penalidades o restricciones.

```
Presupuesto disponible ≈ Contribución Neta del período anterior
                        (neta de publicidad, SF, I+D y estudios ya gastados)
```

---

## Baseline financiero — Período 0 — DATOS EXACTOS DEL SIMULADOR

| Concepto | MOST | MOVE | Total empresa |
|----------|------|------|--------------|
| Unidades vendidas | 141,419 | 43,841 | 185,260 |
| Ingresos | $24,518k | $12,299k | **$36,817k** |
| CMV (transfer cost × vendidas) | −$9,746k | −$5,258k | −$15,004k |
| Costo inventario (8% TC × unid.) | $0 | −$500k | −$500k |
| Contribución antes de marketing | $14,772k | $6,540k | $21,312k |
| Publicidad (medios + investigación) | −$1,500k | −$2,500k | −$4,000k |
| Coste comercial (fuerza de ventas) | −$599k | −$599k | −$1,198k |
| Contribución después de marketing | $12,673k | $3,441k | $16,115k |
| Estudios de mercado | — | — | −$306k |
| I+D | — | — | $0 |
| **EBT (Beneficio antes impuestos)** | — | — | **$15,809k** |

> Los $15,809k de EBT en P0 son la base del presupuesto disponible para R1.

---

## Gastos comprometidos en Ronda 1

### 1. Producción (costo automático — no es una decisión de presupuesto)
| Marca | Unidades a producir | Transfer Cost | Costo de producción |
|-------|--------------------|-----------|--------------------|
| MOST  | 200,000            | $69/u     | **$13,800,000** |
| MOVE  | 10,000             | $120/u    | **$1,200,000** |
| **Total producción** | | | **$15,000,000** |

> ⚠️ El aumento de producción de MOST (+42% vs. las ~141k del período anterior) puede generar **costo de ajuste de capacidad** adicional (por superar el ±20% automático).

### 2. Publicidad (decisión activa)
| Marca | Presupuesto | Target |
|-------|-------------|--------|
| MOST  | $1,500,000  | 90% Gen-Z + 10% Millennials |
| MOVE  | $2,500,000  | 100% Millennials |
| **Total publicidad** | **$4,000,000** | |

### 3. Estudios de mercado
| Concepto | Monto |
|----------|-------|
| 14 estudios (todos disponibles) | **$505,750** |

### 4. I+D
| Proyecto | Monto |
|----------|-------|
| Exploración Vodites | **$31,000** |

### 5. Fuerza de ventas
| Concepto | Monto estimado |
|----------|----------------|
| Vendedores activos × $20,400/año | ? (completar con dato del simulador) |
| Costo de contratación/despidos | ? |

### 6. Marketing Digital / Powerhouse
| Concepto | Monto |
|----------|-------|
| (a completar si se usaron estas herramientas) | ? |

---

## Resumen de egresos R1 (conocidos)

| Rubro | Monto |
|-------|-------|
| Producción MOST + MOVE | $15,000,000 |
| Publicidad | $4,000,000 |
| Estudios de mercado | $505,750 |
| I+D Vodites | $31,000 |
| Fuerza de ventas | ? |
| **TOTAL conocido** | **~$19,536,750+** |

---

## Costos de inventario (fluye automáticamente)

```
Costo de inventario = Unidades sobrantes × Transfer Cost × 8%
```

| Marca | Inventario inicial R1 | + Producción | − Ventas est. | Inventario final | Costo estimado |
|-------|-----------------------|------------|--------------|-----------------|----------------|
| MOST  | 0                     | 200,000    | ?            | ?               | ? |
| MOVE  | 52,000                | 10,000     | ?            | ?               | ? |

**Caso base (si MOVE vende solo 30k de 62k disponibles):**
- Sobrante MOVE: 32,000 u × $120 × 8% = **$307,200**

**Caso optimista (MOVE vende todo el stock):**
- Costo inventario MOVE: $0
- Ingresos adicionales: 62,000 × ($390 / 1.20) = $20.15M solo en eCommerce

---

## Eliminación de inventario — ¿Cuándo conviene?

| Opción | Costo | Cuándo usar |
|--------|-------|-------------|
| Cargar inventario al siguiente período | 8% del Transfer Cost × unidades | Cuando hay expectativa razonable de venta futura |
| Eliminar inventario (escritura directa) | 20% del Transfer Cost × unidades | Cuando el producto va a ser discontinuado o reformulado sin posibilidad de venta |

**Ejemplo MOVE (52k u a $120 TC):**
- Cargarlo un año: $120 × 8% × 52,000 = **$499,200**
- Eliminarlo de golpe: $120 × 20% × 52,000 = **$1,248,000**

→ Conclusión: **conviene intentar venderlo** antes de eliminarlo, salvo que se decida discontinuar MOVE definitivamente.

---

## Dónde se registran los gastos en el simulador

| Rubro | Pantalla en el simulador |
|-------|--------------------------|
| Producción | Decide → Production |
| Precio | Decide → Brand Portfolio |
| Publicidad | Decide → Advertising |
| Fuerza de ventas | Decide → Sales Force |
| I+D | Decide → Research & Development |
| Estudios de mercado | Decide → Market Research |
| Digital / Powerhouse | Decide → Digital Marketing / Powerhouse |

---

## Tracking de resultados financieros por período

| Período | Ingresos | Costo prod. | Publicidad | SF | I+D | Estudios | Inventario | **Contrib. Neta** |
|---------|----------|------------|------------|-----|-----|----------|-----------|------------------|
| P0 (base) | $36.8M | ~$15M | — | — | — | — | — | ~$15.8M |
| R1 | ? | $15M est. | $4M | ? | $31k | $505k | ? | ? |
| R2 | | | | | | | | |
| R3 | | | | | | | | |
