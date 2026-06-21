# Gladia (Speech AI) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gladia-speech-ai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gladia-speech-ai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gladia-speech-ai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transcribe, translate, and analyze audio with Gladia's high-speed Speech AI — support for pre-recorded files and live streaming.

## Description
Connect **Gladia** to your AI agent to unlock enterprise-grade speech-to-text capabilities. Process audio files or live streams with advanced features like speaker diarization, multi-language translation, and automated summarization.

### What you can do

- **Audio Processing** — Upload local files to generate secure URLs for immediate transcription processing.
- **Advanced Transcription** — Initiate jobs with speaker diarization (who said what), summarization, and translation across 100+ languages.
- **Audio-to-LLM** — Apply custom LLM prompts directly to your audio data to extract specific insights or structured data.
- **Live Streaming** — Initialize secure WebSocket sessions for real-time transcription of meetings or broadcasts.
- **Job Management** — List, retrieve, and manage your transcription history and results directly through conversation.

### How it works

1. Subscribe to this server
2. Enter your Gladia API Key
3. Start transcribing audio files or live streams from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Integrate speech-to-text workflows into apps without managing complex API calls manually.
- **Content Creators** — Quickly generate transcripts, summaries, and translations for podcasts or videos.
- **Business Teams** — Analyze meeting recordings to extract action items and speaker insights using natural language.


## Available Tools
- **delete_transcription**: Delete a transcription job
- **upload_audio_file**: Upload an audio file to Gladia
- **get_transcription**: Get status and results of a transcription job
- **list_transcriptions**: List pre-recorded transcriptions
- **init_live_session**: Initiate a live transcription session
- **init_transcription**: Start a pre-recorded transcription job


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gladia (Speech AI)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 5 most recent transcription jobs."

**🤖 AI Agent:**
> I've retrieved your recent jobs. You have 5 tasks: 'Meeting_Notes.mp3' (Done), 'Interview_01.wav' (Done), and 3 others. Would you like the results for any of these?

---

**👤 You:**
> "Start a transcription for this audio URL with summarization enabled: https://example.com/audio.mp3"

**🤖 AI Agent:**
> Transcription job initiated! The Job ID is `job_12345`. I've enabled summarization as requested. I'll monitor the status for you.

---

**👤 You:**
> "I need a WebSocket URL to start a live transcription session in 16000Hz."

**🤖 AI Agent:**
> I've generated a live session. Here is your secure WebSocket URL: `wss://api.gladia.io/v2/live/...`. The sample rate is set to 16000Hz.


## Installation & Usage

To install and use the **Gladia (Speech AI)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gladia-speech-ai](https://vinkius.com/mcp/gladia-speech-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
