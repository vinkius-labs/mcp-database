# Play.ht (Voice Cloning) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/playht-voice-cloning)
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


## Available Tools (2)
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


## ❓ FAQ

**Q: How can I generate audio from text using a specific voice?**
Use the `generate_tts_stream` tool. Provide the text and the unique voice ID. You can also customize the `voice_engine` (like Play3.0-mini) and `emotion` for better results.

**Q: Can I create a new voice clone with this server?**
Yes! Use the `create_instant_voice_clone` tool. You'll need to provide a name for the voice and a base64 encoded audio sample of the voice you want to clone.

**Q: What audio formats are supported for generation?**
When using `generate_tts_stream`, you can specify the `output_format` as mp3, wav, ogg, flac, or mulaw.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/playht-voice-cloning](https://vinkius.com/mcp/playht-voice-cloning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Play.ht (Voice Cloning)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `playht-voice-cloning` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Play.ht (Voice Cloning)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "playht-voice-cloning": {
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
