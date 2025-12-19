# Memory Bank & Constitutional AI Agent System 🧠

[English](docs/README.en.md) | [Türkçe](docs/README.tr.md) | [Azərbaycan](docs/README.az.md) | [Deutsch](docs/README.de.md) | [Français](docs/README.fr.md) | [Español](docs/README.es.md)

> Un marco determinista para transformar LLMs en ingenieros de software sin estado y guiados por documentación.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎯 Filosofía Principal

Imagina a un desarrollador experto con una disciplina arquitectónica perfecta, pero que sufre **amnesia completa** después de cada sesión.  
Para funcionar, depende completamente de dos artefactos:

1. **Constitution (`AGENTS-Constitution.md`)**  
   La ley técnica suprema del proyecto.

2. **Memory Bank (`MemoryBank.md` + archivos de contexto)**  
   Un registro vivo y versionado de los objetivos, la arquitectura, las decisiones y el progreso.

Esta restricción se convierte en una ventaja:

> **Documentación perfecta · Razonamiento reproducible · Desarrollo orientado a la arquitectura**

---

## 📁 Estructura del Repositorio

```text
memory-bank/
├── MemoryBank.md           # Protocolo operativo y framework RAGESe
├── AGENTS-Constitution.md  # Ley técnica suprema (reglas no negociables)
├── projectbrief.md         # “Por qué” estratégico y criterios de éxito
├── productContext.md       # Problemas del usuario y objetivos de experiencia
├── systemPatterns.md       # Patrones de arquitectura y diseño
├── techContext.md          # Stack tecnológico, herramientas y limitaciones
├── activeContext.md        # Estado actual y enfoque
└── progress.md             # Registro de evolución e historial de decisiones

🚀 Inicio Rápido
1️⃣ Clonar en tu proyecto

git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
cp -r memory_bank_and_constitution/memory-bank ./memory-bank

2️⃣ Personalizar la Constitution

Edita memory-bank/AGENTS-Constitution.md:

    Ajusta los lenguajes o versiones de entorno

    Define las capas arquitectónicas

    Establece reglas de calidad de código, pruebas y diseño

    ⚠️ Este archivo actúa como la ley del proyecto. Cámbialo deliberadamente.

3️⃣ Inicializar el Contexto

Completa primero:

    projectbrief.md — Razón de existencia del proyecto

    techContext.md — Stack tecnológico real

    systemPatterns.md — Arquitectura y límites

🤖 Primer Prompt — Boot Protocol

Usa exactamente este prompt para inicializar un agente IA:

You are operating under a stateless execution model.

STEP 1 — MANDATORY CONTEXT LOAD
Read and internalize the following files from the `memory-bank/` directory:
1. MemoryBank.md
2. AGENTS-Constitution.md

Do not proceed until both are fully read.

STEP 2 — ACKNOWLEDGEMENT
Explicitly confirm:
- You have read and understood both files
- You accept RAGESe, the Context Integrity Gateway, and constitutional authority
- You will assume no undocumented knowledge

STEP 3 — PROJECT ANALYSIS
Scan the existing codebase.
Identify whether these files exist and are accurate:
- projectbrief.md
- productContext.md
- systemPatterns.md
- techContext.md
- activeContext.md
- progress.md

STEP 4 — SYNTHESIS
For each missing or outdated file:
- Propose creation or update
- Derive content strictly from observable code and config
- Do NOT invent requirements or architecture

STEP 5 — GATEWAY
Before evolving documentation:
- Pass the Context Integrity Gateway
- Escalate anomalies for confirmation

Do NOT write code yet.

Respond ONLY with:
1. Compliance confirmation
2. Documentation synthesis plan

🔄 Prompt Diario de Trabajo

As per MemoryBank.md protocol:

- Re-read all Memory Bank files
- Re-anchor to project goals and AGENTS-Constitution.md

TASK: [Descripción de la tarea]

CONSTITUTIONAL ARTICLES INVOLVED:
- Art. X — [Nombre de la regla]
- Art. Y — [Nombre de la regla]

Execute the task.

Before completion:
1. Pass the Context Integrity Gateway
2. Update:
   - activeContext.md (Cambios recientes)
   - progress.md (Registro de decisiones)
3. Confirm full constitutional compliance

Final response MUST include:
- Implementation summary
- Compliance confirmation
- Exact documentation updates

🧩 Protocolo RAGESe
Paso	Pregunta respondida	Acción
Retrieve	¿Qué sé?	Leer todos los archivos Memory Bank
Anchor	¿Qué no puede cambiar?	Anclar a los objetivos y la Constitution
Ground	¿Qué es real ahora?	Revisar el código y el estado actual
Evaluate	¿Encaja esto?	Verificar con las reglas y arquitectura
Synthesize	¿Qué se debe construir?	Generar la solución
evolve	¿Cómo lo recordamos?	Actualizar la Memory Bank
🛡️ Context Integrity Gateway

Antes de cualquier evolución de documentación:

    Validación cruzada de archivos — No se permiten contradicciones

    Registro de decisiones — La justificación debe documentarse en progress.md

    Escalado de anomalías — Cualquier realidad no documentada debe reportarse

Este es el mecanismo inmunológico del sistema contra la deriva arquitectónica.
📋 Flujo de Trabajo — Agregar una Funcionalidad

Escenario: Agregar la función de “restablecer contraseña”

1. El usuario define la tarea  
2. El agente ejecuta RAGESe:
   - Lee la Memory Bank  
   - Valida la Constitution  
   - Diseña primero la interfaz  
   - Escribe pruebas e implementación  
   - Actualiza la documentación  
3. El agente pasa por el Context Integrity Gateway  
4. Entrega código + actualizaciones de memoria

🎖️ Mejores Prácticas

    Comienza pequeño y explícito

    Personaliza la Constitution temprano

    Confía en la detección de anomalías

    Revisa regularmente progress.md

    Prioriza la claridad sobre la velocidad

🔧 Guía de Adaptación
Proyectos que no usan Python

    Modifica las secciones de runtime/herramientas en la Constitution

    Actualiza techContext.md

Diferentes Arquitecturas

    Redefine las capas en la Constitution

    Alinea con systemPatterns.md

    Mantén las reglas de dependencia

Agregar Reglas Personalizadas

    Añade nuevos artículos constitucionales

    Haz referencia a ellos en Memory Bank & Gateway

❓ FAQ

¿Necesito usar prompts largos cada vez?
No. Después de la inicialización, bastan prompts cortos basados en el protocolo.

¿Qué modelos funcionan mejor?
Modelos con grandes ventanas de contexto (GPT-4+, Claude 3.5+, etc.).

¿Es obligatoria la Clean Architecture?
No. La consistencia es obligatoria — no una arquitectura específica.

¿Escala este sistema para proyectos grandes?
Sí. Usando archivos Memory Bank jerárquicos y resúmenes.
🤝 Contribuciones

Se aceptan:

    Constitutions para otros lenguajes (Go, Rust, TypeScript, etc.)

    Herramientas de automatización y bootstrap

    Casos de estudio reales

Ver CONTRIBUTING.md.
📜 Licencia

Licencia MIT — ver LICENSE.
