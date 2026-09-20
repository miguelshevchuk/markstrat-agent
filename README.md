# Markstrat-agent

Repositorio de contexto y memoria para la simulación **Digital Markstrat** (StratX / INSEAD).  
Empresa: **Mostros** · Letra M · Industria Albatross · Marcas: MOST y MOVE.

El objetivo de este proyecto es centralizar toda la información de la simulación (decisiones, resultados, reglas, inteligencia competitiva) de forma que Claude pueda levantarla a demanda en cada sesión, sin necesidad de reexplicar el contexto desde cero.

---

## Estructura del proyecto

```
Markstrat-agent/
│
├── README.md                          ← este archivo
│
├── contexto/
│   ├── _index.md                      ← índice ligero (lo carga /mostros)
│   └── manual_participante.md         ← manual completo del simulador (84 págs → MD)
│
├── skills/
│   ├── mostros.md                     ← skill de entrada: carga el índice del proyecto
│   ├── analisis_segmentos.md          ← interpretación de estudios de segmentos
│   ├── estrategia_id.md               ← decisiones de I+D: flujo, rangos, checklist
│   ├── estrategia_precios.md          ← framework de pricing: floor/ceiling, márgenes
│   ├── interpretacion_estudios.md     ← guía de los 14 estudios de mercado
│   ├── publicidad_efectiva.md         ← mix de medios y calibración de presupuesto
│   └── spi_drivers.md                 ← los 5 drivers del SPI y trade-offs clásicos
│
├── 00_general/
│   ├── equipo.md                      ← quiénes somos, estrategia macro
│   ├── competencia.md                 ← specs y shares de los 5 equipos
│   └── reglas_simulacion.md           ← reglas confirmadas en el simulador
│
└── periodos/
    └── periodo_01/
        ├── decisiones/
        │   ├── portfolio.md           ← precios por marca
        │   ├── produccion.md          ← unidades producidas
        │   ├── publicidad.md          ← presupuesto y mix de medios
        │   ├── fuerza_ventas.md       ← vendedores y marketing digital
        │   ├── presupuesto.md         ← presupuesto total y saldo disponible
        │   ├── investigacion.md       ← estudios de mercado contratados
        │   └── i_d.md                 ← proyectos de I+D
        └── resultados/
            ├── kpis.md                ← SPI, market share, finanzas
            ├── informe_anual.md       ← informe anual del simulador
            └── analisis.md            ← análisis post-ronda y decisiones futuras
```

---

## Skills disponibles

### `/mostros`

**Propósito:** Punto de entrada estándar para cualquier sesión de trabajo con el proyecto. Carga el contexto mínimo e indispensable para orientarse, sin traer al contexto todo el proyecto.

**Qué hace:**
1. Lee `contexto/_index.md` — un archivo liviano con el estado actual de la empresa y un mapa de todos los archivos disponibles.
2. Presenta un resumen rápido: empresa, período activo, presupuesto y estado.
3. Queda lista para cargar archivos específicos bajo demanda según lo que se necesite responder.

**Regla de carga:** Solo trae más contexto si la pregunta lo requiere. Nunca carga el manual completo por defecto.

**Cuándo usarla:** Al inicio de cualquier sesión en la que se vaya a trabajar con el proyecto Markstrat.

---

### `/analisis-segmentos`

**Propósito:** Framework para interpretar los estudios de segmentos y traducirlos en decisiones de producto y comunicación.

**Qué hace:**
- Guía la lectura del **Estudio 4 (Semantic Scales):** detecta brechas entre percepción y realidad, y entre lo que el segmento desea y lo que la marca ofrece.
- Guía la lectura del **Estudio 5 (MDS):** interpreta el mapa perceptual y la distancia al punto ideal de cada segmento.
- Guía la lectura del **Estudio 11 (Conjoint Analysis):** extrae el peso relativo de cada atributo por segmento para priorizar decisiones de I+D.
- Incluye tablas de referencia rápida para los 5 segmentos Sonite y los 3 segmentos Vodite (prioridad de atributos, canal preferido, sensibilidad al precio).

**Cuándo usarla:** Cuando llegan los resultados de una ronda y hay que interpretar cómo perciben los consumidores las marcas y qué valoran.

---

### `/estrategia-id`

**Propósito:** Guía de decisiones de Investigación & Desarrollo: cuándo iniciar proyectos, qué specs definir y cómo validarlos antes de enviar.

**Qué hace:**
- Define el **flujo de trabajo en 3 períodos** (solicitar Conjoint → iniciar I+D → lanzar).
- Documenta los **rangos válidos de atributos** para Sonites y Vodites (Processing Power, Screen Size, Design, Battery, Functions / Resolution, Energy Efficiency, Ecological Impact, Connectivity, Apps).
- Establece la **naming convention** para proyectos (`P-MARCA_VERSION`).
- Incluye un **checklist de validación** antes de enviar el proyecto al simulador.

**Cuándo usarla:** Al definir o revisar proyectos de I+D, o cuando hay que diseñar specs para un nuevo producto o mejora.

---

### `/estrategia-precios`

**Propósito:** Framework estructurado para fijar precios por marca, canal y segmento.

**Qué hace:**
- Calcula el **precio mínimo (floor)** a partir del transfer cost y los márgenes de canal.
- Estima el **precio máximo (ceiling)** en función de la disposición a pagar del segmento y los precios de la competencia.
- Documenta los **márgenes por canal** (Especializadas 40%, Grandes Superficies 30%, eCommerce 20%).
- Incluye una tabla de **señales de precio mal calibrado** (stockout, alto inventario, margen bajo, pérdida de share) con diagnóstico y acción recomendada.
- Contempla el **ajuste por inflación** (2% anual).

**Cuándo usarla:** Al revisar o definir precios para la próxima ronda, o cuando hay señales de que el precio actual no está bien calibrado.

---

### `/interpretacion-estudios`

**Propósito:** Guía de cuándo y cómo usar cada uno de los 14 estudios de mercado según el tipo de decisión.

**Qué hace:**
- Clasifica los estudios por tipo de decisión: **producto/I+D**, **comunicación**, **distribución** y **estrategia/finanzas**.
- Identifica cuáles pedir siempre (Consumer Panel, Semantic Scales) y cuáles son específicos de cada momento.
- Incluye ejemplos de lectura para el Semantic Scales (brechas), el Conjoint (pesos por atributo) y el MDS (distancia al ideal).

**Cuándo usarla:** Al planificar qué estudios contratar para la próxima ronda, o al interpretar los resultados recibidos.

---

### `/publicidad-efectiva`

**Propósito:** Guía para diseñar la estrategia publicitaria: mix de medios, calibración de presupuesto y checklist de decisión.

**Qué hace:**
- Define los **principios clave** de publicidad efectiva en Markstrat (comunicar atributos valorados, concentrar presupuesto, consistencia de mensaje).
- Incluye una **tabla de mix de medios por segmento** (Digital Propio, Pagado, Ganado, Tradicional, Exterior) para los 5 segmentos Sonite y los 3 segmentos Vodite.
- Explica cómo **calibrar el presupuesto** evitando estar por debajo del umbral de notoriedad y los rendimientos decrecientes.
- Incluye un **checklist de decisión publicitaria** y guía para usar el Advertising Experiment (Estudio 8).

**Cuándo usarla:** Al definir el presupuesto y estrategia de comunicación para la próxima ronda.

---

### `/spi-drivers`

**Propósito:** Marco para entender qué mueve el SPI y tomar decisiones estratégicas entre rondas.

**Qué hace:**
- Explica los **5 drivers del SPI:** market share en valor, crecimiento de ventas, contribución neta del período, contribución neta acumulada y calidad de I+D.
- Describe la estrategia recomendada para cada driver.
- Incluye una tabla de **trade-offs clásicos:** qué hacer cuando hay alto market share pero baja rentabilidad, alta rentabilidad pero bajo crecimiento, SPI cayendo sin causa clara, o competencia agresiva en precio.

**Cuándo usarla:** Para diagnóstico estratégico entre rondas, especialmente cuando el SPI no evoluciona como se esperaba.

---

## Cómo instalar las skills

Las skills se guardan en la cuenta de Claude y se invocan con `/nombre-skill` en cualquier conversación.

### Instalación (primera vez o reinstalación)

1. Abrí una sesión de Claude (Cowork o Claude Code) con la carpeta `markstrat-agent` conectada.
2. Pedile a Claude que instale las skills desde la carpeta:

   > "Instalá las skills que hay en la carpeta `skills/`"

3. Claude va a mostrar tarjetas de revisión para cada skill nueva — hacé clic en **Guardar** en cada una.

### Verificar que una skill está activa

Escribí `/mostros` en cualquier conversación de Claude. Si está instalada, Claude va a ejecutarla automáticamente.

---

## Flujo de trabajo por período

```
Inicio de ronda
    └── /mostros                        ← orientarse rápido
    └── Revisar decisiones previas      ← periodos/periodo_XX/decisiones/
    └── Tomar nuevas decisiones         ← ingresar en el simulador
    └── Documentar decisiones           ← actualizar archivos en decisiones/

Cuando salen resultados
    └── Documentar en resultados/kpis.md
    └── Documentar en resultados/informe_anual.md
    └── Analizar en resultados/analisis.md
    └── Actualizar contexto/_index.md   ← cambiar "Período actual"
```

---

## Convenciones

- Los archivos de **decisiones** se llenan antes de confirmar la ronda en el simulador.
- Los archivos de **resultados** se llenan cuando el simulador entrega el informe anual.
- `contexto/_index.md` se actualiza al cambiar de período (cambiar la línea "Período actual").
- El `manual_participante.md` no se toca — es referencia de solo lectura.
- **El simulador en `digitalmarkstrat.stratxsimulations.com` es estrictamente de solo lectura.** Ningún script ni automatización debe modificarlo.
