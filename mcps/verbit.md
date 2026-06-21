# Verbit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/verbit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate professional transcription and captioning via Verbit — upload media, track job progress, and retrieve transcripts in multiple formats directly from your AI agent.

## Description
Connect your **Verbit** account to any AI agent to streamline your professional transcription and captioning workflows. This server allows you to handle high-quality speech-to-text tasks through simple conversation.

### What you can do

- **Transcription Jobs** — Create new transcription jobs by providing public media URLs and specifying languages.
- **Status Tracking** — Monitor the real-time progress and status of your transcription requests using unique job IDs.
- **Transcript Retrieval** — Download completed transcripts in various formats including JSON, TXT, SRT, VTT, or DOCX for immediate use.
- **External Referencing** — Tag jobs with external IDs to maintain consistency with your internal database or project management tools.

### How it works

1. Subscribe to this server
2. Enter your Verbit API Key
3. Start managing your transcription pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators & Media Teams** — quickly generate captions (SRT/VTT) for videos without leaving your workflow.
- **Legal & Academic Professionals** — automate the transcription of recordings and interviews into structured documents.
- **Product Managers** — integrate transcription status checks into automated project reports.


## Available Tools
- **create_job**: Upload a media file for transcription
- **get_job**: Check the progress of a transcription job
- **get_transcript**: Download the completed transcript


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Verbit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a transcription job for this audio file: https://example.com/interview.mp3"

**🤖 AI Agent:**
> I've started the transcription job for your file. The Job ID is 'vbt_98765'. You can check its progress anytime.

---

**👤 You:**
> "What is the current status of Verbit job vbt_98765?"

**🤖 AI Agent:**
> Checking the status... Job 'vbt_98765' is currently at 75% progress and is in the 'In Progress' state.

---

**👤 You:**
> "Download the transcript for job vbt_98765 in Word format."

**🤖 AI Agent:**
> I've retrieved the transcript for job 'vbt_98765' in DOCX format. You can access the content here.


## ❓ FAQ

**Q: How do I start a new transcription job using a video link?**
Use the `create_job` tool. Simply provide the `file_url` of your media and optionally specify the `language` and a `title` to identify the job later.

**Q: Can I download subtitles for my video in SRT format?**
Yes! Once the job is finished, use the `get_transcript` tool with your `job_id` and set the `format` parameter to 'srt'.

**Q: How can I check if my transcription is already finished?**
You can use the `get_job` tool. By providing the `job_id`, the agent will return the current status and progress percentage of your transcription.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/verbit](https://vinkius.com/mcp/verbit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Verbit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `verbit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Verbit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "verbit": {
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
