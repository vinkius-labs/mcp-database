# Inworld AI MCP Server

Power your AI agents with Inworld's lifelike voices, voice cloning, and advanced character orchestration routers.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/inworld-ai)

## Overview
**Category:** artificial-intelligence
**Tools Count:** 19

## Description
Connect **Inworld AI** to your agent to unlock advanced multimodal capabilities. This server provides a comprehensive suite of tools for high-fidelity voice synthesis, custom voice design, and intelligent character routing.

### What you can do

- **Voice Synthesis (TTS)** — Generate high-quality speech synchronously or via streaming using advanced models like `inworld-tts-2`.
- **Voice Cloning & Design** — Clone voices from audio samples using `clone_voice` or describe a voice with text prompts using `design_voice` to create unique personas.
- **Character Orchestration** — Manage AI routers with `create_router` and `chat_completions` to build complex, context-aware conversational experiences.
- **Voice Library Management** — List, update, and organize your workspace's voice assets and published models.
- **Speech-to-Text (STT)** — Transcribe audio files directly into text for seamless agent processing.

### How it works

1. Subscribe to this server
2. Enter your Inworld API Key and API Secret from the Inworld Studio
3. Start generating speech and managing AI characters from Claude, Cursor, or any MCP client

### Who is this for?

- **Game Developers** — Create dynamic, voiced NPCs with unique personalities and real-time responses.
- **Content Creators** — Automate voiceovers and character dialogue using custom-designed or cloned voices.
- **AI Engineers** — Build sophisticated agentic workflows that require advanced routing and multimodal interaction.


## Available Tools
- **chat_completions**: Generate chat completions via LLM Router
- **clone_voice**: Clone a voice from audio samples
- **create_realtime_call**: Create a WebRTC realtime call
- **create_router**: Create an LLM Router
- **delete_router**: Delete an LLM Router
- **delete_voice**: Delete a voice
- **design_voice**: Design a voice from a text prompt
- **get_router**: Get details for a specific LLM Router
- **get_voice**: Get details for a specific voice
- **list_models**: List available LLM models
- **list_routers**: List all LLM Routers
- **list_tts_voices**: Use list_voices instead for newer Voice API.

List TTS voices (Deprecated)
- **list_voices**: List voices in the workspace
- **publish_voice**: Publish a draft/preview voice
- **synthesize_speech_stream**: Synthesize speech via streaming
- **synthesize_speech_sync**: Synthesize speech synchronously
- **transcribe_audio**: Transcribe audio to text (Sync)
- **update_router**: Update an LLM Router
- **update_voice**: Update a voice


## Installation & Usage

To install and use the **Inworld AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inworld-ai](https://vinkius.com/mcp/inworld-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
