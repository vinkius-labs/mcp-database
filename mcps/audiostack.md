# AudioStack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/audiostack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Produce end-to-end AI audio via AudioStack — automate high-quality speech, mixing, and mastering via AI.

## Description
Connect your **AudioStack** account to any AI agent and build a complete AI-driven audio production studio through natural conversation.

### What you can do

- **Professional Speech** — Generate high-quality speech using a library of over 700 synthetic voices in dozens of languages
- **Audioforms** — Create complex audio productions (voice, music, and effects) using a single JSON descriptive structure
- **Automated Mastering** — Apply professional-grade mixing and mastering to your audio files automatically
- **Asset Management** — Search for voices, manage sound templates, and organize your media library directly

### How it works

1. Subscribe to this server
2. Enter your AudioStack API Key
3. Start producing professional audio from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — instantly turn scripts into high-quality audio with background music and professional mastering
- **Ad Agencies** — automate the production of localized audio ads across multiple languages and voices
- **Developers** — integrate professional audio generation into your applications using natural language commands


## Available Tools (10)
- **list_media_files**: List your uploaded and generated media files
- **list_voices**: You can filter by language, gender, or provider.

List and search for available AI voices
- **text_to_speech**: Generate speech from text using an AI voice
- **create_audioform**: Create a fully mixed audio production (Audioform)
- **create_mix**: Automate mixing and mastering of audio tracks
- **create_story**: Create a long-form audio story
- **get_audioform**: Get the status and final URL of an Audioform
- **get_usage_analytics**: Get account usage metrics
- **get_voice_details**: Get detailed information for a specific voice
- **list_sound_templates**: List available music and sound design templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AudioStack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for professional male voices in Portuguese."

**🤖 AI Agent:**
> I've searched the library. I found several matches, including 'v123' (Deep, Professional) and 'v456' (Friendly, Energetic). Would you like to hear a sample or use one for your script?

---

**👤 You:**
> "Convert this text to speech using voice 'v123': 'Hello, welcome to our AI audio studio.'"

**🤖 AI Agent:**
> Generating speech... Done! You can access the audio file at the following URL. Would you like me to apply background music to this recording?

---

**👤 You:**
> "Show me all sound templates related to 'Electronic Music'."

**🤖 AI Agent:**
> I found 3 templates: 'Techno Pulse', 'Ambient Synth', and 'House Groove'. Each includes pre-mixed background tracks optimized for professional mastering.


## ❓ FAQ

**Q: Can the AI help me choose the best voice for my content?**
Yes! You can ask the agent to search for voices based on gender, language, or style (e.g., 'professional male Portuguese voice'). It will return a list of matching IDs and descriptions for you to choose from.

**Q: What is an Audioform and how does the AI use it?**
An Audioform is a JSON blueprint for a full production. Your AI agent uses it to define exactly which voice to use, what background music to add, and how the final mastering should sound in a single automated step.

**Q: Is there a limit to the length of audio I can generate?**
The integration supports standard API limits from AudioStack. For very long scripts, it is recommended to generate them in sections or chapters for optimal quality and processing speed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/audiostack](https://vinkius.com/mcp/audiostack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AudioStack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `audiostack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AudioStack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "audiostack": {
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
