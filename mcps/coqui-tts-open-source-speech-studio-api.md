# Coqui TTS (Open Source Speech Studio API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coqui-tts-open-source-speech-studio-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate high-quality speech from text using Coqui TTS. List available models and synthesize audio directly from your AI agent.

## Description
Connect your **Coqui TTS** server to any AI agent to enable advanced text-to-speech capabilities. This MCP server allows you to interact with your self-hosted or cloud-based Coqui Speech Studio API through natural conversation.

### What you can do

- **Model Discovery** — List all available text-to-speech models currently loaded on your Coqui server
- **Speech Synthesis** — Convert any text string into spoken audio instantly using the server's synthesis engine
- **Metadata Retrieval** — Get detailed information about generated audio files and model configurations

### How it works

1. Subscribe to this server
2. Enter your Coqui Server URL (e.g., your local or hosted API endpoint)
3. Start generating high-quality voices from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — integrate voice synthesis into applications without leaving the code editor
- **Content Creators** — quickly generate voiceovers or speech samples using open-source models
- **AI Researchers** — test and compare different TTS models directly through an agent interface


## Available Tools (2)
- **list_models**: List available TTS models
- **synthesize_speech**: Returns metadata about the generated audio file.

Synthesize speech from text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coqui TTS (Open Source Speech Studio API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available TTS models on my Coqui server."

**🤖 AI Agent:**
> I've retrieved the available models from your Coqui server. You have access to models like 'tts_models/en/ljspeech/vits' and 'tts_models/multilingual/multi-dataset/xtts_v2'. Which one would you like to use?

---

**👤 You:**
> "Synthesize the text 'Welcome to the future of open source AI' into speech."

**🤖 AI Agent:**
> I am generating the audio for that text now... Done! The speech has been synthesized successfully using your default Coqui model. You can find the audio metadata and file details here.

---

**👤 You:**
> "What models can I use for speech synthesis?"

**🤖 AI Agent:**
> Let me check your Coqui server... It currently reports 3 active models: a standard English model, a multilingual XTTS model, and a fast VITS model. Would you like to see the full technical IDs for these?


## ❓ FAQ

**Q: How can I check which voice models are currently installed on my server?**
You can use the `list_models` tool. Your agent will query the Coqui server and return a list of all available TTS models ready for synthesis.

**Q: Is it possible to generate audio files from a text string directly?**
Yes! Use the `synthesize_speech` tool by providing the text you want to convert. The agent will process it through Coqui and return the audio metadata.

**Q: What do I need to provide to connect my local Coqui instance?**
You only need to provide the `COQUI_SERVER_URL`. This is the base address where your Coqui Speech Studio API is reachable (e.g., http://localhost:5002).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coqui-tts-open-source-speech-studio-api](https://vinkius.com/mcp/coqui-tts-open-source-speech-studio-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coqui TTS (Open Source Speech Studio API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coqui-tts-open-source-speech-studio-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coqui TTS (Open Source Speech Studio API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coqui-tts-open-source-speech-studio-api": {
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
