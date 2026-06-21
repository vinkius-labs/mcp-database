# AssemblyAI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/assemblyai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Transcribe and audit audio — manage speech-to-text jobs via AI.

## Description
Empower your AI agent to orchestrate your entire audio intelligence and transcription workflow with **AssemblyAI**, the leading platform for speech-to-text. By connecting AssemblyAI to your agent, you transform complex audio processing into a natural conversation. Your agent can instantly start transcription jobs from any URL, audit transcript results with high confidence, and manage job history without you ever touching a technical console. Whether you are analyzing podcast content or transcribing meetings, your agent acts as a real-time linguistic assistant, ensuring your audio data is always accessible and searchable.

### What you can do

- **Transcription Auditing** — Start transcription jobs for any audio or video URL and retrieve cleaned text with speaker labels.
- **Linguistic Oversight** — Retrieve transcripts broken down by sentences or paragraphs to maintain a structured view of spoken content.
- **Status Intelligence** — Monitor the progress of long-running transcription jobs to ensure timely data delivery.
- **Execution Management** — List all past and active transcripts to maintain strict organizational control over your audio assets.
- **Confidence Intelligence** — Retrieve confidence scores for each transcription to verify the accuracy of your linguistic data.

### How it works

1. Subscribe to this server
2. Enter your AssemblyAI API Key
3. Start managing your audio intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — monitor podcast transcriptions and retrieve speaker metadata straight from your workflow.
- **Data Analysts** — verify transcription accuracy and audit linguistic trends across multiple files.
- **Operations Leads** — perform rapid audits of meeting records and retrieve key summaries through natural language.
- **AI Developers** — automate audio data querying to orchestrate cross-functional media intelligence teams smoothly.


## Available Tools
- **delete_transcript**: Delete a transcription record
- **get_transcript_paragraphs**: Get the transcript broken down by paragraphs
- **get_transcript_sentences**: Get the transcript broken down by sentences
- **get_transcript**: Get the result of a transcription job
- **list_transcripts**: List all transcription jobs
- **transcribe_audio**: Start a transcription job for an audio/video URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AssemblyAI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Transcribe the audio file at https://example.com/podcast.mp3 using AssemblyAI."

**🤖 AI Agent:**
> Transcription job started! The Job ID is `transcript_123`. I'll monitor the status for you. Once completed, I can provide the full text or speaker labels.

---

**👤 You:**
> "Show me the result for transcript ID xxxx."

**🤖 AI Agent:**
> I've retrieved the transcript. It has a confidence of 98%. The content discusses the latest AI trends. Would you like the text broken down by paragraphs?

---

**👤 You:**
> "List all my past AssemblyAI transcripts."

**🤖 AI Agent:**
> I've retrieved your transcript history. You have 10 completed jobs, including recordings from last week's webinars. Would you like the details for any specific job?


## ❓ FAQ

**Q: How do I find my AssemblyAI API Key?**
Log in to your [**AssemblyAI dashboard**](https://www.assemblyai.com/app), and you will find your API Key on the main home page. Copy and paste it below.

**Q: What audio formats are supported?**
AssemblyAI supports most common audio and video formats, including MP3, WAV, AAC, MP4, and others. Simply provide a public URL to the file.

**Q: Can the agent identify different speakers?**
Yes. When starting a job via `transcribe_audio`, set the `speaker_labels` parameter to true. Your agent will return the text categorized by speaker ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/assemblyai](https://vinkius.com/mcp/assemblyai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AssemblyAI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `assemblyai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AssemblyAI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "assemblyai": {
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
