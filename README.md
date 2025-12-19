markdown

# Memory Bank & Constitutional AI Agent System 🧠

> A deterministic framework for transforming LLMs into stateless, documentation-driven software engineers.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

## 🎯 Core Philosophy

Imagine an expert developer with perfect architectural discipline who suffers complete amnesia after every session. To function, they rely **entirely** on:
1. **A Constitution** (`AGENTS-Constitution.md`) - The unbreakable law of the project
2. **A Memory Bank** - A living record of goals, context, progress, and decisions

This constraint becomes a superpower: **perfect documentation, reproducible reasoning, and architecture-first development.**

## 📁 Repository Structure

memory-bank/
├── MemoryBank.md # Operational protocol & RAGESe framework
├── AGENTS-Constitution.md # Supreme technical law (non-negotiable rules)
├── projectbrief.md # Strategic "why" and core goals
├── productContext.md # User problems & experience
├── systemPatterns.md # Architecture & design patterns
├── techContext.md # Tech stack & tools
├── activeContext.md # Current state & recent changes
└── progress.md # Evolution log & decision history
text


## 🚀 Quick Start

### 1. Clone into Your Project
```bash
git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
cp -r memory_bank_and_constitution/memory-bank ./memory-bank

2. Customize the Constitution

Edit memory-bank/AGENTS-Constitution.md:

    Adjust Python version (if needed)

    Modify project structure layers

    Set your own code quality rules

3. Initialize Your Context

Fill these key files first:

    projectbrief.md - Why this project exists

    techContext.md - Your actual tech stack

    systemPatterns.md - Your architecture

🤖 First Prompt: Boot Protocol

Copy this exact prompt to start:
text

You are operating under a stateless execution model.

STEP 1 — MANDATORY CONTEXT LOAD
Read and internalize the following files from the `memory-bank/` directory:
1. MemoryBank.md
2. AGENTS-Constitution.md

Do not proceed until both are fully read.

STEP 2 — ACKNOWLEDGEMENT
Explicitly confirm the following in your response:
- That you have read MemoryBank.md and AGENTS-Constitution.md
- That you understand and accept RAGESe, the Context Integrity Gateway, and the constitutional authority of AGENTS-Constitution.md
- That you will not assume any undocumented knowledge

STEP 3 — PROJECT ANALYSIS
Scan the existing project codebase and structure.
Based strictly on observable reality (not assumptions), identify whether the following Memory Bank files exist and are accurate:
- projectbrief.md
- productContext.md
- systemPatterns.md
- techContext.md
- activeContext.md
- progress.md

STEP 4 — SYNTHESIS
For each missing or outdated file:
- Propose creating or updating it
- Derive its content from:
  - Existing code
  - Project structure
  - Tests
  - Configuration files
- Do NOT invent requirements or architecture

STEP 5 — GATEWAY
Before evolving any documentation, pass the Context Integrity Gateway.
If undocumented reality or contradictions are found:
- STOP
- Document them as Context Anomalies
- Escalate for confirmation before proceeding

Do not write code yet.
Do not optimize.
Do not refactor.

First respond ONLY with:
1. Confirmation of compliance
2. A clear plan for documentation synthesis

🔄 Follow-up Prompts (Daily Work)
markdown

As per MemoryBank.md protocol, reconfirm your operational state:
- Re-read all Memory Bank core files.
- Re-anchor to project goals and AGENTS-Constitution.md.

TASK: [Your specific task here]
CONSTITUTIONAL ARTICLES: This task directly implicates:
- Art. 2 (Layered Structure): New code must be placed in correct layers.
- Art. 4 (Dependency Law): Depend on abstractions, not concretions.
- Art. 7 (Testing Law): Mandatory unit tests required.

Execute the task.
**Before reporting completion, you MUST:**
1. Pass the Context Integrity Gateway for any changed or new context.
2. Update documentation as a first-class artifact:
   - activeContext.md: Log the change under "Recent Changes"
   - progress.md: Add a "Decision Log" entry with rationale
3. Ensure all code complies with all triggered Constitutional Articles.

Your final response must include:
- Summary of implementation steps
- Confirmation of Constitutional compliance
- Exact copy of the updates made to activeContext.md and progress.md

🧩 The RAGESe Protocol

The agent's operational cycle defined in MemoryBank.md:
Step	Question Answered	Action
Retrieve	"What do I know?"	Read ALL Memory Bank files
Anchor	"What can't change?"	Lock to project goals & Constitution
Ground	"What's real now?"	Base decisions on actual code
Evaluate	"Does this fit?"	Check against rules & patterns
Synthesize	"What to build?"	Generate solutions
evolve	"How to remember?"	Update Memory Bank
🛡️ Context Integrity Gateway

The quality gate before any documentation update requires:

    Cross-file validation - Changes must be consistent across all files

    Decision logging - Every significant change gets rationale in progress.md

    Anomaly escalation - Contradictions are flagged immediately

📋 Example Workflow: Adding a Feature
python

# Scenario: Add "password reset" to authentication service

1. USER: Gives follow-up prompt with task
2. AGENT: Executes RAGESe:
   - Reads Memory Bank, learns auth structure
   - Checks Constitution (interfaces first, tests required)
   - Examines existing UserRepository
   - Creates PasswordResetService + interface
   - Writes unit tests
   - Updates activeContext.md & progress.md
3. AGENT: Passes Context Integrity Gateway
4. AGENT: Delivers code + documentation updates

🎖️ Best Practices

    Start small - Begin with a well-defined feature

    Customize early - Adjust Constitution before heavy use

    Trust anomalies - Gateway flags real contradictions

    Review logs - Check progress.md regularly

    Be specific - Clear tasks yield better results

🔧 Adaptation Guide
For Non-Python Projects

Modify AGENTS-Constitution.md:

    Sections 1 (Dev Environment)

    Sections 6-7 (Python-specific rules)

    Update tech stack in techContext.md

For Different Architectures

    Update layer definitions in Constitution Section 2

    Modify systemPatterns.md accordingly

    Maintain the dependency rule consistency

Adding Custom Rules

    Add new articles to Constitution

    Reference them in Memory Bank protocol

    Update Context Integrity Gateway matrix

❓ FAQ
Q: Do I need long prompts every time?

A: No. After boot, use: "As per protocol, implement [feature]. Ensure Constitution compliance and update Memory Bank."
Q: Which AI models work best?

A: Models with large context windows (Claude 3.5 Sonnet, GPT-4, etc.) that can read all files simultaneously.
Q: What if my project doesn't use Clean Architecture?

A: Modify AGENTS-Constitution.md Section 2 to match your actual architecture. The system enforces consistency, not a specific pattern.
Q: How to handle large projects?

A: The system scales naturally: progress.md summarizes, systemPatterns.md references sub-documents. Maintain hierarchical relationships.
🤝 Contributing

We welcome:

    Constitution templates for other languages (Go, Rust, TypeScript, etc.)

    Integration scripts (auto-initialize from existing projects)

    Case studies & examples

See CONTRIBUTING.md for guidelines.
📜 License

MIT License - see LICENSE file for details.