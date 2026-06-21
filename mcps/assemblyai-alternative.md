# AssemblyAI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/assemblyai-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/assemblyai-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/assemblyai-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Transcribe audio and video files with industry-leading accuracy, detect speakers, and extract insights from spoken content.

## Description
Connect your **AssemblyAI** account to any AI agent and take full control of your high-fidelity audio transcription and speech intelligence workflows through natural conversation.

### What you can do

- **Speech-to-Text Orchestration** — Programmatically transcribe public audio or video URLs using state-of-the-art MARS models with superhuman accuracy
- **Audio Intelligence** — Extract high-fidelity insights including automated summaries, sentiment analysis, and topic detection directly through your agent
- **Speaker Diarization Architecture** — Retrieve detailed utterances separated by speaker labels to coordinate meeting minutes and interview transcripts perfectly
- **Content Discovery** — Access automated chapters and high-fidelity video recaps to maintain a perfectly coordinated media library
- **Lifecycle Management** — Monitor transcription job status and manage your directory of recent transcripts directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the AssemblyAI dashboard
3. Start localizing and analyzing your audio assets from Claude, Cursor, or any MCP client

No more manual uploading to web portals or waiting for slow human transcriptions. Your AI acts as your dedicated audio engineer and linguistic analyst.

### Who is this for?

- **Content Creators** — instantly generate podcast transcripts and video chapters using natural language commands
- **Support & Sales Teams** — summarize meeting recordings and analyze customer sentiment without leaving your workspace
- **Developers** — integrate high-speed speech-to-text intelligence into custom business workflows through simple AI queries


## Available Tools
- **delete_transcript**: Delete a transcript
- **get_chapters**: Get auto-chapters
- **get_sentiments**: Get sentiment analysis
- **get_speakers**: Get speaker labels
- **get_summary**: Get auto-summary
- **get_topics**: Get topic detection
- **get_transcript**: Get transcript status/result
- **list_transcripts**: List recent transcripts
- **transcribe_audio_url**: Transcribe audio URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AssemblyAI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Transcribe this podcast URL: 'https://example.com/audio.mp3' and enable speaker diarization."

**🤖 AI Agent:**
> Transcription started! I've submitted the URL to AssemblyAI with speaker labels enabled. The job ID is 'tr_123'. I'll monitor the processing status and notify you as soon as the high-fidelity transcript is ready.

---

**👤 You:**
> "Show my 5 most recent transcription jobs."

**🤖 AI Agent:**
> I've retrieved your recent jobs. You have 5 completed transcripts, including 'Team Weekly Sync' and 'Product Interview'. Would you like to extract the high-fidelity summary for the sync meeting?

---

**👤 You:**
> "Get the sentiment analysis for transcript 'tr_123'."

**🤖 AI Agent:**
> Accessing audio intelligence... Transcript tr_123 shows a primarily 'Positive' sentiment with peaks of 'Neutral' during the technical breakdown. I've retrieved the high-fidelity timestamped segments for you. Need more insights?


## Installation & Usage

To install and use the **AssemblyAI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/assemblyai-alternative](https://vinkius.com/mcp/assemblyai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
