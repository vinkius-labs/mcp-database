# CAMB.AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cambai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Translate and dub audio content into dozens of languages using AI voices that sound natural and preserve speaker identity.

## Description
Connect your **CAMB.AI** account to any AI agent and take full control of your high-fidelity audio localization and voice generation workflows through natural conversation.

### What you can do

- **Text-to-Speech (TTS) Orchestration** — Generate high-fidelity speech from text using MARS-8 models with ultra-low latency programmatically through your agent
- **Professional Dubbing & Translation** — Programmatically translate and dub video or audio files into 140+ languages while preserving original emotional nuances
- **Voice Cloning Architecture** — Create custom digital twins of any voice from short samples and retrieve your directory of custom cloned voices in real-time
- **Global Communication Intelligence** — Access comprehensive directories of source and target languages to perfectly coordinate cross-border content delivery
- **Operational Monitoring** — Track the real-time status of generation jobs and retrieve high-fidelity results directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the CAMB.AI Studio dashboard (Settings or API tab)
3. Start localizing your multimedia content from Claude, Cursor, or any MCP client

No more manual toggling between translation portals or waiting on slow dubbing pipelines. Your AI acts as your dedicated audio engineer and localization coordinator.

### Who is this for?

- **Content Creators** — instantly translate videos and generate voiceovers using natural language commands
- **Developers** — integrate real-time low-latency voice responses into custom applications without leaving your workspace
- **Marketing Teams** — automate the scale of personalized audio messages across 140+ languages through simple AI queries


## Available Tools (10)
- **create_dubbing**: Create a dubbing or translation job
- **create_tts**: Returns a task ID to track progress.

Create a Text-to-Speech task
- **create_voice_clone**: Create a custom voice clone
- **get_job_status**: Check the status of a dubbing job
- **get_tts_result**: Get the result of a completed TTS task
- **get_tts_status**: Check the status of a TTS task
- **list_cloned_voices**: List all custom cloned voices
- **list_source_languages**: List supported source languages
- **list_target_languages**: List supported target languages
- **list_voices**: List all available voices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CAMB.AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available voices for Text-to-Speech in CAMB.AI."

**🤖 AI Agent:**
> I've retrieved the voice directory. You have access to 15 public voices and 3 custom clones, including 'Davy' (ID: 1) and 'Sarah'. Which one would you like to use for generation?

---

**👤 You:**
> "Generate speech for 'Hello world' using voice ID 1 and language 'en-us'."

**🤖 AI Agent:**
> TTS task initiated! I've started the generation for 'Hello world' (Task ID: tts_789). I'll monitor the status and alert you as soon as the audio file is ready for download.

---

**👤 You:**
> "Dub video 'https://vinkius.com/promo.mp4' from English (ID: 1) to French (ID: 4)."

**🤖 AI Agent:**
> Dubbing job triggered! Video localization for 'promo.mp4' is now in progress (Job ID: dub_456). I'll track the translation nuances and notify you when the final high-fidelity file is ready.


## ❓ FAQ

**Q: How do I find my CAMB.AI API Key?**
Log in to your account, navigate to the **Studio dashboard**, and go to the **Settings** or **API** tab to generate a new key.

**Q: Can I use my own voice via AI?**
Yes! Use the `create_voice_clone` tool to upload a sample audio file. Once processed, you can use the resulting ID to generate speech with your voice.

**Q: How do I track a dubbing task?**
Use the `get_job_status` tool and provide the job ID. Your agent will return the high-fidelity progress percentage and final results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cambai](https://vinkius.com/mcp/cambai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CAMB.AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cambai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CAMB.AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cambai": {
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
