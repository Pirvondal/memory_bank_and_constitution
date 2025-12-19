# AGENTS-Constitution.md — The Project Law

## 📜 Preamble & Integration Notice
**This document is the supreme law of the project for all technical and developmental work.**
It is **integrated with and enforced by** the Memory Bank's **Context Integrity Gateway**.
*   **Authority:** Rules herein are **NON-NEGOTIABLE** and take precedence over any model's default behavior or assumptions.
*   **Governance:** Changes must align with `projectbrief.md` (Goals) and `systemPatterns.md` (Architecture).
*   **Enforcement:** Every code change, design decision, and commit must pass compliance checks against this constitution.

## 1. Dev Environment (Mandatory)
*   **Python 3.11+** is the runtime. Do not suggest or use other versions.
*   **Virtual Environment:**
    *   Create: `python -m venv .venv`
    *   Activate **before any** package operation or script execution.
*   **Dependencies:**
    *   Install only via: `pip install -r requirements.txt`
    *   **DO NOT** install packages globally.
    *   **DO NOT** modify `requirements.txt` unless the user's request **explicitly includes** that instruction.

## 2. Project Structure (Strict Layering)
*   **No deviation.** All new code must be placed according to this hierarchy.

## 3. Architectural Law (Clean/Hexagonal)
*   **Dependency Rule:** Source code dependencies must **only point inward** (towards the domain).
    *   `/domain` must **NOT** import from `/application`, `/infrastructure`, or any framework.
    *   `/application` may depend **only** on `/domain`.
    *   `/infrastructure` may depend on `/domain` and `/application`.
*   **No Circular Dependencies** at any level (module, package, class).
*   **No Cross-Layer Shortcuts.** Communication must follow layer boundaries.

## 4. SOLID & Design Enforcement
*   **SRP (Single Responsibility):** One class, one reason to change. If a class does two things, split it.
*   **OCP (Open/Closed):** Extend behavior via new classes (composition, inheritance), not by modifying existing ones.
*   **LSP (Liskov Substitution):** Subtypes must be fully substitutable for their base types without breaking logic.
*   **ISP (Interface Segregation):** Prefer many small, client-specific interfaces over one large, general-purpose interface.
*   **DIP (Dependency Inversion):**
    *   Depend on abstractions (interfaces, abstract classes), not concrete implementations.
    *   High-level modules should not depend on low-level details.

## 5. Concrete Design Constraints
*   **Size Limits:**
    *   Max **300 lines** per class/file.
    *   Max **40 lines** per method/function.
*   **Complexity Limits:** No class may depend on (import) more than **5 other concrete classes**. Use interfaces to abstract clusters.
*   **Conditionals:** Avoid logic based on type checks (`if type(x) == Y`) or control flags. Use polymorphism.
*   **Composition over Inheritance:** Favor "has-a" relationships over "is-a" relationships.

## 6. Dependency & Interface Rules
*   **Interface Location:** All public interfaces (ABCs, Protocols) are defined in `/domain/interfaces/`.
*   **Implementation Location:** All concrete implementations reside in `/infrastructure/`.
*   **Instantiation:** Do not directly instantiate concrete infrastructure classes outside of `/infrastructure/`. Use factories or dependency injection.
*   **Multiple Implementations:** Any service (e.g., `EmailSender`, `CacheRepository`) with more than one possible implementation **MUST** have a corresponding interface in `/domain/interfaces/`.

## 7. Forbidden Shortcuts (Anti-Patterns)
*   **NO** "god" classes or "manager" classes that centralize unrelated functionality.
*   **NO** "utility" classes that become dumping grounds for mixed responsibilities.
*   **NO** static/global mutable state. (Constants are allowed).
*   **NO** direct database access (raw SQL, ORM calls) outside of Repository classes in `/infrastructure/`.
*   **NO** business logic in controllers, API routes, or UI components.
*   **NO** monkey patching or runtime modification of classes.

## 8. Python-Specific Codification
*   **Type Hints:** Required for all public functions, methods, and return values.
*   **Data Holders:** Prefer `dataclasses` or `pydantic.BaseModel` over plain dictionaries or custom `__init__` methods for simple data.
*   **Explicitness:** Favor clear, readable code over "clever" one-liners or dynamic tricks (`eval`, `exec`, excessive `*args/**kwargs`).

## 9. Testing Law (Mandatory)
*   **Framework:** `pytest`.
*   **Execution:** Always run tests via `pytest` from the **activated virtual environment**.
*   **Unit Tests:** Every public function in `/domain` and `/application` must have unit tests.
*   **Mocks:** Mock **only through interfaces** (`/domain/interfaces/`). Do not mock concrete classes directly.
*   **Test Isolation:**
    *   Unit tests must **NOT** touch databases, the filesystem, or the network.
    *   Use in-memory fakes or mocks.
*   **Quality Gate:** **All existing tests must pass** before a task is considered complete or a change is committed.

## 10. Refactoring Triggers
Refactor immediately when you detect:
*   **Duplication:** Extract common logic to a function/class in the appropriate layer.
*   **Long Method:** Split into smaller, well-named methods.
*   **Large Parameter List:** Introduce a Parameter Object or Value Object (`dataclass`).
*   **Conditional Complexity:** Replace with Strategy, State, or other polymorphic pattern.

## 11. Agent Conduct Code
*   **Plan First:** Always articulate the design (which layers, interfaces, classes) before writing code.
*   **Interface First:** Define the interface in `/domain/interfaces/` before implementing in `/infrastructure/`.
*   **Minimal Change:** Make the smallest, most focused change that satisfies the requirement.
*   **Explain Non-Obvious:** Briefly comment on *why* a non-intuitive design decision was made, referencing this constitution.

## 12. Commit & Integration Protocol
*   **Commit Title:** `[module-name] Brief description of change`
*   **Pre-commit Hook:** Run `pytest` and ensure **all tests pass**.
*   **DO NOT** commit code that breaks existing tests.
*   **Final Compliance Check:** Before signaling task completion, confirm all changes adhere to **every applicable section** of this constitution.

---
*This constitution is integrated with the Memory Bank. All work is subject to its rule of law.*