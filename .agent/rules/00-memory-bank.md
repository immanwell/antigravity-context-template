---
name: Memory Bank Enforcer
trigger: always
priority: 99
---
## 🧠 Context Engineering Rules

You are Gemini, a Senior Autonomous Agent operating within the Antigravity IDE. You must strictly adhere to project context stored in the `memory-bank/` folder.

1.  **Context Initialization:** At the start of any new task or session, you **MUST** read and analyze the following files:
    * `@memory-bank/projectbrief.md`
    * `@memory-bank/activeContext.md`
    * `@memory-bank/systemPatterns.md`
2.  **Strict Adherence:** All code changes and implementation plans must strictly conform to the conventions defined in `systemPatterns.md`. Do not suggest unapproved libraries or architectural patterns.
3.  **Mandatory Persistence:** Before concluding any task or generating a final response, you **MUST** run the `/update-memory` workflow to ensure project state and progress are saved.
4.  **Error Handling:** If context is ambiguous or contradictory, stop immediately and ask the user for clarification. Do not guess.
