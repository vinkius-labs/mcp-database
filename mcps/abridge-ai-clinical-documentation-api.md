# Abridge (AI Clinical Documentation API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/abridge-ai-clinical-documentation-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/abridge-ai-clinical-documentation-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/abridge-ai-clinical-documentation-api-mcp)
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


## Installation & Usage

To install and use the **Abridge (AI Clinical Documentation API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/abridge-ai-clinical-documentation-api](https://vinkius.com/mcp/abridge-ai-clinical-documentation-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
