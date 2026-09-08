# Project 3: Wire a Skill and a Connector Together

**System Location:** `d:\syeda Gulzar Bano\Skills And Connectors`  
**Author / Lab Tester:** Syeda Gulzar Bano  
**Estimated Time:** 45–60 min  
**Prerequisites:** Projects 1 and 2 completed  
**Status:** Completed & Practically Verified  

---

## 🎯 Project Goal
Create an automated **monthly-close / weekly-batch machine** by orchestrating a **live connector** (Google Drive) and a **custom skill** (`weekly-study-notes` / formatting skill) simultaneously using a **single plain-English sentence**.

---

## 🛠️ Step-by-Step Practical Execution Log

### Step 1: Pre-Flight Verification
1. Verified `weekly-study-notes` skill is enabled on the system shelf.
2. Verified Google Drive Read-Only connector is active for the current chat session.
3. Placed target raw file [`sample-ledger-data.csv`](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/automation/sample-ledger-data.csv) in Drive under the file name `DEMO-ledger-March`.

### Step 2: Sending the Single-Sentence Batch Command
I submitted the exact word-for-word prompt:

```text
Prepare this month's summary for DEMO Trading; the ledger is the file called DEMO-ledger-March in my Drive.
```

### Step 3: Observing System Orchestration
1. **Connector Activation:** Claude autonomously identified the file request, invoked `gdrive.readonly` API, located `DEMO-ledger-March.csv`, and read its text rows.
2. **Skill Activation:** Without additional prompting, Claude fed the raw CSV content directly into the formatting skill, generating categorized spending breakdowns and bold key terms.

---

## 📊 Verification & Hand Spot-Check

To ensure full accuracy before trusting automated batch outputs, I performed a manual spot-check:

```text
Manual Verification Math:
AWS ($1250) + Claude ($480) + Marketing ($2100) + Audit ($3500) + Pinecone ($650) + Hardware ($1850) + GitHub ($920)
= $10,750.00 USD.
```

- **Automated Output Result:** `$10,750.00 USD` (Exact match! 🎯)
- **Formatting Compliance:** Structured H2 headings, bold key terms, exactly 3 review questions.

---

## 📁 Folder Purpose & Artifacts Created
- **Directory:** `automation/`  
  *Why this folder exists:* It contains the raw dataset (`sample-ledger-data.csv`) and output report (`ledger-summary-pipeline.md`) demonstrating single-sentence automated pipeline execution that wires a connector and a skill together.
- [sample-ledger-data.csv](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/automation/sample-ledger-data.csv) - Raw source dataset placed in Drive
- [ledger-summary-pipeline.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/automation/ledger-summary-pipeline.md) - Pipeline output generated from dual engine execution

---

## 🗣️ Summary Victory Statement
> *"I taught AI my weekly report once and pointed it at my files; now the whole thing runs from one sentence and I just review it."*
