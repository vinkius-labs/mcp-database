# Play.ht (AI Voice Generation & TTS) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/playht-ai-voice-generation-tts)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/playht-ai-voice-generation-tts-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/playht-ai-voice-generation-tts-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate ultra-realistic AI voices and convert text to speech instantly using Play.ht's advanced neural engine.

## Description
Connect your **Play.ht** account to any AI agent to generate high-quality, human-like speech from text. This server provides direct access to Play.ht's extensive library of neural voices and advanced synthesis capabilities.

### What you can do

- **Voice Discovery** — List all available Play.ht voices, including metadata like language, gender, and unique voice IDs.
- **Instant Synthesis** — Convert text to speech immediately with customizable parameters for quality, format, and speaking speed.
- **Status Tracking** — Monitor the progress of long-running transcription requests using their unique IDs to ensure reliable delivery.
- **Customizable Output** — Fine-tune your audio by selecting specific formats (MP3, WAV) and quality levels (Draft to High).

### How it works

1. Subscribe to this server
2. Enter your Play.ht API Key and User ID
3. Start generating professional voiceovers directly from your AI agent

### Who is this for?

- **Content Creators** — Generate narrations for videos or podcasts without leaving your workflow.
- **Developers** — Integrate realistic TTS into applications or automate audio asset generation.
- **Accessibility Teams** — Quickly convert written documentation into clear, audible speech.


## Available Tools
- **convert_tts**: Convert text to speech instantly
- **get_tts_status**: Get conversion status for a TTS request
- **get_voices**: Get available Play.ht voices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Play.ht (AI Voice Generation & TTS)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available English voices from Play.ht."

**🤖 AI Agent:**
> I've retrieved the voices. You have access to several options like 'Larry' (Male), 'Susan' (Female), and 'William' (Male). Which one would you like to use for your text?

---

**👤 You:**
> "Convert 'Welcome to our AI platform' to speech using voice ID 's3://voice-id' in high quality."

**🤖 AI Agent:**
> Starting conversion... The request has been submitted. Your transcription ID is 'trans_123'. I will monitor the status for you.

---

**👤 You:**
> "Check the status of transcription ID 'trans_123'."

**🤖 AI Agent:**
> The conversion for 'trans_123' is complete! You can access your audio file at the generated URL.


## Installation & Usage

To install and use the **Play.ht (AI Voice Generation & TTS)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/playht-ai-voice-generation-tts](https://vinkius.com/mcp/playht-ai-voice-generation-tts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
