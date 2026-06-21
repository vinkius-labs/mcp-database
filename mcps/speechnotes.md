# Speechnotes MCP Server

Transcribe audio files, manage transcription jobs, and export text on Speechnotes with AI agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/speechnotes)

## Overview
**Category:** industry-titans
**Tools Count:** 12

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


## Installation & Usage

To install and use the **Speechnotes** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/speechnotes](https://vinkius.com/mcp/speechnotes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
