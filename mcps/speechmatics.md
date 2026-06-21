# Speechmatics MCP Server

Automate speech-to-text and text-to-speech — transcribe audio files, generate natural voices, and manage transcription jobs directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/speechmatics)

## Overview
**Category:** productivity
**Tools Count:** 8

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


## Installation & Usage

To install and use the **Speechmatics** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/speechmatics](https://vinkius.com/mcp/speechmatics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
