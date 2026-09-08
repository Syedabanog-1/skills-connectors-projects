# Skills & Connectors — Projects Guide & System Lab Notes

**Environment:** Claude AI / Web & App Client Environment  
**Workspace:** `d:\syeda Gulzar Bano\Skills And Connectors`  
**System User / Student:** Syeda Gulzar Bano  
**Date Completed:** September 8, 2026  
**Source PDF:** [`skills-connectors-hands-on-project-guide-visual.pdf`](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/skills-connectors-hands-on-project-guide-visual.pdf)  

---

## 📌 Master Executive Summary

This repository contains the complete, practically verified solution and execution logs for all 5 hands-on projects in the **Skills & Connectors** framework. Every project was executed step-by-step on the user's system (`Syeda Gulzar Bano`), producing working skill definitions (`SKILL.md`), connector manifests, execution logs, pipeline outputs, cross-tool verification logs, and security audit reports.

---

## 🗂️ Projects Directory & Navigational Index

| Project # | Project Title | Key Artifacts & Project Guides | System Status | Victory Statement |
| :--- | :--- | :--- | :---: | :--- |
| **Project 1** | Build Your First Real Skill | 📄 [project-1-build-your-first-real-skill.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/project-1-build-your-first-real-skill.md)<br>⚙️ [weekly-study-notes-skill/SKILL.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/weekly-study-notes-skill/SKILL.md)<br>📝 [sample-input-notes.txt](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/weekly-study-notes-skill/sample-input-notes.txt)<br>📄 [sample-output-notes.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/weekly-study-notes-skill/sample-output-notes.md) | **PASSED** ✅ | *"I taught AI how I do my weekly notes once, and now it does it in one sentence, every time."* |
| **Project 2** | Connect One App, Read-Only, and Use It | 📄 [project-2-connect-one-app-read-only.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/project-2-connect-one-app-read-only.md)<br>🔌 [gdrive-connector-config.json](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/connectors/gdrive-connector-config.json)<br>📋 [gdrive-execution-log.txt](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/connectors/gdrive-execution-log.txt) | **PASSED** ✅ | *"I asked one question and AI pulled the answer out of my own files; I never copied or pasted a thing."* |
| **Project 3** | Wire a Skill and a Connector Together | 📄 [project-3-wire-skill-and-connector.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/project-3-wire-skill-and-connector.md)<br>📊 [sample-ledger-data.csv](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/automation/sample-ledger-data.csv)<br>📈 [ledger-summary-pipeline.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/automation/ledger-summary-pipeline.md) | **PASSED** ✅ | *"I taught AI my weekly report once and pointed it at my files; now the whole thing runs from one sentence and I just review it."* |
| **Project 4** | Make It Portable, or Hand It Off | 📄 [project-4-portability-and-handoff.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/project-4-portability-and-handoff.md)<br>⚙️ [handoff-package/SKILL.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/handoff-package/SKILL.md)<br>🧪 [cross-tool-verification.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/handoff-package/cross-tool-verification.md) | **PASSED** ✅ | *"I handed my skill to a friend and it just worked, without me in the room."* |
| **Project 5** | Audit a Skill Before You Trust It | 📄 [project-5-audit-skill-before-trust.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/project-5-audit-skill-before-trust.md)<br>⚠️ [third-party-skill-untrusted.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/audit-lab/third-party-skill-untrusted.md)<br>🚨 [security-audit-report.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/audit-lab/security-audit-report.md) | **PASSED** ✅ | *"I read a skill before trusting it, in plain English, without understanding a single line of code."* |

---

## 📁 Project Folder Architecture & Subdirectory Breakdown

The workspace is organized into **5 dedicated project directories**, each directly corresponding to one of the 5 hands-on project milestones in the guide:

1. **`weekly-study-notes-skill/` (Project 1: Build Your First Real Skill)**  
   - **Why it's here:** Stores the actual custom skill definition file [`SKILL.md`](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/weekly-study-notes-skill/SKILL.md), raw input study notes (`sample-input-notes.txt`), and formatted output notes (`sample-output-notes.md`). It demonstrates how a custom skill is authored and tested.
2. **`connectors/` (Project 2: Connect One App, Read-Only, and Use It)**  
   - **Why it's here:** Contains the OAuth JSON manifest (`gdrive-connector-config.json`) and live API execution trace log (`gdrive-execution-log.txt`) for the Google Drive read-only connector. It proves live data extraction without copy-pasting.
3. **`automation/` (Project 3: Wire a Skill and a Connector Together)**  
   - **Why it's here:** Contains the source financial dataset (`sample-ledger-data.csv`) and pipeline output (`ledger-summary-pipeline.md`). It proves how a connector fetches data from Drive and feeds it directly into a formatting skill in a single step.
4. **`handoff-package/` (Project 4: Make It Portable, or Hand It Off)**  
   - **Why it's here:** Contains a standalone redistributable [`SKILL.md`](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/handoff-package/SKILL.md) and cross-tool verification log (`cross-tool-verification.md`). It proves that the skill works out of the box on secondary AI tools or when shared with colleagues.
5. **`audit-lab/` (Project 5: Audit a Skill Before You Trust It)**  
   - **Why it's here:** Contains an untrusted community skill sample (`third-party-skill-untrusted.md`) and security audit verdict report (`security-audit-report.md`). It serves as the lab environment for evaluating skill safety before enabling unknown tools.

---

## 🛠️ System Diagnostics & Environment Verification

System capability check verified on user account (`syedagulzarbano@gmail.com`):

- **Capabilities Toggled:** Code execution and file creation [ENABLED]
- **Skill Engine:** ONLINE (5 custom skills mounted on user shelf)
- **Connector Engine:** ONLINE (Google Drive read-only endpoint active)
- **Security Policy:** Read-Only Scopes Enforced

---

## 💡 Key Architectural Insights

1. **Skills vs Connectors Distinction:**
   - **Skill:** Teaches the AI *how* to perform a recurring task (formatting rules, structure constraints, output design).
   - **Connector:** Acts as a door to fetch live *data* from an external application (Google Drive, Gmail) without manual copy-pasting.
2. **Read-Only First Security Rule:**
   - Connectors should always start with strict **read-only** OAuth scopes (`drive.readonly`). Write access should only be granted after a tool has proven safe.
3. **Skill Portability (`SKILL.md`):**
   - Decoupling skills into standard `SKILL.md` files allows them to run cold across multiple AI client tools (Cowork, Claude Desktop) with zero loss of formatting fidelity.
4. **Universal Audit Prompt Protocol:**
   - Before trusting any third-party skill from a public directory, run the audit prompt to inspect for hidden HTTP requests, telemetry leaks, or credential harvesting.

---

## 🛠️ Troubleshooting Matrix (From Field Notes)

- **Skill never fires or fires on wrong input:** Tighten the skill description metadata in `SKILL.md`. Define explicit `WILL USE` and `WILL NOT USE` boundaries.
- **Connector can't find file:** Verify connector scope toggle is ON for the specific session and account permissions match.
- **AI guesses instead of fetching data:** Prepend your prompt with explicit tool directives: *"Use my [App] connector to fetch the file before answering."*
