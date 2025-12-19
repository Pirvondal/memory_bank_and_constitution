# Banque de Mémoire & Système d'Agent IA Constitutionnel 🧠

[Türkçe](README.tr.md) | [Azərbaycan](README.az.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Español](README.es.md)

> Un cadre déterministe pour transformer les LLM en ingénieurs logiciels sans état et pilotés par la documentation.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎯 Philosophie de Base

Imaginez un développeur expert avec une discipline architecturale parfaite qui souffre d'amnésie complète après chaque session.
Pour fonctionner, il s'appuie **entièrement** sur deux artefacts :

1.  **Une Constitution (`AGENTS-Constitution.md`)**
    La loi technique non négociable du projet.

2.  **Une Banque de Mémoire (`MemoryBank.md` + fichiers de contexte)**
    Un enregistrement vivant et versionné des objectifs, de l'architecture, des décisions et des progrès.

Cette contrainte devient un super-pouvoir :

> **Documentation parfaite · Raisonnement reproductible · Développement axé sur l'architecture**

---

## 📁 Structure du Référentiel

```text
memory-bank/
├── MemoryBank.md           # Protocole opérationnel & cadre RAGESe
├── AGENTS-Constitution.md  # Loi technique suprême (règles non négociables)
├── projectbrief.md         # "Pourquoi" stratégique et critères de succès
├── productContext.md       # Problèmes utilisateurs & objectifs d'expérience
├── systemPatterns.md       # Architecture & modèles de conception
├── techContext.md          # Pile technique, outils, contraintes
├── activeContext.md        # État actuel & focus
└── progress.md             # Journal d'évolution & historique des décisions
```

---

## 🚀 Démarrage Rapide

### 1️⃣ Cloner dans Votre Projet

```bash
git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
cp -r memory_bank_and_constitution/memory-bank ./memory-bank
```

### 2️⃣ Personnaliser la Constitution

Modifiez `memory-bank/AGENTS-Constitution.md` :

- Ajustez les versions de langue/d'exécution
- Définissez les couches architecturales
- Définissez les règles de qualité du code, de test et de conception

> ⚠️ Ce fichier agit comme **loi du projet**. Changez-le délibérément.

### 3️⃣ Initialiser Votre Contexte

Remplissez ceux-ci en premier :

- `projectbrief.md` — Pourquoi le projet existe
- `techContext.md` — Pile technique réelle
- `systemPatterns.md` — Architecture & limites

---

## 🤖 Première Invite — Protocole de Démarrage

Utilisez **exactement** cette invite pour initialiser un agent IA :

```text
Vous opérez sous un modèle d'exécution sans état.

ÉTAPE 1 — CHARGEMENT DE CONTEXTE OBLIGATOIRE
Lisez et internalisez les fichiers suivants du répertoire `memory-bank/` :
1. MemoryBank.md
2. AGENTS-Constitution.md

Ne procédez pas tant que les deux ne sont pas entièrement lus.

ÉTAPE 2 — RECONNAISSANCE
Confirmez explicitement :
- Vous avez lu et compris les deux fichiers
- Vous acceptez RAGESe, la Passerelle d'Intégrité du Contexte et l'autorité constitutionnelle
- Vous ne supposerez aucune connaissance non documentée

ÉTAPE 3 — ANALYSE DU PROJET
Analysez la base de code existante.
Identifiez si ces fichiers existent et sont exacts :
- projectbrief.md
- productContext.md
- systemPatterns.md
- techContext.md
- activeContext.md
- progress.md

ÉTAPE 4 — SYNTHÈSE
Pour chaque fichier manquant ou obsolète :
- Proposez la création ou la mise à jour
- Dérivez le contenu strictement du code et de la configuration observables
- N'INVENTEZ PAS d'exigences ou d'architecture

ÉTAPE 5 — PASSERELLE
Avant d'évoluer la documentation :
- Passez la Passerelle d'Intégrité du Contexte
- Escaladez les anomalies pour confirmation

N'écrivez PAS encore de code.

Répondez UNIQUEMENT avec :
1. Confirmation de conformité
2. Plan de synthèse de la documentation
```

---

## 🔄 Invite de Travail Quotidienne

```text
Selon le protocole MemoryBank.md :

- Relisez tous les fichiers de la Banque de Mémoire
- Ré-ancrez aux objectifs du projet et à AGENTS-Constitution.md

TÂCHE : [Décrivez la tâche]

ARTICLES CONSTITUTIONNELS IMPLIQUÉS :
- Art. X — [Nom de la règle]
- Art. Y — [Nom de la règle]

Exécutez la tâche.

Avant l'achèvement :
1. Passez la Passerelle d'Intégrité du Contexte
2. Mettez à jour :
   - activeContext.md (Changements Récents)
   - progress.md (Journal des Décisions)
3. Confirmez la pleine conformité constitutionnelle

La réponse finale DOIT inclure :
- Résumé de l'implémentation
- Confirmation de conformité
- Mises à jour exactes de la documentation
```

---

## 🧩 Protocole RAGESe

| Étape      | Question Répondue        | Action                                   |
|------------|--------------------------|------------------------------------------|
| Retrieve   | Que sais-je ?            | Lire TOUS les fichiers de la Banque de Mémoire |
| Anchor     | Qu'est-ce qui ne peut pas changer ? | Verrouiller sur les objectifs & la Constitution |
| Ground     | Qu'est-ce qui est réel maintenant ? | Inspecter le code & l'état réels         |
| Evaluate   | Est-ce que cela correspond ? | Vérifier les règles & l'architecture     |
| Synthesize | Que faut-il construire ? | Produire une solution                    |
| evolve     | Comment nous souvenons-nous ? | Mettre à jour la Banque de Mémoire       |

---

## 🛡️ Passerelle d'Intégrité du Contexte

Avant toute évolution de la documentation :

- **Validation inter-fichiers** — Aucune contradiction autorisée
- **Journalisation des décisions** — Justifications enregistrées dans `progress.md`
- **Escalade des anomalies** — La réalité non documentée doit être signalée

C'est la réponse immunitaire du système contre la dérive architecturale.

---

## 📋 Exemple de Flux de Travail — Ajout d'une Fonctionnalité

```text
Scénario : Ajouter la fonctionnalité "réinitialisation du mot de passe"

1. L'utilisateur émet l'invite de tâche
2. L'agent exécute RAGESe :
   - Lit la Banque de Mémoire
   - Valide la Constitution
   - Conçoit d'abord la solution d'interface
   - Écrit les tests et l'implémentation
   - Met à jour la documentation
3. L'agent passe la Passerelle d'Intégrité du Contexte
4. L'agent livre le code + les mises à jour de mémoire
```

---

## 🎖️ Meilleures Pratiques

- Commencez petit et explicite
- Personnalisez la Constitution tôt
- Faites confiance à la détection d'anomalies
- Examinez `progress.md` régulièrement
- Préférez la clarté à la vitesse

---

## 🔧 Guide d'Adaptation

### Projets Non-Python
- Modifiez les sections runtime/outils de la Constitution
- Mettez à jour `techContext.md` en conséquence

### Architectures Différentes
- Redéfinissez les couches dans la Constitution
- Alignez `systemPatterns.md`
- Préservez les règles de dépendance

### Ajout de Règles Personnalisées
- Ajoutez de nouveaux articles constitutionnels
- Référencez-les dans la Banque de Mémoire & la Passerelle

---

## ❓ FAQ

**Ai-je besoin de longues invites à chaque fois ?**
Non. Après le démarrage, de courtes invites basées sur le protocole suffisent.

**Quels modèles fonctionnent le mieux ?**
Les modèles avec de grandes fenêtres de contexte (GPT-4+, Claude 3.5+, etc.).

**La Clean Architecture est-elle obligatoire ?**
Non. La cohérence est obligatoire — pas une architecture spécifique.

**Cela peut-il passer à l'échelle pour de grands projets ?**
Oui. Utilisez des fichiers de Banque de Mémoire hiérarchiques et des résumés.

---

## 🤝 Contribuer

Nous accueillons :
- Constitutions pour d'autres langues (Go, Rust, TypeScript)
- Outils d'automatisation & d'amorçage
- Études de cas du monde réel

Voir `CONTRIBUTING.md`.

---

## 📜 Licence

Licence MIT — voir `LICENSE`.
