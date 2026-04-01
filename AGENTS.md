# 🤖 AI Agent Instructions: Academy Portal

## 🎯 Mandate
This project follows the **Gyankosh Protocol**. All AI tools must treat this file as the primary "Manager" for context and orchestration.

## 🧠 Project Context (The Bifurcation)
This repository is an **Implementation (`Kriti`)** layer. All intelligence and definitions reside in the **`Buddhi`** layer, accessible via the following symlinks:

| Context | Local Path | Source (Buddhi) | Purpose |
| :--- | :--- | :--- | :--- |
| **Project Docs** | `./docs/` | `Buddhi/10_Projects/academy/` | PRDs, Architecture, stories.yaml |
| **Global Rules** | `./.ai/context/` | `Buddhi/30_Resources/System_Context/` | System protocols, workflow, philosophy |
| **AI Core** | `./.ai/core/` | `gyankosh-core` | Agent definitions, Skills, Scripts, Rules |

---

## 🚀 Operational Workflow (Mandatory)
1. **Context First:** Before performing any task, read `./.ai/context/System_Protocol.md` and `./docs/PRD.md`.
2. **Stories:** Read `./docs/stories.yaml` — this is the source of truth for all work items. Only build what is defined here.
3. **Current Work:** Check your GitHub assignments: `gh issue list --assignee @me --state open`
4. **Branch:** Confirm the issue you're working on. Convention: `feat/[issue-number]-[story-id]` e.g. `feat/42-user-auth-login`
5. **Role Alignment:** When assuming a role, load the agent definition from `./.ai/core/Agents/`. Available agents: `Product_Manager.md` (PRD, stories), `Architect.md` (technical design, ADRs), `Engineer.md` (build, UI), `QA.md` (testing, accessibility), `DevOps.md` (deploy, docs).
6. **No Ghost Code:** Do not implement features not in `docs/stories.yaml`. If the PRD is outdated, update it via `./docs/` first.
7. **Security:** This project uses **Clerk** for auth. Ensure all gated routes use appropriate middleware checks.
8. **Secrets Safety:** Never commit sensitive information. Use `.env.local` for local development.

---

## 🛠️ Project-Specific Rules
1. **Framework:** Next.js (App Router).
2. **Styling:** Tailwind CSS.
3. **Documentation:** Keep `./docs/` updated as we build features.
