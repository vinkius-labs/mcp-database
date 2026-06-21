# Lovo AI (Genny TTS & Voice Synthesis API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lovo-ai-genny-tts-voice-synthesis-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lovo-ai-genny-tts-voice-synthesis-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lovo-ai-genny-tts-voice-synthesis-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate high-quality AI voices and text-to-speech synthesis directly from your AI agent using Lovo AI's Genny API.

## Description
Connect **Lovo AI (Genny)** to your AI agent to transform text into lifelike speech. This server allows you to browse hundreds of premium voices and manage speech synthesis jobs through natural conversation.

### What you can do

- **Voice Discovery** — Use `list_voices` to browse all available AI speakers, filtering by language, gender, and style.
- **Speaker Details** — Use `get_speaker` to retrieve deep metadata for a specific voice ID to ensure the perfect tone for your content.
- **Speech Synthesis** — Use `create_tts_job` to convert text into audio with granular control over speed and emotional styles (e.g., cheerful, sad, professional).
- **Job Monitoring** — Use `get_tts_job` to track the status of your audio generation and retrieve the final output URLs once ready.

### How it works

1. Subscribe to this server
2. Enter your Lovo Genny API Key
3. Start generating professional voiceovers from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Generate narrations for videos or podcasts directly from your script-writing interface.
- **Developers** — Integrate high-fidelity voice synthesis into applications without leaving the code editor.
- **Marketers** — Quickly produce localized audio versions of ad copy and social media content.


## Available Tools
- **create_tts_job**: Submit a text-to-speech synthesis job
- **get_tts_job**: Check the status of a previously submitted TTS job
- **get_speaker**: Get detailed information about a specific speaker
- **list_voices**: List all available voices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lovo AI (Genny TTS & Voice Synthesis API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available English voices in Lovo AI."

**🤖 AI Agent:**
> I've retrieved the list of voices. You have access to speakers like 'Sophia' (ID: 632...), 'Mateo' (ID: 634...), and many others. Would you like to filter them by style or gender?

---

**👤 You:**
> "Create a TTS job for the text 'Welcome to the future of AI' using speaker ID 632c... with a cheerful style."

**🤖 AI Agent:**
> The TTS job has been submitted successfully. The Job ID is 'job_789abc'. I will monitor the status for you. Would you like me to check if it's finished now?

---

**👤 You:**
> "Check the status and get the audio link for job ID job_789abc."

**🤖 AI Agent:**
> The job 'job_789abc' is now complete! You can access your audio file here: [Audio URL]. The synthesis used the 'cheerful' style as requested.


## Installation & Usage

To install and use the **Lovo AI (Genny TTS & Voice Synthesis API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lovo-ai-genny-tts-voice-synthesis-api](https://vinkius.com/mcp/lovo-ai-genny-tts-voice-synthesis-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
