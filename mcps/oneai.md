# OneAI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/oneai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/oneai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/oneai-mcp)
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


## Installation & Usage

To install and use the **OneAI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oneai](https://vinkius.com/mcp/oneai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
