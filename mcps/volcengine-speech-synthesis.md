# Volcengine Speech Synthesis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/volcengine-speech-synthesis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

The massive 'TikTok Voice' TTS API — generate natural speech with ByteDance's iconic voice models.

## Description
Connect **Volcengine Speech Synthesis** (ByteDance's TTS platform) to any AI agent and generate stunning natural speech — including the iconic TikTok voices — through natural conversation.

### What you can do
- **Text-to-Speech** — Convert any text to natural-sounding speech
- **TikTok Voices** — Use the exact voice models behind TikTok's viral TTS effects
- **Multi-Language** — Synthesize in Chinese, English, Japanese, and more
- **SSML Support** — Fine-grained control with pauses, emphasis, and prosody
- **Long-Form Audio** — Synthesize articles, audiobooks, and lengthy documents
- **Custom Voices** — Train personalized voice models from audio samples
- **Speed/Volume Control** — Adjust speech rate and volume dynamically

### How it works
1. Subscribe to this server
2. Enter your Volcengine Access Key and Secret Key
3. Start generating speech from Claude, Cursor, or any MCP client

### Who is this for?
- **Content Creators** — Generate voiceovers for videos, reels, and TikToks
- **Accessibility Teams** — Add speech output to apps and websites
- **Audiobook Producers** — Convert long-form text to natural narration
- **Developers** — Integrate TikTok-quality TTS into applications


## Available Tools
- **get_audio_formats**: Use MP3 for web delivery, WAV for editing, OGG Opus for efficient streaming, or PCM for raw processing.

List supported audio output formats
- **list_voices**: Essential for choosing the right voice before synthesis. Includes the famous TikTok voice styles.

List all available TTS voice models
- **synthesize_long_text**: Ideal for articles, audiobooks, and lengthy documentation. Use this when your text exceeds the standard 1024 character limit.

Synthesize speech from long text (over 1024 characters)
- **synthesize_ssml**: Use SSML tags like <break>, <emphasis>, <prosody> for natural-sounding output with precise timing and intonation control.

Convert SSML (Speech Synthesis Markup Language) to speech
- **synthesize_speech**: Supports multiple languages (Chinese, English, Japanese), various voice styles (female, male, child, trendy, news), and adjustable speed/volume. Returns audio data or URL. Ideal for narration, accessibility, multi-language content, and the iconic TikTok voice effects.

Convert text to speech using Volcengine TTS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Volcengine Speech Synthesis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate speech with the TikTok trendy female voice: 'Welcome to my video!'"

**🤖 AI Agent:**
> 🔊 Speech synthesized successfully! Using BV033_streaming (TikTok Trendy Female). Audio generated in MP3 format at 24kHz.

---

**👤 You:**
> "List all available voices and show me English options."

**🤖 AI Agent:**
> 🎙️ Available voices: BV001 (Generic Female, zh), BV002 (Generic Male, zh), BV033 (TikTok Trendy Female, zh), BV113 (English Female, en), BV115 (English Male, en). English options: BV113 (Female), BV115 (Male).

---

**👤 You:**
> "Synthesize this article into speech: [long article text...]"

**🤖 AI Agent:**
> 📖 Long-text synthesis started! Article split into 5 chunks. Using BV001_streaming voice. Processing will take ~30 seconds for full narration.


## ❓ FAQ

**Q: What makes Volcengine TTS different from other TTS services?**
Volcengine powers the iconic TikTok TTS effects used in billions of videos. It offers industry-leading Chinese speech quality, trendy social media voices, and ByteDance's proprietary neural voice technology.

**Q: Which languages are supported?**
Chinese (Mandarin), English, Japanese, and more. Use language parameter: 'zh' for Chinese, 'en' for English, 'ja' for Japanese. Each language has multiple voice styles.

**Q: What's the max text length?**
Standard synthesis supports up to 1024 characters per request. For longer texts, use the synthesize_long_text tool which automatically handles chunking and combining results for articles and audiobooks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/volcengine-speech-synthesis](https://vinkius.com/mcp/volcengine-speech-synthesis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Volcengine Speech Synthesis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `volcengine-speech-synthesis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Volcengine Speech Synthesis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "volcengine-speech-synthesis": {
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
