# ElevenLabs MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elevenlabs-alternative-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Generate lifelike speech, clone voices, and create sound effects using ElevenLabs' industry-leading AI audio technology.

## Description
Connect your **ElevenLabs** account to any AI agent to generate high-quality audio, manage voices, and process sound directly through natural conversation.

### What you can do

- **Text-to-Speech** — Convert text into lifelike speech using a wide array of pre-made or custom voices with granular control over stability and similarity.
- **Voice Management** — List, retrieve, edit, and delete voices in your library. You can even design new voices or find similar ones.
- **Speech-to-Speech** — Transform audio from one voice to another while maintaining emotion and delivery.
- **Audio Processing** — Isolate audio to remove background noise and create clean voice tracks.
- **Sound Effects** — Generate unique sound effects from text descriptions for games, videos, or presentations.
- **Project & Dubbing** — Manage long-form projects and create automated dubbing workflows across multiple languages.

### How it works

1. Subscribe to this server
2. Enter your ElevenLabs API Key
3. Start generating and managing audio from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — instantly generate voiceovers for videos and social media without leaving your workflow.
- **Developers** — integrate high-quality audio synthesis into applications and test voice settings via the AI agent.
- **Sound Designers** — quickly prototype sound effects and clean up audio recordings using AI-powered isolation.


## Available Tools
- **add_dictionary_from_file**: Add pronunciation dictionary from a PLS file
- **add_dictionary_from_rules**: Add pronunciation dictionary from rules
- **isolate_audio**: Remove background noise from audio
- **convert_speech**: Voice Changer (Speech to Speech)
- **create_agent**: Create a Conversational AI agent
- **create_designed_voice**: Save a designed voice
- **create_dub**: Create a dubbing project
- **create_project**: Create a Studio project
- **create_single_use_token**: Create a single-use token
- **create_speech**: Convert text to speech
- **delete_history_item**: Delete a history item
- **delete_voice**: Delete a custom voice
- **design_voice**: Design a new voice from a prompt
- **edit_voice**: Edit a custom voice
- **find_similar_voices**: Find similar voices in the library
- **generate_sound**: Generate sound effects from text
- **get_character_stats**: Get character usage statistics
- **get_dub_status**: Get status of a dubbing project
- **get_history_audio**: Download audio for a history item
- **get_history_item**: Get details of a history item
- **get_snapshot**: Get a project snapshot
- **get_user**: Get user info and subscription details
- **get_voice**: Get details for a specific voice
- **list_agent_branches**: List branches for a Conversational AI agent
- **list_agents**: List Conversational AI agents
- **list_dictionaries**: List pronunciation dictionaries
- **list_dubs**: List dubbing projects
- **list_history**: Get generated items history
- **list_models**: ).

List available models
- **list_projects**: List Studio projects
- **list_voices**: List available voices
- **stream_isolate_audio**: Stream audio isolation
- **stream_convert_speech**: Stream Voice Changer (Speech to Speech)
- **stream_speech**: Stream text to speech


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ElevenLabs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available voices in my ElevenLabs library."

**🤖 AI Agent:**
> I've retrieved your voices. You have 12 voices available, including 'Rachel' (ID: 21m00Tcm4TlvDq8ikWAM) and 'Clyde' (ID: 2EiwWnXFnvU5JabPnv8n). Would you like to use one of these for speech generation?

---

**👤 You:**
> "Generate a sound effect of a futuristic laser blast."

**🤖 AI Agent:**
> Generating sound effect... I've created a 'futuristic laser blast' audio. You can now download or play the generated sound effect.

---

**👤 You:**
> "Convert this text to speech using voice ID pNInz6obpgmqMArWsc7r: 'The future of audio is here.'"

**🤖 AI Agent:**
> Processing text-to-speech... I've generated the audio for your text using the specified voice. The high-quality speech file is ready.


## ❓ FAQ

**Q: How can I convert text to a specific voice using this server?**
You can use the `create_speech` tool. Simply provide the `voice_id` and the `text` you want to synthesize. The agent will generate the audio for you.

**Q: Can I see all the voices available in my account?**
Yes! Use the `list_voices` query. It will return a list of all available voices, including their IDs, names, and categories, so you can choose the right one for your project.

**Q: Is it possible to remove background noise from an existing audio file?**
Absolutely. Use the `isolate_audio` tool by providing the audio in base64 format. The server will process it and return a clean version with the background noise removed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elevenlabs-alternative-1](https://vinkius.com/mcp/elevenlabs-alternative-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ElevenLabs** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `elevenlabs-alternative-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ElevenLabs** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "elevenlabs-alternative-1": {
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
