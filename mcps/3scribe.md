# 3Scribe MCP Server

Automated audio and video transcription — create jobs, monitor progress, and retrieve text via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/3scribe)

## Overview
**Category:** productivity
**Tools Count:** 4

## Description
Unlock the power of spoken word with **3Scribe**, your automated partner for high-precision audio and video transcription. By connecting 3Scribe to your AI agent, you eliminate the friction of manual data entry from media files. Your agent can now orchestrate the entire transcription lifecycle—from submitting public URLs to auditing job statuses and retrieving final text—all through simple natural language commands. Whether it’s meeting minutes or video captions, your agent acts as a direct bridge to 3Scribe's powerful recognition engine.

### What you can do

- **Automated Transcription** — Create new transcription jobs by providing a public URL to your audio or video files
- **Job Monitoring** — Track the status of your transcriptions in real-time (Requested, Processing, Completed, Error)
- **Text Retrieval** — Access raw text transcripts or detailed word-level data with timestamps and speaker IDs
- **Project Management** — List all transcription jobs, filter by status, and delete old or unnecessary projects
- **Language Detection** — Specify transcription languages or let the AI auto-detect the spoken language

### How it works

1. Subscribe to this server
2. Enter your 3Scribe API Key
3. Start transcribing your media files through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — generate transcripts and captions for YouTube videos or podcasts instantly
- **Journalists & Researchers** — transcribe interviews and field recordings without manual effort
- **Business Professionals** — convert meeting recordings into searchable text for documentation
- **Developers** — integrate transcription capabilities into custom media workflows


## Available Tools
- **create_job**: You must provide a valid public URL. Returns a Job ID useful for tracking progress.

Initiate a new audio or video transcription job in 3Scribe via a public media URL
- **list_jobs**: Retrieve a paginated list of all transcription tasks from the 3Scribe account
- **get_job**: You must provide the Job ID.

Check the status and retrieve the generated text of a specific 3Scribe transcription job
- **delete_job**: This is an irreversible destructive action. Requires the Job ID.

Permanently delete a transcription task and its associated data from the 3Scribe account


## Installation & Usage

To install and use the **3Scribe** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/3scribe](https://vinkius.com/mcp/3scribe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
