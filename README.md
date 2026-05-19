# Obsidian AI Architecture

Vault de Obsidian para organizar un sistema de trabajo con agentes, skills y proyectos de IA sin mezclar responsabilidades.

Este repositorio guarda la arquitectura central, los dashboards de navegacion, los mapas de routing y las bases de conocimiento por dominio.

## Objetivo

El vault esta disenado para trabajar con varias areas de IA conectadas entre si:

- Mantener cada skill separada por proyecto.
- Conectar los proyectos desde un centro global.
- Evitar que Marketing, UI/UX, Remotion, Stop Slop y Context Engineering mezclen responsabilidades.
- Usar un mapa de routing para decidir que skill usar primero y cual usar como soporte.
- Mantener el grafo de Obsidian limpio, con colores por dominio y sin nodos aislados.

## Entrada Principal

Empieza siempre por:

- `00_Global/00_Command_Center.md`

Despues usa:

- `00_Global/Agent_Context_Map.md` para entender la arquitectura general.
- `00_Global/Skill_Routing_Map.md` para decidir que skill usar sin mezclar dominios.

## Estructura

```text
00_Global/
  00_Command_Center.md
  Agent_Context_Map.md
  Skill_Routing_Map.md

Marketing_Project/
  00_Dashboard/
  10_Skills/
  20_Logs/

Stop_Slop_Project/
  00_Dashboard/
  10_Skills/
  20_References/

UI_UX_Pro_Max_Project/
  00_Dashboard/
  10_Skills/
  20_Data/

Remotion_Project/
  00_Dashboard/
  10_Skills/
  20_Logs/

Context_Engineering_Project/
  00_Dashboard/
  10_Foundations/
  20_Course/
  30_Templates/
  40_Cognitive_Tools/
  50_Protocols/
  60_Reference/

references/
```

## Skills

### Marketing

Usar para campanas, funnels, CRO, SEO, ads, emails, pricing, launches y growth strategy.

Entrada:

- `Marketing_Project/00_Dashboard/Marketing_Overview.md`
- `Marketing_Project/10_Skills/Marketing_Skills_Index.md`

### Stop Slop

Usar para limpiar copy, mejorar claridad, tono, estructura y calidad del lenguaje.

Entrada:

- `Stop_Slop_Project/00_Dashboard/StopSlop_Overview.md`
- `Stop_Slop_Project/10_Skills/Stop_Slop_Skills_Index.md`

### UI/UX Pro Max

Usar para diseno de interfaces, sistemas visuales, flujos de producto y razonamiento UX.

Entrada:

- `UI_UX_Pro_Max_Project/00_Dashboard/UI_UX_Overview.md`
- `UI_UX_Pro_Max_Project/10_Skills/UI_UX_Skills_Index.md`

### Remotion

Usar para videos programaticos, animaciones, assets de motion y renderizado.

Entrada:

- `Remotion_Project/00_Dashboard/Remotion_Overview.md`
- `Remotion_Project/10_Skills/Remotion_Skills_Index.md`

### Context Engineering

Usar para prompts, memoria, RAG, agentes, cognitive tools, protocolos y evaluacion.

Entrada:

- `Context_Engineering_Project/00_Dashboard/Context_Overview.md`
- `Context_Engineering_Project/10_Foundations/Foundations_Index.md`
- `Context_Engineering_Project/20_Course/Course_Index.md`
- `Context_Engineering_Project/30_Templates/Templates_Index.md`
- `Context_Engineering_Project/40_Cognitive_Tools/Cognitive_Tools_Index.md`
- `Context_Engineering_Project/50_Protocols/Protocols_Index.md`
- `Context_Engineering_Project/60_Reference/Reference_Index.md`

## Reglas De Uso

- Elegir un skill primario antes de empezar.
- Usar skills secundarios solo cuando la tarea lo necesite.
- Guardar notas, logs y outputs dentro del proyecto primario.
- No mover contenido de un dominio a otro solo para conectar el grafo.
- Usar `Skill_Routing_Map.md` como punto de colaboracion entre proyectos.
- Usar `references/checklist.md` solo como validacion global, no como dueno de proyecto.

## Colores Del Grafo

La configuracion vive en:

- `.obsidian/graph.json`

Colores:

- Global / references: gris
- Marketing: verde
- Stop Slop: naranja
- UI/UX: purpura
- Remotion: azul
- Context Engineering: marron

Tambien esta activado `hideUnresolved` para evitar nodos fantasma por enlaces externos o archivos no copiados.

## Estado Actual

El grafo fue normalizado con:

- 0 enlaces ambiguos.
- 0 notas huerfanas.
- 0 notas aisladas.
- Indices internos por proyecto.
- Routing global para colaboracion entre skills.

## Flujo Recomendado

1. Abrir `00_Global/00_Command_Center.md`.
2. Revisar `00_Global/Skill_Routing_Map.md`.
3. Elegir el dashboard del proyecto primario.
4. Entrar al indice interno de esa skill.
5. Crear logs o nuevas notas dentro del proyecto correspondiente.
6. Si una tarea necesita otro skill, enlazarlo desde el mapa global o desde la seccion de conexiones, no mezclar contenido.

## Git

Este vault esta preparado para guardarse como repositorio Git privado.

Comandos utiles:

```bash
git status
git add .
git commit -m "Update vault"
git push
```
