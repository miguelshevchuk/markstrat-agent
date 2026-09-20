# Markstrat-agent — Índice de Contexto

> Archivo ligero que carga la skill `/mostros`. No contiene datos detallados — solo apunta a dónde encontrarlos.

---

## Estado rápido

| Campo | Valor |
|-------|-------|
| Empresa | **Mostros** — Letra M, Industria Albatross |
| Marcas activas | **MOST** (TC $69) · **MOVE** (TC $120) |
| Período actual | **Ronda 1** — decisiones enviadas, resultados pendientes |
| Presupuesto R1 | Saldo disponible: **+$1,252k** (confirmado en simulador) |
| Vendedores R1 | 170 físicos (MOST 65 / MOVE 105) + $450k digital |

---

## Mapa de archivos

### 00_general — Siempre relevante
| Archivo | Contenido |
|---------|-----------|
| `00_general/equipo.md` | Quiénes somos, misión, estrategia macro por período |
| `00_general/competencia.md` | Specs, market share, ingresos de los 5 equipos (T/L/R/S + nosotros) |
| `00_general/reglas_simulacion.md` | Reglas confirmadas en el simulador (GDP 3%, inflación 2%, etc.) |

### periodo_01/decisiones — Decisiones enviadas en R1
| Archivo | Decisión clave |
|---------|---------------|
| `periodos/periodo_01/decisiones/portfolio.md` | Precios: MOST $182 · MOVE $390 |
| `periodos/periodo_01/decisiones/produccion.md` | MOST 200k · MOVE 10k |
| `periodos/periodo_01/decisiones/publicidad.md` | MOST $1.5M · MOVE $2.5M |
| `periodos/periodo_01/decisiones/fuerza_ventas.md` | 170 vendedores · $450k digital |
| `periodos/periodo_01/decisiones/presupuesto.md` | Saldo $1,252k — breakdown completo |
| `periodos/periodo_01/decisiones/investigacion.md` | 14 estudios · $505,750 |
| `periodos/periodo_01/decisiones/i_d.md` | Exploración Vodites · $31k |

### periodo_01/resultados — A completar cuando salgan los resultados
| Archivo | Estado |
|---------|--------|
| `periodos/periodo_01/resultados/kpis.md` | Baseline P0 cargado · R1 pendiente |
| `periodos/periodo_01/resultados/informe_anual.md` | Pendiente |
| `periodos/periodo_01/resultados/analisis.md` | Pendiente |

### contexto — Solo bajo demanda explícita
| Archivo | Peso | Cuándo cargar |
|---------|------|---------------|
| `contexto/manual_participante.md` | ~7k palabras | Si hay dudas sobre reglas, fórmulas, mecánicas del simulador |

---

## Guía rápida de consulta

| Si preguntan por… | Cargar… |
|-------------------|---------|
| Competencia / market share | `competencia.md` |
| Reglas del simulador / fórmulas | `reglas_simulacion.md` o `manual_participante.md` |
| Presupuesto / plata disponible | `presupuesto.md` |
| Decisión de precio | `portfolio.md` |
| Producción / inventario | `produccion.md` |
| Vendedores / canales | `fuerza_ventas.md` |
| KPIs / SPI / resultados | `kpis.md` |
| I+D / Vodites | `i_d.md` |
| Publicidad / medios | `publicidad.md` |
