# Play.ht (Voice Cloning) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/playht-voice-cloning)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/playht-voice-cloning-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/playht-voice-cloning-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Generate ultra-realistic speech and clone voices instantly using Play.ht's advanced AI voice engines directly from your agent.

## Description
Connect **Play.ht** to your AI agent to generate high-quality Text-to-Speech (TTS) and create instant voice clones through natural conversation.

### What you can do

- **Text-to-Speech Generation** — Convert text into lifelike audio using various engines like Play3.0-mini and PlayHT2.0-turbo.
- **Instant Voice Cloning** — Create a digital twin of any voice by simply providing a short audio sample.
- **Fine-grained Control** — Adjust speed, quality, emotion, and temperature to get the perfect vocal performance.
- **Multi-language Support** — Generate speech in multiple languages including English, French, Spanish, and more.

### How it works

1. Subscribe to this server
2. Enter your Play.ht User ID and API Key
3. Start generating audio and cloning voices from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — automate voiceovers for videos and podcasts without manual recording
- **Developers** — integrate realistic voice interactions into applications and games
- **Marketers** — create personalized audio messages and localized content at scale


## Available Tools
- **create_instant_voice_clone**: Provide the audio file as a base64 encoded string.

Create an instant voice clone from an audio sample
- **generate_tts_stream**: Generate audio from text using Play.ht TTS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Play.ht (Voice Cloning)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an MP3 of 'Hello, how are you today?' using voice ID 's3://voice-cloning-zero-shot/...' and the Play3.0-mini engine."

**🤖 AI Agent:**
> I've initiated the TTS generation using the Play3.0-mini engine. The audio stream is being processed for the text 'Hello, how are you today?' with the specified voice.

---

**👤 You:**
> "Create a new voice clone named 'My Assistant' using this base64 audio sample."

**🤖 AI Agent:**
> I am uploading the audio sample to create your instant voice clone 'My Assistant'. Once finished, you'll receive the unique Voice ID to use in TTS tasks.

---

**👤 You:**
> "Convert this text to speech with a happy emotion and 1.2x speed: 'I am so excited to meet you!'"

**🤖 AI Agent:**
> Generating audio with 'female_happy' emotion at 1.2x speed. The Play.ht engine is now synthesizing the speech for your request.


## Installation & Usage

To install and use the **Play.ht (Voice Cloning)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/playht-voice-cloning](https://vinkius.com/mcp/playht-voice-cloning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
