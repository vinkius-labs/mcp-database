# Abridge (AI Clinical Documentation API) MCP Server

Automate clinical documentation with Abridge — create recordings, track processing status, and retrieve structured medical notes directly via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/abridge-ai-clinical-documentation-api)

## Overview
**Category:** artificial-intelligence
**Tools Count:** 3

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


## Installation & Usage

To install and use the **Abridge (AI Clinical Documentation API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/abridge-ai-clinical-documentation-api](https://vinkius.com/mcp/abridge-ai-clinical-documentation-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
