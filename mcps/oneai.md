# OneAI MCP Server

Analyze text and media with OneAI Language Skills—summarize, extract entities, and transcribe audio directly through your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/oneai)

## Overview
**Category:** developer-tools
**Tools Count:** 3

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


## Installation & Usage

To install and use the **OneAI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oneai](https://vinkius.com/mcp/oneai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
