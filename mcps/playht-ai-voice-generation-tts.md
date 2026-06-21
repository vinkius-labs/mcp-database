# Play.ht (AI Voice Generation & TTS) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/playht-ai-voice-generation-tts)
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


## Available Tools (3)
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


## ❓ FAQ

**Q: How can I find the right voice ID for my language?**
Use the `get_voices` tool. It returns a complete list of available voices, allowing you to filter by name, language, and gender to find the perfect match for your project.

**Q: Can I control the speed and format of the generated audio?**
Yes! When using `convert_tts`, you can specify the `speed` (from 0.5 to 2.0), the `output_format` (like mp3 or wav), and the `quality` level to suit your needs.

**Q: What should I do if a conversion takes a long time?**
For longer texts, use the `get_tts_status` tool with your `transcription_id`. This allows you to check if the audio is still processing or ready for download.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/playht-ai-voice-generation-tts](https://vinkius.com/mcp/playht-ai-voice-generation-tts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Play.ht (AI Voice Generation & TTS)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `playht-ai-voice-generation-tts` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Play.ht (AI Voice Generation & TTS)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "playht-ai-voice-generation-tts": {
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
