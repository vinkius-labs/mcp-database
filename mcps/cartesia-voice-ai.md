# Cartesia (Voice AI) MCP Server

Generate lifelike AI voices, clone speech, and transcribe audio with Cartesia's state-of-the-art Sonic models directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cartesia-voice-ai)

## Overview
**Category:** ai-frontier
**Tools Count:** 20

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


## Available Tools
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


## Installation & Usage

To install and use the **Cartesia (Voice AI)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cartesia-voice-ai](https://vinkius.com/mcp/cartesia-voice-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
