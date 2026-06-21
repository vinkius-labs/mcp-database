# Abridge (AI Clinical Documentation API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/abridge-ai-clinical-documentation-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Automate clinical documentation with Abridge — create recordings, track processing status, and retrieve structured medical notes directly via AI.

## Description
Integrate **Abridge** into your clinical workflow to convert patient-provider conversations into high-quality medical documentation. This MCP server allows AI agents to manage the entire lifecycle of clinical note generation.

### What you can do

- **Recording Management** — Start new sessions or upload audio files for processing with patient and provider context using the `create_recording` tool.
- **Status Tracking** — Monitor the AI processing pipeline with `get_recording_status` to know exactly when notes are ready.
- **Structured Clinical Notes** — Retrieve comprehensive documentation including HPI (History of Present Illness), Physical Exam, and Assessment & Plan sections via `get_clinical_notes`.

### How it works

1. Subscribe to this server
2. Enter your Abridge API Key
3. Start generating clinical documentation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Healthcare Providers** — Reduce administrative burden by automating note-taking during or after patient encounters.
- **Medical Scribes** — Use AI-generated drafts as a starting point for high-accuracy clinical records.
- **Health Tech Developers** — Integrate clinical documentation capabilities into custom EHR or telehealth platforms.


## Available Tools
- **create_recording**: Create a new recording session or upload audio
- **get_clinical_notes**: Returns structured data including summary, HPI, physical exam, and assessment plan.

Retrieve generated clinical notes for a recording
- **get_recording_status**: Statuses can be pending, processing, completed, or failed.

Get the status of a recording processing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Abridge (AI Clinical Documentation API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new clinical recording for patient 'PT-882' using audio file 'encounter_01.mp3'."

**🤖 AI Agent:**
> I've started the recording session for patient PT-882. The recording ID is 'rec_abc123'. I will monitor the status for you.

---

**👤 You:**
> "What is the current status of the Abridge recording 'rec_abc123'?"

**🤖 AI Agent:**
> The recording 'rec_abc123' is currently in the 'processing' stage. It should be completed shortly.

---

**👤 You:**
> "Fetch the final clinical notes and assessment plan for recording 'rec_abc123'."

**🤖 AI Agent:**
> I've retrieved the notes. The HPI indicates a 45-year-old male with hypertension. The Assessment & Plan includes starting Lisinopril 10mg daily and a follow-up in 2 weeks.


## ❓ FAQ

**Q: How do I check if my audio file is still being processed?**
Use the `get_recording_status` tool with your unique recording ID. It will return whether the task is pending, processing, completed, or failed.

**Q: What kind of data is included in the clinical notes?**
The `get_clinical_notes` tool returns structured medical data including a summary, HPI (History of Present Illness), physical exam findings, and the assessment and plan.

**Q: Can I provide patient and provider IDs when creating a recording?**
Yes! The `create_recording` tool accepts optional `patient_id` and `provider_id` strings, as well as a metadata JSON object to provide full context for the encounter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/abridge-ai-clinical-documentation-api](https://vinkius.com/mcp/abridge-ai-clinical-documentation-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Abridge (AI Clinical Documentation API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `abridge-ai-clinical-documentation-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Abridge (AI Clinical Documentation API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "abridge-ai-clinical-documentation-api": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
