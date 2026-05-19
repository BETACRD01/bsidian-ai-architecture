# Agent Context Map: System Workspace

## Overview
This Obsidian vault serves as the centralized knowledge base and control center for multi-project AI engineering. All projects are isolated by directory but interconnected via global navigation nodes.

## Directory Structure
- `/Marketing_Project/`: High-level marketing strategies, logs, and skills.
- `/Stop_Slop_Project/`: Content clarity and language optimization skills.
- `/UI_UX_Pro_Max_Project/`: UI design systems and coding intelligence.
- `/Remotion_Project/`: Programmatic video generation.
- `/Context_Engineering_Project/`: Cognitive architectures and prompt programming.
- `/00_Global/`: Contains the **[[00_Command_Center]]**.

## Graph Color Configuration (graph.json)
The graph view uses path-based color-coding to maintain visual hierarchy:
- **00_Global**: Neutral `#4B5563` (rgb: 4937059)
- **Marketing_Project**: Green `#2F9E44` (rgb: 3120708)
- **Stop_Slop_Project**: Orange `#F08C00` (rgb: 15764480)
- **UI_UX_Pro_Max_Project**: Purple `#9C36B5` (rgb: 10237621)
- **Remotion_Project**: Blue `#1971C2` (rgb: 1667522)
- **Context_Engineering_Project**: Brown `#8D6E63` (rgb: 9268835)

## Skill Relationship Map
- **Context Engineering** feeds prompt architecture, memory, RAG, and agent workflows into all other projects.
- **Marketing** uses UI/UX, Stop Slop, Remotion, and Context Engineering to turn strategy into campaigns.
- **UI/UX Pro Max** defines product experience, interface quality, and visual systems.
- **Stop Slop** cleans language, messaging, and written outputs across Marketing and UI.
- **Remotion** converts marketing and UI concepts into programmable video assets.
- **Routing rule**: use [[Skill_Routing_Map]] to combine skills intentionally. Do not place cross-project work inside a skill folder unless that skill is the primary owner.

## System Navigation
- All project Dashboards are linked back to `00_Global/00_Command_Center.md` for rapid context switching.
- Use `00_Global/Skill_Routing_Map.md` when a task needs more than one skill.
- Use the **Bookmarks** sidebar to jump between project Overviews.

## Agent Guidelines
1. **Always read `00_Global/00_Command_Center.md` first** upon entering this system.
2. Maintain the color hierarchy when adding new projects.
3. Keep logs in the `20_Logs` folder of the respective project to ensure graph connectivity.
4. If a file appears "grey" in the graph, it lacks bidirectional linking to its parent project Overview.
