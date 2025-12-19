# Memory Bank & Constitutional AI Agent System 🧠
[English](README.en.md) | [Türkçe](README.tr.md) | [Azərbaycan](README.az.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Español](README.es.md)
# Memory Bank & Constitutional AI Agent System 🧠

[English](README.en.md) | [Türkçe](README.tr.md) | [Azərbaycan](README.az.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Español](README.es.md)

> Un cadre déterministe pour transformer les LLMs en ingénieurs logiciels sans état, guidés par la documentation.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎯 Philosophie Fondamentale

Imaginez un développeur expert avec une discipline architecturale parfaite — mais souffrant d’une **amnésie totale** après chaque session.  
Pour fonctionner, il s’appuie exclusivement sur deux artefacts :

1. **Constitution (`AGENTS-Constitution.md`)**  
   La loi technique suprême du projet.

2. **Memory Bank (`MemoryBank.md` + fichiers de contexte)**  
   Un enregistrement vivant et versionné des objectifs, de l’architecture, des décisions et des progrès.

Cette contrainte devient une force :

> **Documentation parfaite · Raisonnement reproductible · Développement orienté architecture**

---

## 📁 Structure du Répertoire

```text
memory-bank/
├── MemoryBank.md           # Protocole opérationnel & framework RAGESe
├── AGENTS-Constitution.md  # Loi technique suprême (règles non négociables)
├── projectbrief.md         # Stratégie “pourquoi” et critères de succès
├── productContext.md       # Problèmes utilisateur & objectifs d’expérience
├── systemPatterns.md       # Architecture & modèles de conception
├── techContext.md          # Stack technologique, outils, contraintes
├── activeContext.md        # État actuel & focus
└── progress.md             # Journal d’évolution & historique des décisions

🚀 Démarrage Rapide
1️⃣ Cloner dans votre projet

git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
cp -r memory_bank_and_constitution/memory-bank ./memory-bank

2️⃣ Personnaliser la Constitution

Modifier memory-bank/AGENTS-Constitution.md :

    Ajuster les versions de langage/environnement

    Définir les couches architecturales

    Fixer les règles de qualité du code, de test et de conception

    ⚠️ Ce fichier agit comme la loi du projet. Modifiez-le avec prudence.

3️⃣ Initialiser le Contexte

Remplir en priorité :

    projectbrief.md — Raison d’être du projet

    techContext.md — Stack technologique utilisée

    systemPatterns.md — Architecture et limites

🤖 Premier Prompt — Boot Protocol

Utiliser exactement ce prompt pour initialiser un agent IA :

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

🔄 Prompt de Travail Quotidien

As per MemoryBank.md protocol:

- Re-read all Memory Bank files
- Re-anchor to project goals and AGENTS-Constitution.md

TASK: [Description de la tâche]

CONSTITUTIONAL ARTICLES INVOLVED:
- Art. X — [Nom de la règle]
- Art. Y — [Nom de la règle]

Execute the task.

Before completion:
1. Pass the Context Integrity Gateway
2. Update:
   - activeContext.md (Changements récents)
   - progress.md (Journal des décisions)
3. Confirm full constitutional compliance

Final response MUST include:
- Implementation summary
- Compliance confirmation
- Exact documentation updates

🧩 Protocole RAGESe
Étape	Question traitée	Action
Retrieve	Que sais-je ?	Lire tous les fichiers Memory Bank
Anchor	Qu’est-ce qui est fixe ?	S’ancrer aux objectifs & à la Constitution
Ground	Quelle est la réalité ?	Examiner le code et l’état actuels
Evaluate	Cela correspond-il ?	Vérifier les règles & l’architecture
Synthesize	Que faut-il construire ?	Produire la solution
evolve	Comment s’en souvenir ?	Mettre à jour la Memory Bank
🛡️ Context Integrity Gateway

Avant toute évolution de la documentation :

    Validation inter-fichiers — Aucune contradiction permise

    Journalisation des décisions — Raison consignée dans progress.md

    Escalade des anomalies — Les réalités non documentées doivent être signalées

C’est le système immunitaire contre la dérive architecturale.
📋 Exemple de Flux — Ajouter une Fonctionnalité

Scénario : Ajouter une fonctionnalité "réinitialisation de mot de passe"

1. L’utilisateur définit la tâche  
2. L’agent exécute le protocole RAGESe :
   - Lit la Memory Bank
   - Valide la Constitution
   - Conçoit la solution en priorité par l’interface
   - Écrit les tests et l’implémentation
   - Met à jour la documentation
3. L’agent passe le Context Integrity Gateway
4. L’agent livre le code + les mises à jour mémoire

🎖️ Bonnes Pratiques

    Commencer petit et explicite

    Personnaliser la Constitution dès le départ

    Faire confiance à la détection d’anomalies

    Revoir régulièrement progress.md

    Préférer la clarté à la vitesse

🔧 Guide d’Adaptation
Projets non-Python

    Modifier les sections runtime/outils dans la Constitution

    Mettre à jour techContext.md

Architectures Différentes

    Redéfinir les couches dans la Constitution

    Aligner avec systemPatterns.md

    Préserver les règles de dépendance

Ajouter des Règles Personnalisées

    Ajouter de nouveaux articles constitutionnels

    Les référencer dans la Memory Bank & Gateway

❓ FAQ

Dois-je utiliser de longs prompts à chaque fois ?
Non. Après l’initialisation, des prompts courts basés sur le protocole suffisent.

Quels modèles fonctionnent le mieux ?
Les modèles avec de grandes fenêtres de contexte (GPT-4+, Claude 3.5+, etc.).

Clean Architecture est-elle obligatoire ?
Non. Ce qui est obligatoire, c’est la cohérence — pas un style d’architecture particulier.

Ce système est-il évolutif pour de grands projets ?
Oui. Grâce à des fichiers Memory Bank hiérarchiques et des résumés.
🤝 Contributions

Nous acceptons :

    Des Constitutions pour d’autres langages (Go, Rust, TypeScript, etc.)

    Des outils d’automatisation et de bootstrap

    Des études de cas réelles

Voir CONTRIBUTING.md.
📜 Licence

Licence MIT — voir LICENSE.