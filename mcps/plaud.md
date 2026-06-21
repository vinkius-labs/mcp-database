# Plaud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plaud)
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


## ❓ FAQ

**Q: How do I find my Plaud Access Token?**
Log in to [**web.plaud.ai**](https://web.plaud.ai), open DevTools (F12), go to **Application** > **Local Storage**, and look for `tokenstr`. Copy and paste it into the field below.

**Q: What is the Plaud API Domain?**
It is the base URL for the Plaud API (e.g., `https://api-euc1.plaud.ai`). You can find it in your browser's Local Storage under `plaud_user_api_domain`.

**Q: Can the agent retrieve full AI summaries?**
Yes. Use the `get_summary` tool with the File ID. Your agent will fetch the structured AI summary, including key points and action items.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plaud](https://vinkius.com/mcp/plaud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plaud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `plaud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plaud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plaud": {
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
