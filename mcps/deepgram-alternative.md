# Deepgram MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deepgram-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Transcribe speech to text with blazing speed and accuracy using neural networks trained on real-world audio at scale.

## Description
Connect your **Deepgram** account to any AI agent and take full control of your speech-to-text (STT) and text-to-speech (TTS) workflows through natural conversation.

### What you can do

- **Transcription Orchestration** — Convert speech from public audio or video URLs into high-fidelity text programmatically using the latest Nova-3 models with smart formatting and diarization
- **Neural Speech Synthesis** — Programmatically generate natural-sounding audio from text input using the high-speed Aura engine to coordinate voice-enabled interfaces
- **Model Discovery** — Access complete directories of high-performance STT and TTS models supported by Deepgram to ensure the perfect accuracy and latency for your content
- **Project & Usage Monitoring** — Programmatically track your API utilization, minute consumption, and request counts across multiple projects for instant operational reporting
- **Credential Lifecycle** — Retrieve identifiers for active API keys associated with your projects directly through your agent to maintain high-fidelity security oversight

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the Deepgram Console
3. Start transcribing and synthesizing audio from Claude, Cursor, or any MCP client

No more manual file uploading or complex latency tuning in the portal. Your AI acts as your dedicated audio engineer and media production coordinator.

### Who is this for?

- **Developers & Engineers** — instantly transcribe recorded meetings and integrate high-speed TTS into applications using natural language commands
- **Content Creators** — automate the generation of voiceovers and subtitles for global video assets without leaving your workspace
- **Research Teams** — scale the processing of interview recordings and monitor usage limits through simple AI queries


## Available Tools (6)
- **list_available_models**: List high-performance AI models
- **get_project_usage**: Check API usage and limits
- **list_api_keys**: List active API keys
- **list_deepgram_projects**: List your Deepgram projects
- **convert_text_to_speech**: Generate audio from text (TTS)
- **transcribe_audio_url**: Transcribe an audio file via URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deepgram** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Transcribe the audio from this URL: 'https://static.deepgram.com/examples/interview_segments_nuwav.wav'."

**🤖 AI Agent:**
> Transcription triggered! I'm converting the speech from your URL into high-fidelity text using Nova-3. I'll provide the formatted transcript and speaker diarization details shortly.

---

**👤 You:**
> "Convert this text to speech: 'Deepgram is the fastest way to add voice to your AI'."

**🤖 AI Agent:**
> Audio synthesis complete! I've rendered your text into natural-sounding speech using the Aura engine. You can now access the media file and metadata for playback.

---

**👤 You:**
> "List all active API keys for project 'proj_123'."

**🤖 AI Agent:**
> I've retrieved the identifiers for your active API keys in project proj_123. There are 2 keys currently authorized for transcription and synthesis. Shall I check the usage stats for this project?


## ❓ FAQ

**Q: How do I get a Deepgram API Key?**
Log in to the Deepgram Console, navigate to the **API Keys** section, and create a new key with the necessary permissions.

**Q: What is the Nova-3 model?**
Nova-3 is Deepgram's latest state-of-the-art transcription model, offering unmatched speed and accuracy for real-world audio.

**Q: Can I synthesize speech in different voices?**
Yes! The `convert_text_to_speech` tool allows you to specify models like `aura-asteria-en` or `aura-orion-en` for different vocal profiles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deepgram-alternative](https://vinkius.com/mcp/deepgram-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deepgram** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deepgram-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deepgram** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deepgram-alternative": {
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
