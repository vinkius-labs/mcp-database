# Plaud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plaud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/plaud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/plaud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Plaud AI recordings — audit transcripts and summaries via AI.

## Description
Empower your AI agent to orchestrate your entire voice-to-intelligence ecosystem with **Plaud**, the AI voice recorder. By connecting Plaud to your agent, you transform complex recording management into a natural conversation. Your agent can instantly list your files, retrieve AI-generated transcripts, and audit meeting summaries without you ever touching a dashboard. Whether you are capturing client meetings, lectures, or personal notes, your agent acts as a real-time intelligence assistant, ensuring your spoken data is always accessible and organized.

### What you can do

- **Recording Auditing** — List all recordings in your account and retrieve detailed metadata for each, including creation dates.
- **Intelligence Extraction** — Query full transcripts and AI summaries for any recording instantly to capture key insights.
- **Organization Management** — List all folders and tags to keep your recording library structured and easy to browse.
- **Data Governance** — Update file names and autonomously delete recordings when they are no longer needed.
- **Asset Access** — Retrieve secure download URLs for your audio files to maintain local backups or share recordings.

### How it works

1. Subscribe to this server
2. Enter your Plaud Access Token and API Domain
3. Start managing your voice data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Professionals** — monitor meeting recordings and retrieve summaries straight from your workflow.
- **Students** — verify if lecture transcripts have been correctly generated and organized by the agent.
- **Content Creators** — perform rapid audits of voice notes and extract content ideas without manual dashboard logins.
- **Operations Leads** — automate recording querying to orchestrate cross-functional team intelligence smoothly.


## Available Tools
- **delete_file**: Delete a Plaud recording
- **get_download_url**: Get MP3 download URL for a recording
- **get_file_detail**: Get details for a specific recording
- **get_me**: Get Plaud account details
- **get_summary**: Get AI summary for a recording
- **get_transcript**: Get transcription for a recording
- **list_files**: List all Plaud recordings
- **list_folders**: List all recording folders
- **list_tags**: List all recording tags
- **update_file**: Update recording metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plaud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 recordings in Plaud."

**🤖 AI Agent:**
> I've retrieved your recent recordings. You have 5 files, including 'Client Meeting Q4' and 'Podcast Draft'. Would you like the transcript for any of them?

---

**👤 You:**
> "Summarize the recording titled 'Strategy Session'."

**🤖 AI Agent:**
> I've analyzed the 'Strategy Session'. The main points discussed were the 2024 budget and the new hiring plan. I can provide the full AI summary if you'd like.

---

**👤 You:**
> "Show me my recording folders."

**🤖 AI Agent:**
> You have 3 folders in Plaud: 'Work', 'Personal', and 'Archive'. I can list the recordings inside any of these folders for you.


## Installation & Usage

To install and use the **Plaud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plaud](https://vinkius.com/mcp/plaud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
