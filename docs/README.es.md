# Banco de Memoria & Sistema de Agente de IA Constitucional 🧠

[Türkçe](README.tr.md) | [Azərbaycan](README.az.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Español](README.es.md)

> Un marco determinista para transformar los LLM en ingenieros de software sin estado y guiados por documentación.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎯 Filosofía Central

Imagine un desarrollador experto con una disciplina arquitectónica perfecta que sufre amnesia completa después de cada sesión.
Para funcionar, confía **completamente** en dos artefactos:

1.  **Una Constitución (`AGENTS-Constitution.md`)**
    La ley técnica no negociable del proyecto.

2.  **Un Banco de Memoria (`MemoryBank.md` + archivos de contexto)**
    Un registro vivo y versionado de objetivos, arquitectura, decisiones y progreso.

Esta restricción se convierte en un superpoder:

> **Documentación perfecta · Razonamiento reproducible · Desarrollo guiado por la arquitectura**

---

## 📁 Estructura del Repositorio

```text
memory-bank/
├── MemoryBank.md           # Protocolo operativo & marco RAGESe
├── AGENTS-Constitution.md  # Ley técnica suprema (reglas no negociables)
├── projectbrief.md         # "Por qué" estratégico y criterios de éxito
├── productContext.md       # Problemas del usuario & objetivos de experiencia
├── systemPatterns.md       # Arquitectura & patrones de diseño
├── techContext.md          # Pila tecnológica, herramientas, restricciones
├── activeContext.md        # Estado actual & enfoque
└── progress.md             # Registro de evolución & historial de decisiones
```

---

## 🚀 Inicio Rápido

### 1️⃣ Clonar en Su Proyecto

```bash
git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
cp -r memory_bank_and_constitution/memory-bank ./memory-bank
```

### 2️⃣ Personalizar la Constitución

Edite `memory-bank/AGENTS-Constitution.md`:

- Ajuste las versiones de lenguaje/tiempo de ejecución
- Defina las capas arquitectónicas
- Establezca reglas de calidad de código, pruebas y diseño

> ⚠️ Este archivo actúa como **ley del proyecto**. Cámbielo deliberadamente.

### 3️⃣ Inicializar Su Contexto

Llene estos primero:

- `projectbrief.md` — Por qué existe el proyecto
- `techContext.md` — Pila tecnológica real
- `systemPatterns.md` — Arquitectura & límites

---

## 🤖 Primer Prompt — Protocolo de Arranque

Use **exactamente** este prompt para inicializar un agente de IA:

```text
Usted está operando bajo un modelo de ejecución sin estado.

PASO 1 — CARGA DE CONTEXTO OBLIGATORIA
Lea e interiorice los siguientes archivos del directorio `memory-bank/`:
1. MemoryBank.md
2. AGENTS-Constitution.md

No proceda hasta que ambos sean leídos completamente.

PASO 2 — RECONOCIMIENTO
Confirme explícitamente:
- Ha leído y entendido ambos archivos
- Acepta RAGESe, la Puerta de Enlace de Integridad del Contexto y la autoridad constitucional
- No asumirá ningún conocimiento no documentado

PASO 3 — ANÁLISIS DEL PROYECTO
Escanee la base de código existente.
Identifique si estos archivos existen y son precisos:
- projectbrief.md
- productContext.md
- systemPatterns.md
- techContext.md
- activeContext.md
- progress.md

PASO 4 — SÍNTESIS
Para cada archivo faltante o desactualizado:
- Proponga creación o actualización
- Derive contenido estrictamente de código y configuración observables
- NO INVENTE requisitos o arquitectura

PASO 5 — PUERTA DE ENLACE
Antes de evolucionar la documentación:
- Pase la Puerta de Enlace de Integridad del Contexto
- Escale anomalías para confirmación

NO escriba código todavía.

Responda SOLO con:
1. Confirmación de cumplimiento
2. Plan de síntesis de documentación
```

---

## 🔄 Prompt de Trabajo Diario

```text
Según el protocolo MemoryBank.md:

- Relea todos los archivos del Banco de Memoria
- Reanclese a los objetivos del proyecto y AGENTS-Constitution.md

TAREA: [Describa la tarea]

ARTÍCULOS CONSTITUCIONALES INVOLUCRADOS:
- Art. X — [Nombre de la regla]
- Art. Y — [Nombre de la regla]

Ejecute la tarea.

Antes de completar:
1. Pase la Puerta de Enlace de Integridad del Contexto
2. Actualice:
   - activeContext.md (Cambios Recientes)
   - progress.md (Registro de Decisiones)
3. Confirme el cumplimiento constitucional total

La respuesta final DEBE incluir:
- Resumen de implementación
- Confirmación de cumplimiento
- Actualizaciones exactas de documentación
```

---

## 🧩 Protocolo RAGESe

| Paso       | Pregunta Respondida      | Acción                                   |
|------------|--------------------------|------------------------------------------|
| Retrieve   | ¿Qué sé?                 | Leer TODOS los archivos del Banco de Memoria |
| Anchor     | ¿Qué no puede cambiar?   | Bloquear en objetivos & Constitución     |
| Ground     | ¿Qué es real ahora?      | Inspeccionar código & estado real        |
| Evaluate   | ¿Encaja esto?            | Comprobar reglas & arquitectura          |
| Synthesize | ¿Qué se debe construir?  | Producir solución                        |
| evolve     | ¿Cómo recordamos?        | Actualizar Banco de Memoria              |

---

## 🛡️ Puerta de Enlace de Integridad del Contexto

Antes de cualquier evolución de documentación:

- **Validación entre archivos** — No se permiten contradicciones
- **Registro de decisiones** — Racionales registrados en `progress.md`
- **Escalada de anomalías** — La realidad no documentada debe ser marcada

Esta es la respuesta inmune del sistema contra la deriva arquitectónica.

---

## 📋 Flujo de Trabajo de Ejemplo — Agregar una Función

```text
Escenario: Agregar función "restablecimiento de contraseña"

1. El usuario emite el prompt de tarea
2. El agente ejecuta RAGESe:
   - Lee el Banco de Memoria
   - Valida la Constitución
   - Diseña primero la solución de interfaz
   - Escribe pruebas e implementación
   - Actualiza la documentación
3. El agente pasa la Puerta de Enlace de Integridad del Contexto
4. El agente entrega código + actualizaciones de memoria
```

---

## 🎖️ Mejores Prácticas

- Comience pequeño y explícito
- Personalice la Constitución temprano
- Confíe en la detección de anomalías
- Revise `progress.md` regularmente
- Prefiera la claridad sobre la velocidad

---

## 🔧 Guía de Adaptación

### Proyectos No-Python
- Modifique las secciones de tiempo de ejecución/herramientas de la Constitución
- Actualice `techContext.md` en consecuencia

### Arquitecturas Diferentes
- Redefina capas en la Constitución
- Alinee `systemPatterns.md`
- Preserve las reglas de dependencia

### Agregar Reglas Personalizadas
- Agregue nuevos artículos constitucionales
- Referéncielos en el Banco de Memoria & Puerta de Enlace

---

## ❓ Preguntas Frecuentes

**¿Necesito prompts largos cada vez?**
No. Después del arranque, los prompts cortos basados en protocolos son suficientes.

**¿Qué modelos funcionan mejor?**
Modelos con grandes ventanas de contexto (GPT-4+, Claude 3.5+, etc.).

**¿Es obligatoria la Clean Architecture?**
No. La consistencia es obligatoria — no una arquitectura específica.

**¿Puede esto escalar a grandes proyectos?**
Sí. Use archivos de Banco de Memoria jerárquicos y resúmenes.

---

## 🤝 Contribución

Damos la bienvenida a:
- Constituciones para otros lenguajes (Go, Rust, TypeScript)
- Herramientas de automatización & arranque
- Estudios de caso del mundo real

Ver `CONTRIBUTING.md`.

---

## 📜 Licencia

Licencia MIT — ver `LICENSE`.
