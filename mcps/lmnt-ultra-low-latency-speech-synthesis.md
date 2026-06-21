# LMNT (Ultra-low Latency Speech Synthesis) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lmnt-ultra-low-latency-speech-synthesis)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lmnt-ultra-low-latency-speech-synthesis-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lmnt-ultra-low-latency-speech-synthesis-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Synthesize ultra-low latency AI speech, clone voices instantly, and manage your LMNT audio assets directly from any AI agent.

## Description
Connect **LMNT** to your AI agent to generate high-quality, lifelike speech with industry-leading speed. Perfect for real-time applications, accessibility, and content creation.

### What you can do

- **Speech Synthesis** — Convert text to audio in milliseconds using the `generate_speech` tool with support for multiple languages and formats.
- **Voice Cloning** — Create instant voice clones by uploading audio samples via `create_voice`.
- **Voice Management** — List, inspect, update, or delete your custom and system voices using `list_voices`, `get_voice`, and `delete_voice`.
- **Account Monitoring** — Keep track of your usage and plan limits with `get_account`.

### How it works

1. Subscribe to this server
2. Enter your LMNT API Key
3. Start generating audio from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — building real-time conversational AI or voice-enabled applications.
- **Content Creators** — looking to automate voiceovers or localize content quickly.
- **Accessibility Teams** — creating responsive tools for users with visual impairments.


## Available Tools
- **create_voice**: Create a new voice (Instant Cloning)
- **delete_voice**: Delete a voice by ID
- **generate_speech**: Returns a base64 encoded audio stream.

Generates speech from text and returns base64 audio
- **get_account**: Retrieve account usage and plan information
- **get_voice**: Retrieve a specific voice by ID
- **list_voices**: List available voices
- **update_voice**: Update an existing voice


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LMNT (Ultra-low Latency Speech Synthesis)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the voices I have access to."

**🤖 AI Agent:**
> I've retrieved the available voices. You have access to system voices like 'Aura' (ID: aura) and 'Lily' (ID: lily), as well as your custom clones. Would you like to hear a sample of one?

---

**👤 You:**
> "Synthesize 'Welcome to the future of speech' using the voice ID 'lily' in MP3 format."

**🤖 AI Agent:**
> Generating audio... Done! I've synthesized the text using the 'Lily' voice. The MP3 audio is ready for playback or download.

---

**👤 You:**
> "Show me my current LMNT account usage and plan info."

**🤖 AI Agent:**
> Your account is currently on the 'Pro' plan. You have used 45,000 characters out of your 1,000,000 monthly limit. Your next billing cycle resets in 12 days.


## Installation & Usage

To install and use the **LMNT (Ultra-low Latency Speech Synthesis)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lmnt-ultra-low-latency-speech-synthesis](https://vinkius.com/mcp/lmnt-ultra-low-latency-speech-synthesis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
