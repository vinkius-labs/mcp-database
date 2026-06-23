# Cartesia (Voice AI) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cartesia-voice-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Generate lifelike AI voices, clone speech, and transcribe audio with Cartesia's state-of-the-art Sonic models directly from your AI agent.

## Description
Connect **Cartesia** to your AI agent to unlock high-performance voice synthesis and speech recognition. Cartesia's Sonic models provide industry-leading latency and quality for real-time applications.

### What you can do

- **Text-to-Speech (TTS)** — Generate high-fidelity audio bytes or stream via SSE using models like Sonic 3.5 and Sonic 3.
- **Speech-to-Text (STT)** — Transcribe audio files into text using the Ink Whisper model with multi-language support.
- **Voice Cloning** — Create custom voice models from as little as 5 seconds of audio input.
- **Voice Management** — List, retrieve, and update voices, or use the Voice Changer to transform existing audio.
- **Pronunciation Control** — Manage custom pronunciation dictionaries for specialized terminology or accents.
- **Agent Orchestration** — List and manage AI agents and monitor call logs and usage credits.

### How it works

1. Subscribe to this server
2. Enter your Cartesia API Key
3. Start generating audio or transcribing speech from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — integrate real-time voice synthesis into applications without managing complex infrastructure.
- **Content Creators** — automate voiceovers and audio localization using high-quality cloned voices.
- **Product Teams** — build conversational AI agents that sound human and respond with sub-second latency.


## Available Tools (20)
- **get_voice**: Get details for a specific voice
- **list_agent_calls**: List calls and transcripts for a specific agent
- **update_voice**: Update voice metadata
- **clone_voice**: Clone a voice from a 5s audio clip
- **create_pronunciation_dict**: Create a new pronunciation dictionary
- **delete_pronunciation_dict**: Delete a pronunciation dictionary
- **delete_voice**: Delete a voice
- **generate_access_token**: Generate a short-lived access token for client-side requests
- **get_agent**: Get details for a specific voice agent
- **get_usage_credits**: Get credit usage statistics
- **infill_bytes**: Generate audio to smoothly connect two existing segments
- **list_agents**: List all voice agents
- **list_pronunciation_dicts**: List pronunciation dictionaries
- **list_voices**: List available voices
- **localize_voice**: Adapt a voice to a new language/dialect
- **stt_batch**: Transcribe audio file to text (Batch STT)
- **tts_bytes**: Generate text-to-speech audio bytes
- **tts_sse**: Generate text-to-speech via Server-Sent Events
- **update_pronunciation_dict**: Update a pronunciation dictionary
- **voice_changer_bytes**: Change voice of an audio clip while preserving intonation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cartesia (Voice AI)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available voices in my Cartesia account."

**🤖 AI Agent:**
> I've retrieved the list of voices. You have access to several models, including 'Baritone' (ID: 79a045e3...), 'British Lady' (ID: 123x-456y...), and your custom cloned voices. Which one would you like to use?

---

**👤 You:**
> "Generate a WAV audio file saying 'Welcome to the future of AI' using voice ID 79a045e3-a621-4923-b05c-8029db0dffca."

**🤖 AI Agent:**
> Generating audio... I've synthesized the text using the Sonic-3.5 model. The WAV file is ready for download.

---

**👤 You:**
> "Check my current usage credits on Cartesia."

**🤖 AI Agent:**
> You currently have 45,200 credits remaining in your account. Your last billing cycle refreshed on the 1st of the month.


## ❓ FAQ

**Q: Can I generate audio in different formats like MP3 or WAV?**
Yes. Using the `tts_bytes` tool, you can specify the `output_format_container` as 'mp3', 'wav', or 'raw', and configure the sample rate and encoding to match your needs.

**Q: How do I transcribe an existing audio file to text?**
Use the `stt_batch` tool. Provide the base64 encoded audio file, specify the model (e.g., 'ink-whisper'), and the language code to receive a full transcription.

**Q: Is it possible to clone a voice using this integration?**
Absolutely. The `clone_voice` tool allows you to create a new voice model by uploading a short (approx. 5s) base64 encoded audio clip.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cartesia-voice-ai](https://vinkius.com/mcp/cartesia-voice-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cartesia (Voice AI)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cartesia-voice-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cartesia (Voice AI)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cartesia-voice-ai": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
