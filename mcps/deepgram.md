# Deepgram MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deepgram)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Power audio AI via Deepgram — perform high-speed speech-to-text, generate lifelike text-to-speech, track usage, and manage API keys directly from any AI agent.

## Description
Connect your **Deepgram** account to any AI agent and take full control of your speech-to-text (STT) and text-to-speech (TTS) workflows through natural conversation.

### What you can do

- **Speech-to-Text (STT)** — Dispatch automated transcription requests for remote audio URLs using the lightning-fast Nova-2 model to consume explicit WAV/MP3 web streams
- **Text-to-Speech (TTS)** — Generate high-fidelity audio from raw text using Aura voices, outputting the exact binary stream footprint natively from your chat
- **Usage Monitoring** — Analyze specific global bounds hitting `/usage` to map literally terabytes of exact API transcription times and TTS byte usage
- **Project & Key Management** — List and create ephemeral Deepgram access boundaries (API keys) and isolate organizational tenants where Audio AI billing is enforced
- **Wallet Oversight** — Retrieve explicit cloud logging tracing explicit Vault limits and verify direct wallet thresholds to ensure pipelines never drop
- **Identity & Invites** — Manage developer limits by listing members and sending team invites to specific project UUIDs strictly

### How it works

1. Subscribe to this server
2. Enter your Deepgram API Key (found in the Deepgram Console under Settings > API Keys)
3. Start managing your audio AI workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — test STT/TTS models and manage API keys without leaving the development environment
- **Product Teams** — monitor audio AI usage and verify transcription accuracy in real-time
- **Data Engineers** — audit transcription volumes and manage project-wide audio pipelines using natural language
- **Ops Teams** — track wallet balances and manage team access across multiple Deepgram projects


## Available Tools
- **send_invite**: Invite a team member to a project
- **list_keys**: List API keys for a project
- **get_balances**: Get credit balances for a project
- **create_key**: Payload should include comment, scopes, and optional expiration.

Create a new API key for a project
- **delete_key**: Revoke and delete an API key
- **list_members**: List team members in a project
- **list_projects**: List all Deepgram projects in your account
- **transcribe_url**: Supports WAV, MP3, FLAC, and other formats.

Transcribe audio from a URL using Deepgram Nova-2
- **speak_text**: Returns metadata about the generated audio.

Convert text to speech using Deepgram Aura voices
- **get_usage**: Use query_string for date filters (e.g. "start=2026-01-01&end=2026-06-01").

Get API usage statistics for a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deepgram** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Transcribe this audio: https://example.com/recording.mp3 using nova-2"

**🤖 AI Agent:**
> Transcription complete! Using the Nova-2 model, I've processed the audio stream. Here is the text: 'Welcome to the deep dive into AI orchestration...'. I can also provide the confidence scores for each word.

---

**👤 You:**
> "Generate speech for: 'The future of AI is agentic' using aura-asteria-en"

**🤖 AI Agent:**
> Audio stream generated! I've synthesized the text using the Aura Asteria voice. You can download or play the resulting MP3 binary data. The sound is high-fidelity and naturally paced.

---

**👤 You:**
> "Show me my Deepgram usage for this month"

**🤖 AI Agent:**
> Retrieving usage data... You have transcribed 450 minutes of audio and generated 12MB of TTS content this month. Your project limits are well within the current thresholds.


## ❓ FAQ

**Q: Can my agent transcribe an audio file from a public URL?**
Yes. Use the 'transcribe_url' tool. Provide the public URL of the audio file (WAV, MP3, etc.) and specify the model (e.g., 'nova-2'). The agent will dispatch the request to Deepgram and return the transcribed text instantly.

**Q: How do I generate speech from text using the agent?**
Use the 'speak_text' tool. Provide the text script and the target voice model (e.g., 'aura-asteria-en'). Your agent will trigger the high-fidelity Aura voice engine and return the binary audio stream data.

**Q: Can I monitor my remaining project balance via chat?**
Absolutely. Use the 'get_balances' tool with your project ID. The agent will retrieve your current wallet thresholds and funding limits directly from Deepgram to ensure your audio pipelines stay active.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deepgram](https://vinkius.com/mcp/deepgram)
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
3. Set Type to "SSE", enter `deepgram` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deepgram** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deepgram": {
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
