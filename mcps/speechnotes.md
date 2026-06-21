# Speechnotes MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/speechnotes)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Transcribe audio files, manage transcription jobs, and export text on Speechnotes with AI agents.

## Description
Connect your **Speechnotes** account to any AI agent to automate your professional audio transcription and speech-to-text orchestration. Speechnotes provides a high-accuracy AI engine for converting audio files into text, and this integration allows you to initiate transcription jobs from URLs, monitor progress, and export results through natural conversation.

### What you can do

- **Transcription Orchestration** — Initiate new transcription jobs from audio URLs and retrieve real-time status updates programmatically.
- **Job & History Lifecycle Management** — List all past transcription jobs and retrieve detailed metadata, including timestamps and speaker counts directly from the AI interface.
- **Export & Format Control** — Retrieve transcribed text in multiple formats (TXT, DOCX, SRT) and manage file exports via simple AI commands.
- **Language & Model Intelligence** — Access available transcription languages and AI models to ensure your results are optimized for your specific content.
- **Operational Monitoring** — Check your account credits, monitor usage statistics, and manage webhooks to ensure your transcription pipeline is always synchronized.

### How it works

1. Subscribe to this server
2. Enter your Speechnotes API Key and API Secret from your developer dashboard
3. Start generating high-accuracy transcriptions from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Journalists & Content Creators** — quickly transcribe interviews and podcasts without switching apps.
- **Researchers** — automate the retrieval of meeting transcriptions and monitor processing progress via natural conversation.
- **Operations Teams** — streamline the export of transcribed text and monitor account credits directly within the chat.


## Available Tools
- **remove_transcription_job**: Delete job record
- **get_remaining_credits**: Check account balance
- **get_transcription_export**: Export result format
- **list_transcription_models**: Get engine models
- **generate_webhook_signature**: Sign payload
- **get_transcription_status**: Check job progress
- **get_usage_statistics**: Check usage logs
- **list_transcription_history**: List past jobs
- **list_supported_languages**: Get language codes
- **list_configured_webhooks**: Get delivery endpoints
- **test_speechnotes_auth**: Check connection
- **transcribe_audio_url**: Transcribe remote file


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Speechnotes** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Transcribe the audio file at this URL: 'https://example.com/interview.mp3'."

**🤖 AI Agent:**
> Transcription job started! I've triggered the process for your audio file. You can check the status using the provided Job ID: SN-789.

---

**👤 You:**
> "Transcribe the latest team meeting recording and generate a summary with action items."

**🤖 AI Agent:**
> Transcription complete. Meeting: "Engineering Weekly" (47 minutes, 6 participants). Accuracy: 96.2%. Summary: Sprint 13 review (8 stories completed, 2 carried over), API performance discussion (latency reduced 30%), new hire onboarding plan, Q3 roadmap preview. Action items: 1) Sarah: fix authentication bug by Friday. 2) James: prepare load testing plan by Monday. 3) Alex: schedule architecture review for database migration. 4) Lisa: update API documentation for v3 endpoints. 5) David: onboard new engineer (start date May 19). Word count: 5,670. Speakers identified: 6.

---

**👤 You:**
> "Show me all transcriptions from the past week with their word counts and language detection."

**🤖 AI Agent:**
> 12 transcriptions last week. Total audio processed: 8.4 hours. Languages: English (9), Spanish (2), Portuguese (1). Longest: "Board Meeting" (2h 15m, 14,500 words). Shortest: "Quick Standup" (8 min, 890 words). Average accuracy: 95.8%. "Sales Call - Meridian" (45 min, 4,200 words, EN). "Customer Interview" (30 min, 3,100 words, EN). "Marketing Brainstorm" (1h, 6,800 words, EN). "Team Retrospective" (35 min, 3,600 words, EN). 5 additional transcriptions. Storage used: 234 MB. Export formats available: TXT, SRT, VTT, DOCX.


## ❓ FAQ

**Q: How do I find my Speechnotes API credentials?**
Log in to your Speechnotes account and navigate to the API or developer section in your dashboard to find your unique API Key and API Secret.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/speechnotes](https://vinkius.com/mcp/speechnotes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Speechnotes** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `speechnotes` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Speechnotes** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "speechnotes": {
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
