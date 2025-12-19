# Memory Bank & Constitutional AI Agent System 🧠

[English](README.en.md) | [Türkçe](README.tr.md) | [Azərbaycan](README.az.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Español](README.es.md)

> Ein deterministisches Framework, um LLMs in zustandslose, dokumentationsgetriebene Softwareingenieure zu verwandeln.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎯 Grundphilosophie

Stellen Sie sich einen erfahrenen Entwickler mit perfekter architektonischer Disziplin vor – der jedoch nach jeder Sitzung **sein Gedächtnis verliert**.  
Um zu funktionieren, verlässt er sich ausschließlich auf zwei Artefakte:

1. **Constitution (`AGENTS-Constitution.md`)**  
   Das unverrückbare technische Gesetz des Projekts.

2. **Memory Bank (`MemoryBank.md` + Kontextdateien)**  
   Ein lebendiges, versioniertes Protokoll von Zielen, Architektur, Entscheidungen und Fortschritt.

Diese Einschränkung wird zu einer Superkraft:

> **Perfekte Dokumentation · Reproduzierbares Denken · Architekturorientierte Entwicklung**

---

## 📁 Repository-Struktur

```text
memory-bank/
├── MemoryBank.md           # Betriebliches Protokoll & RAGESe-Framework
├── AGENTS-Constitution.md  # Oberstes technisches Gesetz (unverhandelbare Regeln)
├── projectbrief.md         # Strategisches „Warum“ und Erfolgskriterien
├── productContext.md       # Benutzerprobleme & Erfahrungsziele
├── systemPatterns.md       # Architektur- & Designmuster
├── techContext.md          # Technologiestack, Tools, Einschränkungen
├── activeContext.md        # Aktueller Zustand & Fokus
└── progress.md             # Entwicklungsprotokoll & Entscheidungshistorie

🚀 Schnellstart
1️⃣ In dein Projekt klonen

git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
cp -r memory_bank_and_constitution/memory-bank ./memory-bank

2️⃣ Constitution anpassen

Bearbeite memory-bank/AGENTS-Constitution.md:

    Sprache/Runtime-Versionen anpassen

    Architekturschichten definieren

    Regeln für Codequalität, Tests und Design festlegen

    ⚠️ Diese Datei ist das Gesetz des Projekts. Änderungen nur bewusst vornehmen.

3️⃣ Kontext initialisieren

Fülle zuerst diese Dateien aus:

    projectbrief.md — Warum das Projekt existiert

    techContext.md — Verwendeter Technologiestack

    systemPatterns.md — Architektur und Grenzen

🤖 Erstes Prompt — Boot Protocol

Verwende genau dieses Prompt, um den AI-Agenten zu initialisieren:

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

🔄 Tägliches Arbeits-Prompt

As per MemoryBank.md protocol:

- Re-read all Memory Bank files
- Re-anchor to project goals and AGENTS-Constitution.md

TASK: [Beschreibung der Aufgabe]

CONSTITUTIONAL ARTICLES INVOLVED:
- Art. X — [Regelname]
- Art. Y — [Regelname]

Execute the task.

Before completion:
1. Pass the Context Integrity Gateway
2. Update:
   - activeContext.md (Letzte Änderungen)
   - progress.md (Entscheidungslog)
3. Confirm full constitutional compliance

Final response MUST include:
- Implementation summary
- Compliance confirmation
- Exact documentation updates

🧩 RAGESe-Protokoll
Schritt	Beantwortete Frage	Aktion
Retrieve	Was weiß ich?	Alle Memory Bank-Dateien lesen
Anchor	Was darf sich nicht ändern?	An Zielen & Constitution verankern
Ground	Was ist aktuell real?	Code & Zustand prüfen
Evaluate	Passt das?	Mit Regeln & Architektur abgleichen
Synthesize	Was soll gebaut werden?	Lösung generieren
evolve	Wie behalten wir es?	Memory Bank aktualisieren
🛡️ Context Integrity Gateway

Vor jeder Dokumentationsänderung:

    Cross-Datei-Validierung — Keine Widersprüche erlaubt

    Entscheidungsprotokoll — Begründung in progress.md festhalten

    Anomalie-Eskalation — Nicht dokumentierte Fakten melden

Dies ist das Immunsystem des Systems gegen architektonische Drift.
📋 Beispiel-Workflow — Eine Funktion hinzufügen

Szenario: „Passwort-zurücksetzen“-Funktion hinzufügen

1. Benutzer beschreibt die Aufgabe  
2. Agent führt RAGESe aus:
   - Liest Memory Bank
   - Validiert Constitution
   - Entwirft die Schnittstelle
   - Schreibt Tests und Implementierung
   - Aktualisiert Dokumentation
3. Agent passiert Context Integrity Gateway
4. Agent liefert Code + Memory-Updates

🎖️ Beste Praktiken

    Klein und explizit starten

    Constitution früh anpassen

    Anomalie-Erkennung vertrauen

    progress.md regelmäßig prüfen

    Klarheit vor Geschwindigkeit stellen

🔧 Anpassungsleitfaden
Nicht-Python-Projekte

    Runtime/Tooling in Constitution anpassen

    techContext.md entsprechend aktualisieren

Verschiedene Architekturen

    Schichten in Constitution neu definieren

    Mit systemPatterns.md abgleichen

    Abhängigkeitsregeln beibehalten

Eigene Regeln hinzufügen

    Neue konstitutionelle Artikel hinzufügen

    Diese in Memory Bank & Gateway referenzieren

❓ FAQ

Muss ich jedes Mal lange Prompts verwenden?
Nein. Nach der Initialisierung reichen kurze, protokollbasierte Prompts aus.

Welche Modelle funktionieren am besten?
Modelle mit großem Kontextfenster (GPT-4+, Claude 3.5+, usw.).

Ist Clean Architecture Pflicht?
Nein. Konsistenz ist Pflicht — nicht ein bestimmter Architekturstil.

Skaliert das System für große Projekte?
Ja. Mit hierarchischen Memory Bank-Dateien und Zusammenfassungen.
🤝 Beiträge

Willkommen sind:

    Constitutions für andere Sprachen (Go, Rust, TypeScript usw.)

    Automatisierungs- & Bootstrap-Tools

    Praxisbeispiele

Siehe CONTRIBUTING.md.
📜 Lizenz

MIT-Lizenz — siehe LICENSE.