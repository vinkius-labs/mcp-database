# Speechmatics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/speechmatics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate speech-to-text and text-to-speech — transcribe audio files, generate natural voices, and manage transcription jobs directly.

## Description
Connect **Speechmatics** to your AI agent to handle advanced audio processing workflows. This server enables high-accuracy transcription and natural-sounding speech synthesis through a simple interface.

### What you can do

- **Batch Transcription** — Submit audio via URL or base64 and process large files with industry-leading accuracy using `create_job`.
- **Text-to-Speech (TTS)** — Convert text into natural human speech using high-quality voices like Sarah, Theo, Megan, or Jack via `generate_tts`.
- **Transcript Retrieval** — Export completed transcriptions in multiple formats including JSON, plain text, or SRT subtitles using `get_transcript`.
- **Job Management** — Monitor the status of your processing tasks, list recent activity, and manage resources with `list_jobs` and `get_job`.
- **Usage & Security** — Track your account consumption with `get_usage` and generate temporary keys for secure client-side access using `create_temp_key`.

### How it works

1. Subscribe to this server
2. Enter your Speechmatics API Key
3. Start transcribing audio or generating speech directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Content Creators** — Automatically generate subtitles (SRT) for videos or transcribe podcasts in seconds.
- **Developers** — Integrate speech capabilities into apps without managing complex audio infrastructure.
- **Data Analysts** — Convert large volumes of recorded meetings or calls into searchable text for analysis.


## Available Tools
- **create_job**: Create a new batch transcription job
- **create_temp_key**: Create a temporary API key
- **delete_job**: Delete a transcription job
- **generate_tts**: Generate speech from text (TTS)
- **get_job**: Get details for a specific job
- **get_transcript**: Retrieve the transcript for a job
- **get_usage**: Get usage statistics
- **list_jobs**: List recent transcription jobs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Speechmatics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Transcribe the audio file at this URL: https://example.com/audio.mp3"

**🤖 AI Agent:**
> I've started a new transcription job (ID: j123abc). I'll use the default English configuration. You can check its status using `get_job`.

---

**👤 You:**
> "Generate an audio file of Sarah saying 'Welcome to the future of speech technology'."

**🤖 AI Agent:**
> Generating speech with Sarah's voice... Done! You can now access the synthesized audio for the text provided.

---

**👤 You:**
> "List my 5 most recent transcription jobs."

**🤖 AI Agent:**
> Fetching your recent jobs... I found 5 jobs. The most recent one is 'Meeting_Notes.mp3' (ID: j987xyz) which is currently 'completed'.


## ❓ FAQ

**Q: What formats can I get my transcripts in?**
You can use the `get_transcript` tool to retrieve results in `json`, `txt`, or `srt` (subtitle) formats. Simply specify the `format` parameter when calling the tool.

**Q: Which voices are available for Text-to-Speech?**
The `generate_tts` tool supports four high-quality voices: `sarah`, `theo`, `megan`, and `jack`. You can choose the one that best fits your content's tone.

**Q: How do I check if my transcription job is finished?**
Use the `get_job` tool with your specific `job_id`. It will return the current status (e.g., running, completed) and metadata about the processing task.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/speechmatics](https://vinkius.com/mcp/speechmatics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Speechmatics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `speechmatics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Speechmatics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "speechmatics": {
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
