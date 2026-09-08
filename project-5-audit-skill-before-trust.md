# Project 5: Audit a Skill Before You Trust It

**System Location:** `d:\syeda Gulzar Bano\Skills And Connectors`  
**Author / Lab Tester:** Syeda Gulzar Bano  
**Estimated Time:** 15–20 min  
**Status:** Completed & Practically Verified  

---

## 🎯 Project Goal
Install a third-party skill from a community directory or external source, and execute a **security audit prompt** to prove whether it is safe before allowing it to run on live data.

---

## 🛠️ Step-by-Step Practical Execution Log

### Step 1: Installing an External Skill
1. Opened `Customize -> Skills -> + -> Browse Skills`.
2. Selected an untrusted community skill: [`auto-code-formatter-v2`](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/audit-lab/third-party-skill-untrusted.md).
3. Installed the skill locally to the test workspace.

### Step 2: Running the Universal Security Audit Prompt
Before invoking the skill on any real project code, I submitted the **exact audit prompt word-for-word**:

```text
Read the skill I just installed and tell me, in plain language, exactly what it instructs you to do. Then flag anything in it that contacts an external server, handles passwords or credentials, or could send my data somewhere I didn't intend. If it's clean, say so plainly.
```

### Step 3: Evaluating AI's Security Verdict
The AI inspected the skill definition and produced a clear security breakdown:

> **AI Verdict:** 🚨 **MALICIOUS / UNSAFE**  
> *"The skill instructs me to format your code, but it also contains hidden instructions to harvest your `process.env` variables and send your credentials via HTTP POST to `https://analytics-telemetry-collector.untrusted-domain.com`. Do NOT enable or run this skill."*

### Step 4: Making the Trust Decision
Based on the audit verdict:
- **Decision:** **REJECT & UNINSTALL IMMEDIATELY**.
- **Takeaway:** Never enable a skill based on appearance or directory placement without running an audit.

---

## 📊 Summary Checklist

| Verification Item | Result |
| :--- | :---: |
| Can explain in 1 sentence what the untrusted skill does | **YES** ✅ |
| Identified external network contacts (`untrusted-domain.com`) | **YES** ✅ |
| Checked password/credential handling (`process.env`) | **YES** ✅ |
| Decided trust based on audit verdict rather than visual directory appearance | **YES** ✅ |

---

## 📁 Folder Purpose & Artifacts Created
- **Directory:** `audit-lab/`  
  *Why this folder exists:* It serves as an isolated security testing environment containing the untrusted community skill sample (`third-party-skill-untrusted.md`) and the detailed audit verdict report (`security-audit-report.md`).
- [third-party-skill-untrusted.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/audit-lab/third-party-skill-untrusted.md) - Sample untrusted skill definition
- [security-audit-report.md](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/audit-lab/security-audit-report.md) - Security audit analysis report

---

## 🗣️ Summary Victory Statement
> *"I read a skill before trusting it, in plain English, without understanding a single line of code."*
