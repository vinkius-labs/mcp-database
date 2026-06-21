# Castmagic MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/castmagic)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/castmagic-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/castmagic-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate audio and video content repurposing via Castmagic — generate transcripts, show notes, and social posts directly from any AI agent.

## Description
Connect your **Castmagic** account to any AI agent and take full control of your content repurposing workflow through natural conversation. Transform long-form audio and video into ready-to-use assets instantly.

### What you can do

- **Instant Transcription** — Submit audio/video URLs and retrieve high-accuracy transcripts with speaker identification natively
- **Magic Content Generation** — Generate AI-driven show notes, summaries, social media posts, and titles flawlessly
- **Speaker Analysis** — List and manage identified speakers within your recordings to refine transcript metadata securely
- **Asset Management** — List all uploaded recordings and transcripts to organize your content library in real-time
- **Quota Oversight** — Retrieve account and subscription information to monitor your usage and limits directly
- **Automated Workflows** — Submit new content for processing and delete old transcripts directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Castmagic Secret Key (obtained from your Developer Dashboard)
3. Start repurposing your content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Podcasters** — generate show notes and social clips from latest episodes using natural language
- **Content Marketers** — transform webinars and videos into blog posts and social updates without manual work
- **Creators** — audit and manage their entire audio content library straight from their chat interface
- **Agencies** — automate transcript delivery and content drafting for multiple client projects


## Available Tools
- **create_new_transcript**: Submit a new audio or video URL for transcription
- **delete_transcript**: Delete a transcript and its associated data
- **get_castmagic_account**: Retrieve core account and quota information
- **get_magic_content**: Retrieve AI-generated content (show notes, social posts) for a transcript
- **get_transcript_details**: Get details and text for a specific transcript
- **list_castmagic_recordings**: List all uploaded recordings
- **list_transcript_speakers**: List identified speakers in a transcript
- **list_transcripts**: List all audio/video transcripts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Castmagic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Transcribe this audio file: https://example.com/episode1.mp3"

**🤖 AI Agent:**
> Submitting 'episode1.mp3' for transcription... I've started the job (ID: tr_12345). I'll let you know when it's finished processing.

---

**👤 You:**
> "Get the magic content for transcript ID tr_12345."

**🤖 AI Agent:**
> Retrieving AI assets for tr_12345... I found show notes, 3 LinkedIn posts, and 5 suggested titles. Which one should I display first?

---

**👤 You:**
> "Show me my last 10 recordings in Castmagic."

**🤖 AI Agent:**
> Retrieving your recent recordings... I found 10 entries including 'Weekly Sync' and 'Product Launch Interview'. All are successfully processed.


## Installation & Usage

To install and use the **Castmagic** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/castmagic](https://vinkius.com/mcp/castmagic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
