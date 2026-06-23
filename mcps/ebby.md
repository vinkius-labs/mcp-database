# Ebby MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ebby)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage audio transcriptions, track processing status, and retrieve text via the Ebby API.

## Description
Integrate **Ebby**, the powerful automatic transcription and subtitling platform, directly into your AI workflow. Manage your audio and video transcriptions, track real-time processing statuses and durations, retrieve transcribed text in various formats (TXT, SRT, VTT), and oversee speaker identification using natural language.

### What you can do

- **Transcription Oversight** — List and retrieve detailed information and status for all your audio and video transcription projects.
- **Content Intelligence** — Access the actual transcribed text content and identified speaker labels directly via chat.
- **Processing Monitoring** — Track real-time processing progress, file durations, and language settings for your media library.
- **Account Auditing** — Retrieve high-level summaries of transcription activity, remaining minutes, and organizational metadata instantly.

### How it works

1. Connect the Ebby integration to your AI assistant.
2. Authorize using your Ebby API Key (found in your account settings).
3. Orchestrate your media transcription and content analysis through intuitive conversation.

### Who is this for?

- **Content Creators** — Quickly check transcription status and retrieve text for scripts on the go.
- **Researchers & Journalists** — Search previous transcriptions and speaker labels via chat.
- **Operations Teams** — Monitor transcription volumes and remaining account balances instantly.


## Available Tools (10)
- **get_ebby_account_metadata**: Retrieve metadata and usage limits for your Ebby account
- **get_transcription_text**: Retrieve the transcribed text content for a specific file
- **quick_transcription_volume_audit**: Retrieve a high-level summary of transcription activity and processing rates
- **get_transcription_details**: Get detailed settings and status for a specific transcription
- **list_successfully_processed_audio**: Identify transcriptions that have finished processing and are ready for export
- **list_in_progress_transcriptions**: Identify transcriptions that are currently in the processing queue
- **list_latest_transcriptions**: Identify the most recently created or updated transcriptions
- **list_transcription_speakers**: List all speakers identified in a specific transcription
- **list_audio_transcriptions**: List all transcriptions created in your Ebby account
- **search_transcriptions_by_name**: Search for transcriptions using a filename or title keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ebby** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all completed transcriptions."

**🤖 AI Agent:**
> I've found 8 completed transcriptions, including 'Interview_John_Doe.mp3' and 'Q2_Board_Meeting.mp4'. Both are ready for export. Would you like to retrieve the text for the Interview?

---

**👤 You:**
> "Show me the transcribed text for 'Interview_John_Doe.mp3' in SRT format."

**🤖 AI Agent:**
> I've retrieved the SRT captions for 'Interview_John_Doe.mp3'. The file includes timestamps and identified speakers. Would you like the full JSON output or just a preview of the first few lines?

---

**👤 You:**
> "Check how many minutes are remaining in my Ebby account."

**🤖 AI Agent:**
> Your Ebby account has 150 transcription minutes remaining. Your current plan is 'Pro Monthly' and your next renewal is on April 15th. Should I list the most recent files currently in progress?


## ❓ FAQ

**Q: How do I get an Ebby API Key?**
Log in to your Ebby account, navigate to **Settings > API**, and you can generate or retrieve your unique API Key from there. Ensure you have available minutes in your balance.

**Q: What export formats are supported?**
Ebby supports exporting transcriptions in various formats including Plain Text (txt), Subtitles (srt, vtt), and Microsoft Word (docx). You can specify the format using the get_transcription_text tool.

**Q: Can the agent upload new audio files?**
This integration currently focuses on listing, auditing, and retrieving text for existing transcriptions. Uploading and starting new transcription jobs should be managed via the Ebby web interface.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ebby](https://vinkius.com/mcp/ebby)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ebby** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ebby` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ebby** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ebby": {
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
