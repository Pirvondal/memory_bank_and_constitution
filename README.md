# Memory Bank & Constitutional AI Agent System 🧠

 [Türkçe](docs/README.tr.md) | [Azərbaycan](docs/README.az.md) | [Deutsch](docs/README.de.md) | [Français](docs/README.fr.md) | [Español](docs/README.es.md)

> A deterministic framework for transforming LLMs into stateless, documentation-driven software engineers.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎯 Core Philosophy

Imagine an expert developer with perfect architectural discipline who suffers complete amnesia after every session.  
To function, they rely **entirely** on two artifacts:

1. **A Constitution (`AGENTS-Constitution.md`)**  
   The non-negotiable technical law of the project.

2. **A Memory Bank (`MemoryBank.md` + context files)**  
   A living, versioned record of goals, architecture, decisions, and progress.

This constraint becomes a superpower:

> **Perfect documentation · Reproducible reasoning · Architecture-first development**

---

## 📁 Repository Structure

```text
memory-bank/
├── MemoryBank.md           # Operational protocol & RAGESe framework
├── AGENTS-Constitution.md  # Supreme technical law (non-negotiable rules)
├── projectbrief.md         # Strategic "why" and success criteria
├── productContext.md       # User problems & experience goals
├── systemPatterns.md       # Architecture & design patterns
├── techContext.md          # Tech stack, tools, constraints
├── activeContext.md        # Current state & focus
└── progress.md             # Evolution log & decision history
```

---

## 🚀 Quick Start

### 1️⃣ Clone Into Your Project

```bash
git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
cp -r memory_bank_and_constitution/memory-bank ./memory-bank
```

### 2️⃣ Customize the Constitution

Edit `memory-bank/AGENTS-Constitution.md`:

- Adjust language/runtime versions
- Define architectural layers
- Set code quality, testing, and design rules

> ⚠️ This file acts as **project law**. Change it deliberately.

### 3️⃣ Initialize Your Context

Fill these first:

- `projectbrief.md` — Why the project exists
- `techContext.md` — Actual tech stack
- `systemPatterns.md` — Architecture & boundaries

---

## 🤖 First Prompt — Boot Protocol

Use **exactly** this prompt to initialize an AI agent:

```text
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
```

---

## 🔄 Daily Work Prompt

```text
As per MemoryBank.md protocol:

- Re-read all Memory Bank files
- Re-anchor to project goals and AGENTS-Constitution.md

TASK: [Describe the task]

CONSTITUTIONAL ARTICLES INVOLVED:
- Art. X — [Rule name]
- Art. Y — [Rule name]

Execute the task.

Before completion:
1. Pass the Context Integrity Gateway
2. Update:
   - activeContext.md (Recent Changes)
   - progress.md (Decision Log)
3. Confirm full constitutional compliance

Final response MUST include:
- Implementation summary
- Compliance confirmation
- Exact documentation updates
```

---

## 🧩 RAGESe Protocol

| Step       | Question Answered        | Action                                  |
|------------|--------------------------|------------------------------------------|
| Retrieve   | What do I know?          | Read ALL Memory Bank files                |
| Anchor     | What cannot change?      | Lock to goals & Constitution              |
| Ground     | What is real right now?  | Inspect actual code & state               |
| Evaluate   | Does this fit?           | Check rules & architecture                |
| Synthesize | What should be built?    | Produce solution                          |
| evolve     | How do we remember?      | Update Memory Bank                        |

---

## 🛡️ Context Integrity Gateway

Before any documentation evolution:

- **Cross-file validation** — No contradictions allowed
- **Decision logging** — Rationale recorded in `progress.md`
- **Anomaly escalation** — Undocumented reality must be flagged

This is the system’s immune response against architectural drift.

---

## 📋 Example Workflow — Adding a Feature

```text
Scenario: Add "password reset" feature

1. User issues task prompt
2. Agent executes RAGESe:
   - Reads Memory Bank
   - Validates Constitution
   - Designs interface-first solution
   - Writes tests and implementation
   - Updates documentation
3. Agent passes Context Integrity Gateway
4. Agent delivers code + memory updates
```

---

## 🎖️ Best Practices

- Start small and explicit
- Customize Constitution early
- Trust anomaly detection
- Review `progress.md` regularly
- Prefer clarity over speed

---

## 🔧 Adaptation Guide

### Non-Python Projects
- Modify Constitution runtime/tooling sections
- Update `techContext.md` accordingly

### Different Architectures
- Redefine layers in Constitution
- Align `systemPatterns.md`
- Preserve dependency rules

### Adding Custom Rules
- Add new constitutional articles
- Reference them in Memory Bank & Gateway

---

## ❓ FAQ

**Do I need long prompts every time?**  
No. After boot, short protocol-based prompts are sufficient.

**Which models work best?**  
Models with large context windows (GPT-4+, Claude 3.5+, etc.).

**Is Clean Architecture mandatory?**  
No. Consistency is mandatory — not a specific architecture.

**Can this scale to large projects?**  
Yes. Use hierarchical Memory Bank files and summaries.

---

## 🤝 Contributing

We welcome:
- Constitutions for other languages (Go, Rust, TypeScript)
- Automation & bootstrap tools
- Real-world case studies

See `CONTRIBUTING.md`.

---

## 📜 License

MIT License — see `LICENSE`.
