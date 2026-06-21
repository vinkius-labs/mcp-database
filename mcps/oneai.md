# OneAI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/oneai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Analyze text and media with OneAI Language Skills—summarize, extract entities, and transcribe audio directly through your AI agent.

## Description
Connect **OneAI** to any AI agent to process text, audio, and video using a library of pre-trained Language Skills through natural conversation.

### What you can do

- **Text Analysis** — Run synchronous pipelines to summarize articles, detect sentiments, and extract entities from text input using `run_pipeline`.
- **Large File Processing** — Use asynchronous pipelines via `run_async_pipeline` for long documents or media files that require more processing time.
- **Audio Transcription** — Convert audio and video files into text with specialized transcription skills.
- **Task Monitoring** — Track the progress of long-running analysis tasks and retrieve results once completed using `get_async_task_status`.

### How it works

1. Subscribe to this server
2. Enter your OneAI API Key
3. Start processing content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — automatically summarize long articles or transcribe podcast episodes.
- **Data Analysts** — extract structured entities and sentiments from customer feedback or emails.
- **Developers** — integrate advanced NLP capabilities into your workflow without building custom models.


## Available Tools
- **get_async_task_status**: Check the status of an asynchronous OneAI pipeline task
- **run_async_pipeline**: Provide either content_url or input text, plus steps.

Run an asynchronous OneAI pipeline for large files or audio
- **run_pipeline**: g., summarize, entities, sentiments).

Run a synchronous OneAI language pipeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OneAI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Summarize this article and extract entities: [text]"

**🤖 AI Agent:**
> I've processed the text using `run_pipeline`. Here is the summary: [Summary]. I also found these entities: [Entities].

---

**👤 You:**
> "Transcribe the audio at this URL: https://example.com/audio.mp3"

**🤖 AI Agent:**
> I've started an asynchronous transcription task using `run_async_pipeline`. Your Task ID is `task_123`. You can check its status later.

---

**👤 You:**
> "Check the status of OneAI task task_123."

**🤖 AI Agent:**
> I've retrieved the status using `get_async_task_status`. The task is 'completed'. Here is the transcribed text: '...'


## ❓ FAQ

**Q: How can I summarize a text and extract entities at the same time?**
Use the `run_pipeline` tool. Provide your text in the `input` field and define the `steps` as a JSON array like `[{"skill":"summarize"}, {"skill":"entities"}]`.

**Q: What should I use for processing large audio files?**
Use `run_async_pipeline`. You can provide a `content_url` for the audio file and set the `steps` to include the `transcribe` skill. This starts a background task.

**Q: How do I know when my asynchronous processing is finished?**
Use the `get_async_task_status` tool with the `task_id` returned by the async pipeline. It will provide the current status and the final results once completed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oneai](https://vinkius.com/mcp/oneai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OneAI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `oneai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OneAI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oneai": {
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
