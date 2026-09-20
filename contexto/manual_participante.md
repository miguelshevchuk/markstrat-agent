# Manual del Participante — Digital Markstrat
> StratX Simulations / INSEAD · 2023-10-16 · Versión B2C / DG / es-sp
> *Documento de referencia — cargar a contexto solo bajo demanda*

---

## ÍNDICE

- [I. Introducción](#i-introducción)
- [II. Los Productos — Sonites y Vodites](#ii-los-productos)
- [III. Los Consumidores — Segmentos](#iii-los-consumidores)
- [IV. Los Canales de Distribución](#iv-los-canales-de-distribución)
- [V. Entorno Económico](#v-entorno-económico)
- [VI. Investigación y Desarrollo (I+D)](#vi-investigación-y-desarrollo)
- [VII. Costes de Producción y Curva de Experiencia](#vii-costes-de-producción-y-curva-de-experiencia)
- [VIII. Presupuesto de Marketing](#viii-presupuesto-de-marketing)
- [IX. Estudios de Mercado](#ix-estudios-de-mercado)
- [X. El Software — Guía de Uso](#x-el-software)
- [XI. Posicionamiento e I+D](#xi-posicionamiento-e-id)
- [XII. Herramienta Plan de Marketing (VII)](#xii-herramienta-plan-de-marketing)

---

## I. Introducción

Digital Markstrat es una simulación de Marketing estratégico creada por Jean Claude Larreché (cátedra Alfred H. Heineken, INSEAD) y Hubert Gatignon (cátedra Claude Jensen, INSEAD). Fue creada hace más de 30 años y se actualiza continuamente.

**Objetivo:** Gestionar una empresa con portfolio de productos de bienes de consumo no perecederos (consumer durables) en un entorno dinámico y competitivo.

**KPI principal: SPI (Share Price Index)** — índice de precio de la acción. Todas las empresas arrancan en 1.000. El SPI refleja el valor a largo plazo de la empresa. También se mide el **DMI (Digital Marketing Index)** que trackea el nivel de digitalización.

**Duración:** Múltiples períodos de decisión (generalmente 6–8 rondas). Cada período representa un año fiscal.

---

## II. Los Productos

### Sonites (categoría existente)
Dispositivos de consumo electrónico ya establecidos en el mercado.

**Atributos físicos:**
| Atributo | Rango | Descripción |
|----------|-------|-------------|
| Funciones | 5 – 20 | Número de funciones del dispositivo |
| Diseño | 3 – 10 | Puntuación estética/diseño |
| Batería | 24 – 96 h | Duración de batería |
| Pantalla | 4 – 40 " | Tamaño de pantalla |
| Potencia | 5 – 100 GFlops | Capacidad de procesamiento |

**Importancia percibida de atributos por consumidores (Escalas Semánticas):**
> Precio=10 >> Potencia=5.8 >> Diseño=3.4 >> Pantalla=3.1 >> Batería=1.7 >> Funciones=1.3

**Dimensiones perceptuales MDS (posicionamiento Sonites):**
1. **Economía** — percepción de valor/precio
2. **Rendimiento** — percepción de potencia/performance
3. **Conveniencia** — percepción de practicidad/portabilidad

### Vodites (categoría emergente)
Nuevo tipo de producto tecnológico. No está en el mercado al inicio. Requiere inversión en I+D para lanzar.

**Atributos físicos:**
| Atributo | Rango | Descripción |
|----------|-------|-------------|
| Resolución | 20 – 100 L/mm | Resolución de imagen/pantalla |
| Energía | 10 – 100 bC/Wh | Eficiencia energética |
| Carbón/Impacto ecológico | 5 – 50 kg CO2 | Huella de carbono (menos = mejor) |
| Conexión/Conectividad | 3 – 10 | Calidad de conectividad |
| Apps | 5 – 100 | Número de aplicaciones disponibles |

### Operaciones de marca (Brand Portfolio)
- **Mantenerse:** Sin cambios en especificaciones físicas
- **Modificarse:** Requiere proyecto de I+D completado que rediseñe la marca
- **Lanzarse:** Lanzar nueva marca (requiere proyecto I+D completado)
- **Retirarse:** Abandonar la marca. El inventario remanente se elimina con coste

> ⚠️ Cuando una marca se modifica: el inventario antiguo se vende al 80% de su valor (20% de pérdida se carga a Marketing).
> ⚠️ Máximo 5 marcas por categoría (Sonite o Vodite) en el mercado por período.

---

## III. Los Consumidores

### Segmentos Sonite (5 segmentos)

| Segmento | También llamados | Perfil |
|----------|-----------------|--------|
| Profesionales (Pr) | Exploradores | Alta renta, buscan rendimiento máximo |
| Baby Boomers (BB) | Altos Ingresos | Maduros, valoran calidad y marca |
| Gen-X (Gx) | Profs | Experimentados, pragmáticos |
| Millennials (Mi) | Compradores | Orientados a precio-valor, experiencia |
| Gen-Z (Gz) | Ahorradores | Precio muy sensible, digital-first |

Cada segmento tiene diferentes ideales en atributos físicos y perceptuales. Los ideales evolucionan cada período según tendencias del mercado.

### Segmentos Vodite (3 segmentos — adopción secuencial)

| Segmento | Descripción | Cuándo adoptan |
|----------|-------------|---------------|
| Innovadores (In) | Early adopters, dispuestos a pagar más | Primero |
| Pioneros/Adoptadores (Pi) | Seguidores rápidos | Segundo |
| Seguidores (Se) | Mayoría tardía | Tercero |

El mercado Vodite crece de forma natural con el tiempo. Los Seguidores son el segmento más grande pero solo compran cuando el producto ya está establecido.

---

## IV. Los Canales de Distribución

| Canal | Margen retail | Descripción |
|-------|--------------|-------------|
| Tiendas Especializadas | ~35–40% | Clientes que buscan asesoramiento; vendedores físicos |
| Gran Superficie | ~30% | Volumen masivo; menor precio promedio |
| eCommerce / Tiendas Online | ~20% | Canal digital; compra sin asistencia |
| eStore propia | ~20% | Tienda propia de la empresa; mayor control |

**Fuerza de ventas (SF físicos):** Vendedores asignados a Tiendas Especializadas y Gran Superficie. Contratar o despedir vendedores tarda **1 período** en surtir efecto. Se puede ajustar ±20% automáticamente sin coste adicional.

**Marketing Digital:** Presupuesto asignado a eCommerce y eStore propia.

**Costes de SF:**
- Salario: ~$20,400/vendedor/año (sube con inflación del 2% anual)
- Contratación: ~$3,121/vendedor (estimado)
- Despido: ~$5,202/vendedor (estimado)

---

## V. Entorno Económico

| Variable | Valor |
|----------|-------|
| Crecimiento del PIB | **3%** *(⚠️ el PDF indica 4% pero el simulador confirma 3%)* |
| Inflación | **2%** anual |
| Coste de almacenamiento de inventario (IHC) | **8%** del Transfer Cost × unidades/año |
| Coste de eliminación de inventario (IDL) | **20%** del Transfer Cost × unidades (cargo único) |

**Cuándo eliminar vs. almacenar inventario:**
- Almacenar: 8% por año → conveniente si hay expectativa razonable de venta futura
- Eliminar: 20% one-shot → solo si se discontinúa definitivamente la marca

---

## VI. Investigación y Desarrollo

### Proyectos I+D
- **Nomenclatura:** PO+nombre para Sonites; PE+nombre para Vodites
- **Máximo 10 proyectos por período**
- **Coste base:** equivalente al Transfer Cost para las primeras 100,000 unidades
- **Reglas críticas:**
  - El presupuesto sobrante de un proyecto NO se devuelve
  - Las especificaciones de un proyecto en curso NO pueden cambiarse
  - Un proyecto se completa en el período en que se finaliza la inversión necesaria

### Estados de proyectos I+D
1. **No iniciado:** Solo existe en los planes
2. **En curso:** Inversión parcial realizada; NO se pueden cambiar specs
3. **Completado:** Disponible para lanzar o modificar marca

### Cómo usar I+D para modificar/lanzar marcas
1. Crear proyecto I+D con las nuevas specs físicas deseadas
2. Invertir hasta completar el presupuesto necesario
3. En la siguiente decisión de portfolio: seleccionar la marca → "Modificarse" o "Lanzarse" → elegir el proyecto completado

### Proyectos I+D — Inicio de ronda
⚠️ Al inicio de cada nueva ronda, todos los proyectos I+D en curso **continúan automáticamente** a menos que se posponga activamente. Verificar siempre qué proyectos están activos.

---

## VII. Costes de Producción y Curva de Experiencia

### Transfer Cost (TC)
El Transfer Cost es el coste de producción por unidad al que la empresa "vende" internamente a su división comercial.

### Curva de Experiencia
**El TC disminuye −15% cada vez que la producción acumulada se duplica.**

Ejemplo: si el TC actual es $100 con producción acumulada de X, cuando la producción acumulada llegue a 2X, el TC será $85.

### Regla de producción ±20%
La producción puede ajustarse automáticamente hasta ±20% vs. la producción del período anterior, sin coste adicional. Si se supera este rango (en más o en menos), se genera un **coste de ajuste de capacidad**.

### Inventario
```
Stock disponible = Inventario inicial + Producción del período
Inventario final = Stock disponible − Unidades vendidas

Coste inventario = Inventario final × TC × 8% (por año)
Coste eliminación = Unidades eliminadas × TC × 20%
```

---

## VIII. Presupuesto de Marketing

### Cálculo del presupuesto disponible
```
Presupuesto de Marketing = 20% × Contribución Neta del período anterior
Rango: mínimo $7M — máximo $20M
```

> ⚠️ **CRÍTICO:** El presupuesto NO utilizado **NO se transfiere** al siguiente período. Use todo lo que tenga disponible (o planifique bien para no sobre-gastar).

> ⚠️ Si la desviación presupuestaria es **negativa** (gasto > presupuesto), el simulador recorta arbitrariamente el gasto en publicidad para cuadrar el presupuesto. Siempre mantener saldo ≥ 0.

### Componentes del presupuesto de Marketing
El presupuesto de marketing cubre:
1. **Publicidad** (Medios + Investigación publicitaria)
2. **Fuerza de ventas** (Físicos + Digital)
3. **Estudios de mercado**
4. **I+D** (proyectos de investigación y desarrollo)

La producción NO forma parte del presupuesto de marketing. Es un coste separado.

### Medios publicitarios — 5 categorías (deben sumar 100%)
1. **Tradicional** — TV, radio, prensa
2. **Exterior** — vallas, OOH
3. **Digital propio (Owned)** — web propia, redes sociales orgánicas
4. **Digital pagado (Paid)** — SEM, display ads, social ads
5. **Digital afines/boca-oreja (Earned)** — influencers, viralización

**Investigación en publicidad (% del total de publicidad):**
- 4–8% → mantener awareness existente
- 10–15% → reposicionamiento activo (necesario para cambiar percepción)

---

## IX. Estudios de Mercado

Hay **14 estudios disponibles** por período. Se compran al inicio del período y los resultados llegan con los informes de resultados.

### Listado completo de estudios

| Estudio | Nombre | Descripción | Utilidad principal |
|---------|--------|-------------|-------------------|
| A | Benchmark | Especificaciones físicas de TODAS las marcas | Ver qué specs tienen los competidores |
| B | Consumer Survey | Percepción de las marcas en el mercado | Ver cómo nos perciben vs. competencia |
| C | Consumer Panel | Market share por segmento por marca | **Imprescindible** — ver quién compra qué |
| D | Distribution Panel | Share por canal de distribución | Optimizar fuerza de ventas por canal |
| E | Semantic Scales | Percepción en escalas semánticas (1–7) | Evaluar posicionamiento en atributos |
| F | MDS (perceptual map) | Mapa perceptual multidimensional | Posicionamiento visual en espacio perceptual |
| G | Market Forecast | Proyecciones de tamaño de mercado | Planificación de producción y crecimiento |
| H | Competitive Advertising | Presupuestos de publicidad de competidores | Benchmarking de inversión |
| I | Competitive Commercial Team | Fuerza de ventas de competidores | Benchmarking comercial |
| J | Advertising Experiment | Test A/B presupuesto publicidad | Calibrar elasticidad de publicidad |
| K | Commercial Team Experiment | Test fuerza de ventas | Calibrar elasticidad comercial |
| L | Conjoint Analysis | Importancia de atributos para los segmentos | Definir specs óptimas de I+D |
| M | Customer Centricity | Satisfacción y lealtad del cliente | Evaluar calidad de la relación con cliente |
| N | Media Reporting | Efectividad de canales de medios | Optimizar mix de medios publicitarios |

### Estudios recomendados por situación

| Situación | Estudios prioritarios |
|-----------|----------------------|
| Inicio de ronda (siempre) | C (Consumer Panel), B (Consumer Survey), A (Benchmark) |
| Decisión de I+D/specs | L (Conjoint), E (Semantic Scales), F (MDS) |
| Optimizar SF y canales | D (Distribution Panel), K (Commercial Team Experiment) |
| Optimizar publicidad | H (Competitive Advertising), J (Advertising Experiment), N (Media) |
| Planificación a largo plazo | G (Market Forecast) |

### Notas sobre estudios MDS (Estudio F)
El mapa perceptual MDS muestra posiciones de marcas en 3 dimensiones: Economía, Rendimiento, Conveniencia. Los puntos ideales de cada segmento también se muestran. Cuanto más cerca esté una marca del punto ideal de un segmento, mayor participación tenderá a tener en ese segmento.

---

## X. El Software — Guía de Uso

### Acceso
URL: `https://digitalmarkstrat.stratxsimulations.com`

> ⚠️ **RESTRICCIÓN DE SEGURIDAD:** El simulador NUNCA debe modificarse sin autorización explícita. Todas las sesiones de revisión son solo lectura.

### Secciones principales del simulador

#### Menú Decide (tomar decisiones)

| Pantalla | Decisiones |
|----------|-----------|
| **Brand Portfolio** | Precio de venta al canal (precio ex-factory); operación de marca (mantener/modificar/lanzar/retirar) |
| **Production** | Unidades a producir por marca |
| **Advertising** | Presupuesto total por marca; distribución por tipo de medio (%); investigación publicitaria (%); objetivos de segmentos (%) |
| **Sales Force** | Número de vendedores por canal (Especializadas / Gran Superficie); presupuesto Digital Marketing (eCommerce / eStore) |
| **Research & Development** | Proyectos I+D: nuevo proyecto (specs + presupuesto) o continuar proyecto existente |
| **Market Research** | Seleccionar qué estudios comprar este período |
| **Digital Marketing / Powerhouse** | Iniciativas de marketing digital avanzado |

#### Menú Results (ver resultados)
Disponible tras cerrar cada ronda. Incluye:
- **Annual Report:** Informe financiero completo (P&L por marca y empresa)
- **Market Research Reports:** Resultados de los estudios comprados

#### Herramientas de apoyo

**Budget Checker:** Muestra el saldo disponible en tiempo real mientras se toman decisiones. El encabezado del simulador muestra el monto en "+X.XXXk$" (positivo = dentro del presupuesto; negativo = alerta de sobrepasar).

**Errors & Warnings:** Lista de problemas en las decisiones actuales. Revisar siempre antes de confirmar la ronda.

**Marketing Plan Tool (VII):** Herramienta de pro-forma interna. ⚠️ Usa TUS estimaciones, no el modelo matemático real. No está conectada a los resultados reales de la simulación. Ver Sección XII para el detalle.

### Pre-carga de decisiones al inicio de ronda
Al inicio de cada nueva ronda, el simulador pre-carga automáticamente las decisiones del período anterior. Hay que revisar y actualizar TODO, especialmente:
- Precio (puede necesitar ajuste)
- Producción (ajustar por ventas reales del período anterior)
- Publicidad (revisar mix de medios)
- I+D (verificar qué proyectos están activos y si conviene continuar/pausar)
- SF (ajustar según resultados de distribution panel)

---

## XI. Posicionamiento e I+D

### Evaluación perceptual
Las marcas se posicionan en el espacio perceptual según sus especificaciones físicas y las campañas publicitarias. El **Estudio F (MDS)** muestra el mapa actual.

### Puntos ideales por segmento
Cada segmento tiene un "punto ideal" en el espacio perceptual. El objetivo es posicionar la marca lo más cerca posible al punto ideal del segmento objetivo.

### Cuándo reposicionar

**Señales para reposicionar:**
- La distancia al punto ideal objetivo aumenta
- Otros competidores se acercan al punto ideal de tu segmento
- Cambias de segmento objetivo

**Herramientas para reposicionar:**
1. **Via publicidad:** Cambiar la distribución del presupuesto y los objetivos. Efecto gradual. Requiere 10–15% en investigación publicitaria para ser efectivo.
2. **Via I+D:** Cambiar especificaciones físicas. Efecto más duradero pero tarda más (1 ronda de I+D + 1 ronda de lanzamiento).

### Conversión entre atributos físicos y percepción

Para convertir **percepción → físico** (saber qué spec se necesita para un punto perceptual dado):
```
X_físico = LB + [(UB − LB) × (P − 1.0) / 6.0]
```

Para convertir **físico → percepción** (saber en qué punto perceptual está una spec dada):
```
P_perceptual = 1.0 + [6.0 × (X_físico − LB) / (UB − LB)]
```

Donde:
- `LB` = límite inferior del rango físico del atributo
- `UB` = límite superior del rango físico del atributo
- `P` = valor en escala perceptual (1–7)
- `X` = valor físico del atributo

### Estrategia de I+D para specs

**Proceso recomendado:**
1. Consultar el **Estudio L (Conjoint)** para saber qué atributos valora más el segmento objetivo
2. Consultar el **Estudio E (Semantic Scales)** para ver la percepción actual
3. Usar la fórmula de conversión para calcular los valores físicos que dan la percepción deseada
4. Crear el proyecto I+D con esas specs
5. En el período siguiente (una vez completado), modificar/lanzar la marca

---

## XII. Herramienta Plan de Marketing (VII)

La herramienta de Plan de Marketing (sección VII del software) es una **pro-forma interna de 5 pasos**. Es una herramienta de planificación, **no** de decisión. Sus resultados son proyecciones basadas en TUS estimaciones, no en el modelo matemático del simulador.

> ⚠️ El Marketing Plan Tool NO está conectado al motor de resultados reales. Usar solo como referencia de planificación.

### Paso 1 — Estimaciones de tamaño de segmento

Ingresar las estimaciones de tamaño de cada segmento para el período actual. Se puede usar el **Estudio G (Market Forecast)** como base.

### Paso 2 — Estimaciones de Market Share

Para cada marca/segmento, ingresar el market share esperado (%). La herramienta calcula el volumen de ventas estimado: `Ventas estimadas = Tamaño segmento × Market share %`

### Paso 3 — Estimaciones de ventas en valor

Dado el volumen de ventas estimado y el precio, calcula los ingresos proyectados por marca.

### Paso 4 — Contribución por marca (Brand Contribution)

Formulario pro-forma de contribución por marca. Componentes:

| Línea | Cálculo |
|-------|---------|
| (a) Ingresos | Precio × Unidades estimadas vendidas |
| (b) Inventario inicial | Unidades en stock al inicio del período |
| (c) Plan de producción | Según decisión de producción |
| (d) Producción real | Puede diferir si se activa límite ±20% |
| (e) Inventario final proyectado | b + d − ventas estimadas |
| (f) Ventas finales | Ventas reales (igual a estimadas si no hay stock-out) |
| (g) Ingresos | Precio × f |
| (h) **CUV (Coste Unidades Vendidas)** | Ventas estimadas × TC unitario (considera curva de experiencia) |
| (i) **Coste de almacenamiento de inventario** | Inventario final × TC × IHC (8%) |
| (j) **Coste por eliminación de inventario** | Unidades eliminadas × TC × IDL (20%) |
| (k) **Contribución antes de Marketing** | (g) − (h) − (i) − (j) |
| (l) Medios de publicidad | Según decisión |
| (m) Investigación en publicidad | Según decisión |
| (n) Costes del equipo comercial | Basado en decisión de SF + coste por vendedor del período |
| (o) **Contribución después de Marketing** | (k) − (l) − (m) − (n) |

### Paso 5 — Pérdidas y Ganancias de la empresa (Company P&L)

Consolida todas las marcas y añade los gastos a nivel empresa:

| Línea | Descripción |
|-------|-------------|
| Revenues | Suma de ingresos de todas las marcas |
| Cost of goods sold | Suma de CUV de todas las marcas |
| Inventory costs | Suma de costes de inventario |
| **Contribution before marketing** | Suma línea (k) de todas las marcas |
| Advertising expenditures | Suma publicidad (medios + investigación) |
| Commercial team costs | Suma costes SF de todas las marcas |
| **Contribution after marketing** | Suma línea (o) de todas las marcas |
| (j) Estudios de Investigación de Mercado | Coste total de estudios comprados |
| (k) Investigación y desarrollo | Suma de presupuestos I+D asignados |
| (l) Costes y beneficios excepcionales | Normalmente $0; se activa si se retira una marca |
| (m) **Beneficios antes de impuestos (EBT)** | Contribución después de mkt − (j) − (k) − (l) |

**Reflexiones que guía la herramienta:**

*¿Cómo mejorar ingresos?*
- ¿El producto es adecuado para el segmento? → Considerar I+D
- ¿El precio es el correcto? → ¿Subir rentabilidad o bajar para ganar volumen?
- ¿Los objetivos de percepción están bien definidos? → Revisar posicionamiento
- ¿El esfuerzo en publicidad y SF es suficiente?
- ¿Focalizarse en 1 segmento o atacar 2–3 segmentos?

*¿Cómo reducir costes?*
- ¿I+D de reducción de costes para bajar el CUV?
- ¿Reducir producción para eliminar inventario existente?
- ¿Incrementar producción para aprovechar la curva de experiencia?
- ¿La awareness es suficiente para reducir publicidad?
- ¿El equipo comercial está sobredimensionado vs. la competencia?

---

## APÉNDICE — Resumen de fórmulas clave

### Finanzas

```
EBT = Contribución después de Mkt − Estudios de mercado − I+D − Costes excepcionales

Contribución después de Mkt = Ingresos − CMV − Inv. holding − Publicidad − SF

CMV = Unidades vendidas × Transfer Cost (con curva de experiencia)

Inventario holding = Unidades sobrantes × TC × 8%

Inventario eliminación = Unidades eliminadas × TC × 20%

Presupuesto Marketing disponible = 20% × Contribución Neta período anterior
Rango: $7M – $20M (no transferible al siguiente período)
```

### Curva de Experiencia
```
TC_nuevo = TC_actual × (1 − 0.15) cuando producción acumulada se duplica
```

### Conversión física ↔ perceptual
```
Perceptual → Físico: X = LB + [(UB − LB) × (P − 1.0) / 6.0]
Físico → Perceptual: P = 1.0 + [6.0 × (X − LB) / (UB − LB)]
```

### Producción
```
Ajuste automático sin coste: ±20% vs. producción período anterior
Superar ±20% → costo de ajuste de capacidad (en ambas direcciones)
```

### Publicidad efectiva para reposicionamiento
```
Investigación publicitaria: 10–15% del presupuesto total de publicidad
Mantener awareness: 4–8%
```

---

## ACERCA DE DIGITAL MARKSTRAT

Digital Markstrat fue creada hace más de 30 años por Jean Claude Larreché (cátedra Alfred H. Heineken, INSEAD) y Hubert Gatignon (cátedra Claude Jensen, INSEAD). Ha sido continuamente actualizada y mejorada desde su creación.

StratX Simulations es una filial de STRATX, fundada por Jean Claude Larreché. Sus herramientas incluyen Digital Markstrat, BrandPRO, MixPRO, Digital MediaPRO, Markops y Blue Ocean Strategy Simulation, utilizadas en más de 500 escuelas de negocios de más de 60 países.
