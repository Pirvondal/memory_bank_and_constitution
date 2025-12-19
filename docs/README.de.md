# Memory Bank & Constitutional AI Agent System 🧠

[Türkçe](README.tr.md) | [Azərbaycan](README.az.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Español](README.es.md)

> Ein deterministisches Framework zur Transformation von LLMs in stateless (zustandslose), documentation-driven Software Engineers.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎯 Kernphilosophie

Stellen Sie sich einen Expertenentwickler mit perfekter architektonischer Disziplin vor, der nach jeder Sitzung einen vollständigen Gedächtnisverlust erleidet.
Um zu funktionieren, verlässt er sich **vollständig** auf zwei Artefakte:

1.  **Eine Constitution (`AGENTS-Constitution.md`)**
    Das nicht verhandelbare technische Gesetz des Projekts.

2.  **Eine Memory Bank (`MemoryBank.md` + Context-Dateien)**
    Ein lebendiger, versionierter Datensatz von Zielen, Architektur, Entscheidungen und Fortschritten.

Diese Einschränkung wird zu einer Superkraft:

> **Perfekte Dokumentation · Reproduzierbare Argumentation · Architecture-first development**

---

## 📁 Repository-Struktur

```text
memory-bank/
├── MemoryBank.md           # Betriebsprotokoll & RAGESe-Framework
├── AGENTS-Constitution.md  # Oberstes technisches Gesetz (nicht verhandelbare Regeln)
├── projectbrief.md         # Strategisches "Warum" und Erfolgskriterien
├── productContext.md       # Benutzerprobleme & Erlebnisziele
├── systemPatterns.md       # Architektur & Design Patterns
├── techContext.md          # Tech-Stack, Tools, Einschränkungen
├── activeContext.md        # Aktueller Status & Fokus
└── progress.md             # Evolutionslog & Entscheidungshistorie
```

---

## 🚀 Quick Start

### 1️⃣ In Ihr Projekt klonen

```bash
git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
cp -r memory_bank_and_constitution/memory-bank ./memory-bank
```

### 2️⃣ Die Constitution anpassen

Bearbeiten Sie `memory-bank/AGENTS-Constitution.md`:

- Sprach-/Runtime-Versionen anpassen
- Architekturschichten definieren
- Regeln für Codequalität, Tests und Design festlegen

> ⚠️ Diese Datei fungiert als **Projektgesetz**. Ändern Sie sie bewusst.

### 3️⃣ Ihren Context initialisieren

Füllen Sie diese zuerst aus:

- `projectbrief.md` — Warum das Projekt existiert
- `techContext.md` — Tatsächlicher Tech-Stack
- `systemPatterns.md` — Architektur & Grenzen

---

## 🤖 Erster Prompt — Boot Protocol

Verwenden Sie **exakt** diesen Prompt, um einen KI-Agenten zu initialisieren:

```text
Sie arbeiten unter einem stateless Execution Model.

SCHRITT 1 — OBLIGATORISCHES CONTEXT LOAD
Lesen und verinnerlichen Sie die folgenden Dateien aus dem Verzeichnis `memory-bank/`:
1. MemoryBank.md
2. AGENTS-Constitution.md

Fahren Sie nicht fort, bis beide vollständig gelesen sind.

SCHRITT 2 — ACKNOWLEDGEMENT (BESTÄTIGUNG)
Bestätigen Sie ausdrücklich:
- Sie haben beide Dateien gelesen und verstanden
- Sie akzeptieren RAGESe, das Context Integrity Gateway und die constitutional Autorität
- Sie werden kein undokumentiertes Wissen voraussetzen

SCHRITT 3 — PROJECT ANALYSE
Scannen Sie die vorhandene Codebasis.
Stellen Sie fest, ob diese Dateien existieren und korrekt sind:
- projectbrief.md
- productContext.md
- systemPatterns.md
- techContext.md
- activeContext.md
- progress.md

SCHRITT 4 — SYNTHESE
Für jede fehlende oder veraltete Datei:
- Schlagen Sie Erstellung oder Aktualisierung vor
- Leiten Sie Inhalte strikt aus beobachtbarem Code und Konfiguration ab
- ERFINDEN Sie KEINE Anforderungen oder Architektur

SCHRITT 5 — GATEWAY
Vor der Weiterentwicklung der Dokumentation:
- Passieren Sie das Context Integrity Gateway
- Eskalieren Sie Anomalien zur Bestätigung

Schreiben Sie noch KEINEN Code.

Antworten Sie NUR mit:
1. Konformitätsbestätigung
2. Dokumentationssyntheseplan
```

---

## 🔄 Täglicher Work Prompt

```text
Gemäß MemoryBank.md-Protokoll:

- Lesen Sie alle Memory Bank-Dateien erneut
- Verankern Sie sich erneut in den Projektzielen und AGENTS-Constitution.md

TASK: [Beschreiben Sie die Aufgabe]

BETEILIGTE CONSTITUTIONAL ARTIKEL:
- Art. X — [Regelname]
- Art. Y — [Regelname]

Führen Sie die Aufgabe aus.

Vor Abschluss:
1. Passieren Sie das Context Integrity Gateway
2. Aktualisieren Sie:
   - activeContext.md (Kürzliche Änderungen)
   - progress.md (Entscheidungslog)
3. Bestätigen Sie die volle constitutional Konformität

Die endgültige Antwort MUSS beinhalten:
- Implementierungszusammenfassung
- Konformitätsbestätigung
- Exakte Dokumentationsaktualisierungen
```

---

## 🧩 RAGESe-Protokoll

| Schritt    | Beantwortete Frage       | Aktion                                   |
|------------|--------------------------|------------------------------------------|
| Retrieve   | Was weiß ich?            | Lies ALLE Memory Bank-Dateien             |
| Anchor     | Was darf sich nicht ändern? | An Ziele & Constitution binden              |
| Ground     | Was ist jetzt real?      | Tatsächlichen Code & Zustand inspizieren  |
| Evaluate   | Passt das?               | Regeln & Architektur prüfen               |
| Synthesize | Was soll gebaut werden?  | Lösung produzieren                        |
| evolve     | Wie erinnern wir uns?    | Memory Bank aktualisieren                 |

---

## 🛡️ Context Integrity Gateway

Vor jeder Dokumentationsevolution:

- **Dateiübergreifende Validierung** — Keine Widersprüche erlaubt
- **Entscheidungsprotokollierung** — Begründungen in `progress.md` aufgezeichnet
- **Anomalie-Eskalation** — Undokumentierte Realität muss gekennzeichnet werden

Dies ist die Immunreaktion des Systems gegen architektonischen Drift.

---

## 📋 Beispiel-Workflow — Feature hinzufügen

```text
Szenario: "Passwort-Reset"-Funktion hinzufügen

1. Benutzer gibt Aufgabenprompt aus
2. Agent führt RAGESe aus:
   - Liest Memory Bank
   - Validiert Constitution
   - Entwirft zuerst Interface-Lösung
   - Schreibt Tests und Implementierung
   - Aktualisiert Dokumentation
3. Agent passiert Context Integrity Gateway
4. Agent liefert Code + Speicheraktualisierungen
```

---

## 🎖️ Best Practices

- Beginnen Sie klein und explizit
- Passen Sie die Constitution frühzeitig an
- Vertrauen Sie der Anomalieerkennung
- Überprüfen Sie `progress.md` regelmäßig
- Bevorzugen Sie Klarheit vor Geschwindigkeit

---

## 🔧 Anpassungsleitfaden

### Nicht-Python-Projekte
- Ändern Sie die Abschnitte zu Runtime/Tools in der Constitution
- Aktualisieren Sie `techContext.md` entsprechend

### Andere Architekturen
- Definieren Sie Schichten in der Constitution neu
- Richten Sie `systemPatterns.md` aus
- Bewahren Sie Abhängigkeitsregeln

### Hinzufügen eigener Regeln
- Fügen Sie neue Constitutional Artikel hinzu
- Verweisen Sie in Memory Bank & Gateway darauf

---

## ❓ FAQ

**Brauche ich jedes Mal lange Prompts?**
Nein. Nach dem Booten reichen kurze Protokoll-basierte Prompts aus.

**Welche Modelle funktionieren am besten?**
Modelle mit großen Context Windows (GPT-4+, Claude 3.5+, usw.).

**Ist Clean Architecture obligatorisch?**
Nein. Konsistenz ist obligatorisch — keine spezifische Architektur.

**Kann dies auf große Projekte skalieren?**
Ja. Verwenden Sie hierarchische Memory Bank-Dateien und Zusammenfassungen.

---

## 🤝 Contributing

Wir begrüßen:
- Constitutions für andere Sprachen (Go, Rust, TypeScript)
- Automatisierungs- & Boot-Tools
- Fallstudien aus der realen Welt

Siehe `CONTRIBUTING.md`.

---

## 📜 Lizenz

MIT-Lizenz — siehe `LICENSE`.
