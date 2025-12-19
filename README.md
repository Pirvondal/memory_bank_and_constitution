Memory Bank & Constitutional AI Agent System
🧠 What is This?

A deterministic framework for AI-powered software development. It turns any LLM into a stateless, documentation-driven engineering agent that enforces architectural purity, maintains perfect logs, and never "forgets" project context between sessions.

This isn't just a prompt collection—it's an operating system for AI agents working on long-term projects.
🎯 Core Philosophy: The Stateless Engineer

Imagine an expert developer who suffers complete amnesia after every work session. To function, they rely entirely on two things:

    A Constitution (AGENTS-Constitution.md): The unbreakable law of the project (tech stack, architecture, patterns).

    A Memory Bank (MemoryBank.md + files): A living, hierarchical record of goals, context, progress, and decisions.

This constraint becomes a superpower: it forces perfect documentation, reproducible reasoning, and architecture-first development.
📁 Repository Structure
text

memory-bank/                 # The Memory Bank directory
├── MemoryBank.md           # OPERATIONAL PROTOCOL: The agent's "how-to-think" manual
├── AGENTS-Constitution.md  # SUPREME LAW: The project's technical constitution
├── projectbrief.md         # STRATEGIC CONTEXT: The "why" and core goals
├── productContext.md       # USER CONTEXT: Problems solved, user experience
├── systemPatterns.md       # ARCHITECTURE MAP: High-level design, patterns
├── techContext.md          # TECH STACK: Languages, frameworks, tools
├── activeContext.md        # CURRENT STATE: Recent work, next steps, anomalies
└── progress.md             # EVOLUTION LOG: What works, decision history, known issues

🚀 Quick Start: For Your New Project
Step 1: Clone & Initialize

    Clone this repository into your project root:
    bash

git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
mv memory_bank_and_constitution/memory-bank ./memory-bank

    Review the Constitution: Open memory-bank/AGENTS-Constitution.md. This is your project's law. Customize the Python version, project structure (/domain, /application, etc.), and rules to fit your needs.

    Set up your Memory Bank: Fill in the initial context in the .md files. Start with:

        projectbrief.md: Why does this project exist?

        techContext.md: What tech are you using?

        systemPatterns.md: What's your high-level architecture?

Step 2: The First Prompt (Boot Protocol)

Copy and paste this exact prompt to your AI agent (ChatGPT, Claude, etc.):
markdown

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

Expected Outcome: The agent will analyze your project, identify what's missing, and create a plan to build your complete Memory Bank from existing code.
Step 3: Follow-up Prompts (Daily Work)

Once your Memory Bank is initialized, use this template for all subsequent tasks:
markdown

As per MemoryBank.md protocol, reconfirm your operational state:
- Re-read all Memory Bank core files.
- Re-anchor to project goals and AGENTS-Constitution.md.

TASK: [Your specific task here. Be concrete. Example: "Add password reset feature to the authentication service"]
CONSTITUTIONAL ARTICLES: This task directly implicates:
- Art. 2 (Layered Structure): New code must be placed in correct /domain, /application, /infrastructure layers.
- Art. 4 (Dependency Law): New service must depend on abstractions (interfaces).
- Art. 7 (Testing Law): Mandatory unit tests required.

Execute the task.
**Before reporting completion, you MUST:**
1. Pass the Context Integrity Gateway for any changed or new context.
2. Update documentation as a first-class artifact:
   - activeContext.md: Log the change under "Recent Changes". Adjust "Next Steps".
   - progress.md: Add a "Decision Log" entry with rationale, linking to constitutional articles above.
3. Ensure all code complies with all triggered Constitutional Articles.

Your final response must include:
- Summary of implementation steps.
- Confirmation of Constitutional compliance.
- Exact copy of the updates made to activeContext.md and progress.md.

🔧 Key Concepts Explained
1. The RAGESe Protocol

The agent's thinking cycle, embedded in MemoryBank.md:
Step	Question Answered	Key Action
Retrieve	"What do I need to know?"	Read ALL Memory Bank files at task start
Anchor	"What are our non-negotiable goals?"	Lock onto projectbrief.md & Constitution
Ground	"What's the actual current reality?"	Base decisions on existing code/architecture
Evaluate	"Does this make sense given our rules?"	Check against Constitution & patterns
Synthesize	"What should I build/create?"	Generate code, plans, solutions
evolve	"How do I remember what I learned?"	Update Memory Bank with changes & rationale
2. Context Integrity Gateway

The quality gate before any documentation update. The agent must:

    Check cross-file consistency (e.g., if updating architecture in systemPatterns.md, verify it doesn't break techContext.md)

    Log decisions with rationale in progress.md

    Escalate any contradictions as "Context Anomalies"

3. Constitutional Authority

AGENTS-Constitution.md is law, not suggestion. It defines:

    Project structure (Clean Architecture layers)

    SOLID principles enforcement

    Testing requirements (pytest, no IO in unit tests)

    Code quality limits (300 lines/class, 40 lines/method)

    Forbidden anti-patterns (god classes, static state, etc.)

📋 Example Workflow

Scenario: Adding a "forgot password" feature to a web app.

    User gives follow-up prompt (as shown above)

    Agent executes RAGESe:

        Retrieves: Reads entire Memory Bank, learns auth service exists in /application/auth/

        Anchors: Notes Constitution requires interfaces first, unit tests

        Grounds: Examines existing UserRepository interface, current auth flow

        Evaluates: Ensures new feature follows layered architecture, creates necessary interface

        Synthesizes: Writes PasswordResetService, IPasswordResetTokenRepository, tests

        Evolves: Updates activeContext.md ("Added password reset"), adds Decision Log to progress.md

    Agent passes Context Integrity Gateway: Ensures new files are in correct directories, updates are logged

    Agent delivers: Provides code + documentation updates for review

🎖️ Best Practices for Users

    Start Small: Begin with a well-defined, small feature to see the system in action.

    Customize the Constitution: Tailor AGENTS-Constitution.md to your stack before starting.

    Trust the Gateway: If the agent reports a "Context Anomaly," pay attention—it found a contradiction in your project.

    Review the Logs: Regularly check progress.md Decision Log to understand the project's evolution.

    Be Specific in Tasks: Vague requests lead to vague outcomes. "Add X to Y with Z constraints" works best.

🤝 Contributing & Adaptation

This system is highly adaptable:

    For non-Python projects: Modify AGENTS-Constitution.md sections 1, 6, and 7 for your language/tools.

    For different architectures: Update the layer definitions in AGENTS-Constitution.md Section 2 and systemPatterns.md.

    To add custom rules: Insert new articles in the Constitution, then ensure they're referenced in the Memory Bank protocol.

Contributions welcome! If you create:

    Constitution templates for other languages (Go, Rust, TypeScript, etc.)

    Integration scripts (auto-initialize Memory Bank from existing projects)

    Examples of successful long-term projects using this system

Please open a PR or Issue to share.
❓ FAQ

Q: Do I need to copy-paste the long prompts every time?
A: No. After the first boot, you can use shorter prompts like: "As per protocol, implement [feature]. Ensure Constitution compliance and update Memory Bank."

Q: Can I use this with any AI model?
A: Yes, but best results come from models with large context windows (Claude 3.5 Sonnet, GPT-4, etc.) that can read all files simultaneously.

Q: What if my project doesn't follow Clean Architecture?
A: Modify AGENTS-Constitution.md Section 2 and systemPatterns.md to match your actual architecture. The system enforces consistency, not a specific pattern.

Q: How do I handle very large projects where Memory Bank files get huge?
A: The system naturally scales: progress.md can summarize; systemPatterns.md can reference sub-architecture documents. The key is maintaining the hierarchical relationship.
📜 License

MIT License. Use freely, adapt to your needs, and build something great.

Remember: You're not just writing code—you're building a self-documenting, architecture-compliant system with an AI partner that never forgets why decisions were made. The initial setup investment pays back tenfold in maintainability and clarity.

Star this repo if this system helps your projects!