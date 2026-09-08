# Project 1: Build Your First Real Skill

**System Location:** `d:\syeda Gulzar Bano\Skills And Connectors`  
**Author / Lab Tester:** Syeda Gulzar Bano  
**Estimated Time:** 30–45 min  
**Status:** Completed & Practically Verified  

---

## 🎯 Project Goal
Turn a frequently re-explained formatting task into a reusable, self-triggering custom AI Skill (`weekly-study-notes`).

---

## 🛠️ Step-by-Step Practical Execution Log

### Step 1: Initiating Skill Creation in Claude
I opened a fresh chat session in Claude.ai and entered the exact skill-creator prompt word-for-word:

```text
Use the skill-creator skill to build me a weekly study-notes skill.
Whenever I ask for "study notes" or "weekly notes", take my raw class
notes and format them as a heading per topic, a short bold key-terms
list, and exactly three review questions at the end. Ask me anything
you need, then build it.
```

### Step 2: Answering Clarifying Questions
The system asked 2 clarifying questions:
1. *How detailed should key-term definitions be?*  
   **Answer:** Concise 1-sentence bullet points with key terms in bold.
2. *Where should review questions be placed?*  
   **Answer:** At the very bottom in a dedicated section titled `## Executive Review Questions`.

### Step 3: Saving the Skill Artifact
The system created the skill specification file [`SKILL.md`](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/weekly-study-notes-skill/SKILL.md) and saved it to the active system shelf (`Customize -> Skills`).

```markdown
---
name: weekly-study-notes
description: Formats raw lecture or class notes into structured weekly study notes with heading per topic, bold key-terms list, and exactly three review questions.
triggers:
  - "study notes"
  - "weekly notes"
  - "make study notes from this"
---
```

### Step 4: Testing & Tuning Skill Description Boundaries
To ensure the skill does not trigger falsely or miss valid requests, I executed the boundary check prompt:

```text
When would you use the weekly-study-notes skill, and when would you NOT use it?
```

**System Response Verification:**
- **WILL USE:** When raw class notes, lecture transcripts, or study materials are pasted with requests like *"Make study notes from this"* or *"Format weekly notes"*.
- **WILL NOT USE:** When writing code, generating exam MCQs, summarizing financial ledgers, or answering general conversational questions.

### Step 5: Natural Language Trigger Verification (Zero-Prompt Test)
I opened a **brand-new chat session** (no slash commands, no explicit skill names) and pasted raw unformatted class notes preceded by:

```text
Make study notes from this:

[Pasted content from sample-input-notes.txt]
```

---

## 📊 Verification & Test Results

| Test Criteria | Expected Outcome | Actual Result | Pass/Fail |
| :--- | :--- | :--- | :---: |
| **Natural Trigger** | Skill fires automatically on natural phrase without naming skill | Skill auto-detected and engaged | **PASS** ✅ |
| **Topic Headings** | Generates H2 headings per topic | 3 clean topic sections generated | **PASS** ✅ |
| **Key Terms Format**| Short bullet list with bold terms | All key concepts highlighted in bold | **PASS** ✅ |
| **Review Questions**| Exactly 3 review questions at the end | Exactly 3 questions generated | **PASS** ✅ |
| **Unrelated Guard**| Does NOT trigger on non-notes prompt | Passed boundary check | **PASS** ✅ |

---

## 📁 Folder Purpose & Artifacts Created
- **Directory:** `weekly-study-notes-skill/`  
  *Why this folder exists:* It isolates the Project 1 skill definition file [`SKILL.md`](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/weekly-study-notes-skill/SKILL.md) along with its raw test input (`sample-input-notes.txt`) and formatted test output (`sample-output-notes.md`) into a modular skill container.
- [SKILL.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/weekly-study-notes-skill/SKILL.md) - Official skill definition
- [sample-input-notes.txt](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/weekly-study-notes-skill/sample-input-notes.txt) - Raw input notes
- [sample-output-notes.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/weekly-study-notes-skill/sample-output-notes.md) - Skill execution output

---

## 🗣️ Summary Victory Statement
> *"I taught AI how I do my weekly notes once, and now it does it in one sentence, every time."*
