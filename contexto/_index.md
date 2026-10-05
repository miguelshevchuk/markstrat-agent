# Markstrat-agent — Índice de Contexto

> Archivo ligero que carga la skill `/mostros`. No contiene datos detallados — solo apunta a dónde encontrarlos.

---

## Estado rápido

| Campo | Valor |
|-------|-------|
| Empresa | **Mostros** — Letra M, Industria Albatross |
| Marcas activas | **MOST** ($177, coste $78) · **MOVE** ($273, coste $123) |
| Período actual | **Ronda 3**: plan en `periodos/periodo_03/decisiones/plan_r3.md` + `periodos/periodo_03/plan_r3.html` (sin cargar) |
| Supuestos R3 | Sin I+D Vodites, sin préstamos |
| Presupuesto R3 | $10,600k autorizado |
| SPI / ranking | P1: 944 (3°) → **P2: 781 (5° de 5)**. Líder L 1,351 |
| Situación P2 | Ingresos $33.7M (−15%) · Contrib. neta $7.7M (última) · MS unid. 17.4% |
| Listos para P3 | **POMOST2** (Gen-Z, coste $68) · **POMOVE2** (Millennials, coste $127) |
| Vodites | I+D ~$10M según el profesor → descartado por ahora |

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

### periodo_01/resultados — ✅ Completo
| Archivo | Contenido |
|---------|-----------|
| `periodos/periodo_01/resultados/kpis.md` | Baseline P0 + KPIs R1 (SPI 944, 3°) |
| `periodos/periodo_01/resultados/informe_anual.md` | Panel de industria, marcas y estudios R1 |
| `periodos/periodo_01/analisis.md` | Post-ronda R1 |
| `periodos/periodo_01/resultados/TeamExport_Periodo_1.xlsx` | Export crudo |

### periodo_02 — ✅ Completo
| Archivo | Contenido |
|---------|-----------|
| `periodos/periodo_02/decisiones/decisiones_r2.md` | Decisiones R2 reconstruidas (precios, producción, publicidad, SF, I+D) |
| `periodos/periodo_02/resultados/kpis.md` | KPIs R2: SPI 781 (5°), finanzas, funnel, ROMI |
| `periodos/periodo_02/resultados/informe_anual.md` | Industria, marcas, semánticas, MDS, conjoint, Vodites |
| `periodos/periodo_02/analisis.md` | **Por qué caímos de 3° a 5°** + ideas R3 |
| `periodos/periodo_02/resultados/TeamExport_Periodo_2.xlsx` | Export crudo |

### contexto — Solo bajo demanda explícita
| Archivo | Peso | Cuándo cargar |
|---------|------|---------------|
| `contexto/manual_participante.md` | ~7k palabras | Si hay dudas sobre reglas, fórmulas, mecánicas del simulador |

---

## Reglas de comportamiento para Claude

> Estas reglas aplican a todas las sesiones. Claude debe respetarlas sin que se le recuerden.

| Regla | Detalle |
|-------|---------|
| **Enfoque agresivo** | Ninguna propuesta debe ser conservadora. Siempre maximizar: capturar share, invertir fuerte donde hay oportunidad, tomar riesgos calculados. En precios, publicidad, I+D, distribución y cualquier decisión estratégica. |
| **URL del simulador** | https://digitalmarkstrat.stratxsimulations.com — Para interactuar con el simulador, aclarar que se necesita **Claude en Chrome** activo y la sesión iniciada en la plataforma. |

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
| KPIs / SPI / resultados | `periodos/periodo_02/resultados/kpis.md` (último) |
| Por qué caímos / diagnóstico | `periodos/periodo_02/analisis.md` |
| Semánticas / MDS / conjoint | `periodos/periodo_02/resultados/informe_anual.md` |
| I+D / Vodites | `i_d.md` |
| Publicidad / medios | `publicidad.md` |
