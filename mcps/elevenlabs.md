# ElevenLabs MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elevenlabs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Generate high-quality AI speech via ElevenLabs — use lifelike voices, manage text-to-speech, track usage, and handle audio dubbing directly from any AI agent.

## Description
Connect your **ElevenLabs** account to any AI agent and take full control of your AI audio generation and lifelike speech synthesis through natural conversation.

### What you can do

- **Speech Synthesis Orchestration** — Extract explicit REST maps utilizing text-to-speech endpoints to fire heavy inference pipelines streaming perfect conversational intonation blocks
- **Voice Library Navigation** — Identify bounded records inside the ElevenLabs platform and pull globally curated standard and cloned voice libraries natively
- **Voice Tuning** — Perform structural extraction of properties driving human likeness, dissecting precisely Stability and Similarity bounds for active account logic
- **Audio Dubbing** — Initiate massive video and audio translation queues injecting cross-lingual voice models to automate multi-language content production
- **Generation Auditing** — Enumerate explicitly attached structured rules exporting active history and mapping literal historic generations across time limits
- **Quota Oversight** — Validate API logic querying strict character quotas and subscription limits to monitor character consumption and block system overruns
- **Vault Security** — Identify precise active arrays spanning native gateway auth to retrieve explicit cloud generation logs and manage generated blobs securely

### How it works

1. Subscribe to this server
2. Enter your ElevenLabs API Key (found in My Workspace > API Keys)
3. Start generating lifelike AI speech from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — generate high-quality voiceovers and dub videos into multiple languages using natural language
- **Developers** — test and debug text-to-speech integrations and verify voice settings through natural conversation
- **Marketers** — create localized audio content and monitor character usage across different campaigns in real-time
- **AI Researchers** — explore different voice models and stability settings directly from the chat interface


## Available Tools (10)
- **get_voice**: Get voice details
- **text_to_speech**: Returns audio metadata. Supports 29+ languages.

Convert text to speech audio
- **list_models**: List AI speech models
- **list_history**: List generation history
- **get_history_item**: Get history item details
- **get_user_info**: Get user profile info
- **get_subscription**: Get subscription details
- **list_projects**: List dubbing/voice projects
- **list_voices**: List all available voices
- **list_pronunciation_dictionaries**: List pronunciation dictionaries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ElevenLabs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate audio for: 'Hello, this is a lifelike AI voice.' using voice 'abc-123'"

**🤖 AI Agent:**
> Inference pipeline triggered! I've sent your script to ElevenLabs using voice 'abc-123'. The audio is being generated with perfect intonation. Would you like to check the history for the download link?

---

**👤 You:**
> "Show me my remaining character quota"

**🤖 AI Agent:**
> Retrieving subscription info... You have used 15,000 characters out of your 100,000 monthly limit. You have 85,000 characters remaining for this billing cycle.

---

**👤 You:**
> "Dub this video into Spanish: https://example.com/video.mp4"

**🤖 AI Agent:**
> Dubbing job initiated! I've started the translation queue for your video into Spanish. I'll provide the tracking ID (dub_abc) so you can monitor the rendering status.


## ❓ FAQ

**Q: Can my agent generate speech using a specific voice ID?**
Yes. Use the 'text_to_speech' tool. Provide the 'voice_id' and the text script. The agent will fire the inference pipeline and return the generated audio content natively.

**Q: How do I monitor my character quota via chat?**
Use the 'get_subscription' tool. Your agent will validate the API logic querying your character usage (e.g., 100k limits) and subscription status to prevent system overruns.

**Q: Can I translate a video using the dubbing tool through the agent?**
Absolutely. Use the 'create_dubbing' tool. Provide a JSON payload with the 'source_url' and 'target_lang'. The agent will initiate the massive video translation queue and track the rendering job for you.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elevenlabs](https://vinkius.com/mcp/elevenlabs)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `elevenlabs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ElevenLabs** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "elevenlabs": {
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
