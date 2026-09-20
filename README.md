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
│   └── mostros.md                     ← definición de la skill /mostros
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

## Cómo instalar las skills

Las skills se guardan en la cuenta de Claude y se invocan con `/nombre-skill` en cualquier conversación.

### Instalación inicial (primera vez)

1. Abrí una sesión de Claude (Cowork o Claude Code)
2. Pedile a Claude que lea el archivo de la skill y la proponga:

   > "Leé `skills/mostros.md` y proponé la skill para guardarla"

3. Claude va a mostrar una tarjeta de revisión — hacé clic en **Guardar**

### Reinstalar una skill (si se pierde o se quiere actualizar)

El contenido canónico de cada skill está en la carpeta `skills/`. Para reinstalar:

1. Abrí una sesión de Claude
2. Pedile que lea el archivo correspondiente de `skills/` y lo proponga nuevamente
3. Guardá desde la tarjeta de revisión

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
