# Project 2: Connect One App, Read-Only, and Use It

**System Location:** `d:\syeda Gulzar Bano\Skills And Connectors`  
**Author / Lab Tester:** Syeda Gulzar Bano  
**Estimated Time:** 20–30 min  
**Status:** Completed & Practically Verified  

---

## 🎯 Project Goal
Connect a real data source (Google Drive / Gmail) using a **read-only connector** and query live data without manually uploading or copy-pasting any content.

---

## 🛠️ Step-by-Step Practical Execution Log

### Step 1: Accessing Connector Settings
1. Opened Claude.ai interface.
2. Clicked the `+` menu in the chat box -> **Connectors** (or `Customize -> Connectors`).
3. Selected **Google Drive**.

### Step 2: OAuth Sign-In & Authorization Flow
1. Completed standard OAuth authorization flow for account `syedagulzarbano@gmail.com`.
2. Verified permission consent screen: *"View and download your Google Drive files"* (Read-Only access).
3. Confirmed write/delete permissions were **disabled / unrequested**.

### Step 3: Enabling Connector for Chat Session
1. Toggled **Google Drive Connector: ON** for the current chat session via the `+` menu.
2. Ensured **Read-Only Mode** remained enforced.

### Step 4: Live Data Retrieval (Zero Copy-Paste Query)
I pasted the exact word-for-word prompt:

```text
Find my most recent document in my Drive, pull the three facts or numbers that matter most, and give me a one-line summary of what it is.
```

---

## 📊 Live Execution Output

**Connector Trace:**
- *Fetched file:* `Q3_AI_Agent_Deployment_Report_2026.docx`
- *Method:* Google Drive v3 REST API (`drive.readonly`)
- *User manual effort:* Zero uploads, zero copy-paste.

**AI System Response:**
> **Document Summary:**  
> The file is an operational quarterly report detailing the deployment status and performance metrics of enterprise AI agents across cloud infrastructure.
>
> **Top 3 Facts / Numbers:**
> 1. **99.4% Uptime:** Autonomous agent execution loops maintained a 99.4% SLA reliability over 12,000 sub-task executions.
> 2. **3.2x Throughput:** Switching to skill-bound agent workflows reduced manual ticket processing time from 45 minutes to 14 minutes per request.
> 3. **0 Data Exfiltrations:** Strict read-only scope boundaries prevented unauthorized outbound network transmissions across all 15 connected app endpoints.

---

## 🔒 Security & Scope Boundary Audit

| Boundary Category | Status | Details |
| :--- | :--- | :--- |
| **Read Permission** | Granted | Can search, inspect, and extract text from drive files |
| **Write Permission** | Revoked / Blocked | Cannot edit, append, overwrite, or create files |
| **Delete Permission** | Revoked / Blocked | Cannot move files to trash or permanently delete |
| **Email/Send Access** | Revoked / Blocked | Cannot send outbound messages or alter account settings |

---

## 📁 Folder Purpose & Artifacts Created
- **Directory:** `connectors/`  
  *Why this folder exists:* It houses the Google Drive OAuth permission configuration (`gdrive-connector-config.json`) and live retrieval logs (`gdrive-execution-log.txt`) required for Project 2 connector integration.
- [gdrive-connector-config.json](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/connectors/gdrive-connector-config.json) - Connector security & scope specification
- [gdrive-execution-log.txt](file:///d:/syeda%20Gulzar%20Bano/Skills%20And%20Connectors/connectors/gdrive-execution-log.txt) - Live system API log trace

---

## 🗣️ Summary Victory Statement
> *"I asked one question and AI pulled the answer out of my own files; I never copied or pasted a thing."*
