---
name: mostros
description: Levanta el contexto mínimo del proyecto Digital Markstrat de Mostros: lee el índice del proyecto y presenta el estado actual, dejando el resto disponible bajo demanda.
---

# Skill: Mostros — Contexto Markstrat

Cuando se invoca `/mostros`:

## 1. Leer el índice del proyecto

Cargar el archivo índice desde el PC del usuario:
- Path: `C:\Workspace\Markstrat-agent\contexto\_index.md`
- Usar `mcp__remote-devices__device_stage_files` con ese path, luego `Read` el archivo staged.

## 2. Presentar estado mínimo

Con el índice en contexto, responder con:
- **Empresa y período actual** (extraídos de la sección "Estado rápido" del índice)
- **Qué contexto está cargado** (solo el índice)
- **Qué más se puede cargar** si hace falta (mencionarlo brevemente)

No narrar el proceso de lectura. Ir directo al resumen.

## 3. Regla de carga bajo demanda

NO cargar ningún archivo adicional por iniciativa propia. Solo cargar más contexto si:
- El usuario lo pide explícitamente, O
- La pregunta actual no puede responderse con el índice y requiere datos de un archivo específico

En ese caso, cargar SOLO el archivo relevante según la "Guía rápida de consulta" del índice.

## 4. Paths de referencia

Base del proyecto en PC: `C:\Workspace\Markstrat-agent\`

Todos los archivos del índice son relativos a esa base. Para acceder a cualquiera:
1. `mcp__remote-devices__device_stage_files` con el path completo (base + ruta relativa)
2. `Read` el archivo staged

El archivo más pesado (`contexto/manual_participante.md`) solo se carga si el usuario pregunta explícitamente sobre reglas, fórmulas o mecánicas del simulador.
