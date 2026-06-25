# ElevenLabs MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elevenlabs-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Generate lifelike speech from text with neural voice synthesis that clones voices and supports dozens of languages naturally.

## Description
Connect your **ElevenLabs** account to any AI agent and take full control of your neural audio synthesis and voice management workflows through natural conversation.

### What you can do

- **Speech Orchestration** — Convert text to high-fidelity audio programmatically using the world's most advanced lifelike AI voices
- **Voice Intelligence** — Access your complete voice library, including standard, community, and custom cloned voices to maintain high-fidelity branding
- **History Tracking** — Programmatically retrieve and manage your audio generation history, including direct download links for all past creations
- **Model Selection** — Explore and select from multiple neural audio models (including Multilingual v2) to ensure the perfect tone and stability for your content
- **Administrative Visibility** — Monitor your character usage, subscription limits, and account metadata directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your ElevenLabs profile (Profile > API Key)
3. Start generating high-quality AI audio from Claude, Cursor, or any MCP client

No more manual copy-pasting into the web editor or complex history searching. Your AI acts as your dedicated neural audio producer.

### Who is this for?

- **Content Creators** — instantly generate voiceovers for videos and social media using natural language commands
- **Developers** — integrate high-fidelity text-to-speech and voice cloning into applications through simple AI actions
- **Marketing Teams** — automate the creation of personalized audio messages and track credit utilization without leaving your workspace


## Available Tools (12)
- **delete_voice**: Delete a cloned voice
- **get_download_link**: Get audio download URL
- **get_account_info**: Get user profile
- **get_history_item**: Get history item details
- **get_subscription_info**: Get usage and plan info
- **get_voice_settings**: Get voice fine-tuning
- **get_voice**: Get voice details
- **list_audio_history**: List generated audio logs
- **list_models**: List AI audio models
- **list_voices**: List all available voices
- **text_to_speech**: Convert text to audio
- **delete_history_item**: Delete audio record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ElevenLabs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert this text to speech using 'Bella' voice: 'Welcome to the world of neural audio'."

**🤖 AI Agent:**
> Audio generation triggered! I've converted your text using the 'Bella' voice (ID: EXAV...vXU). You can find the record in your history or I can retrieve the download link for you.

---

**👤 You:**
> "List all my available voices in ElevenLabs."

**🤖 AI Agent:**
> I've retrieved your voice library. You have access to 10 standard voices and 2 custom cloned voices ('CEO Voice' and 'Narrator'). Which one would you like to use?

---

**👤 You:**
> "Check my remaining character limits for this month."

**🤖 AI Agent:**
> Scanning subscription... You have 15,420 characters remaining out of your 30,000 monthly limit. Your next reset is in 12 days. Would you like to view your generation history?


## ❓ FAQ

**Q: How do I find my ElevenLabs API Key?**
Log in to your account, click your profile icon (bottom left), and navigate to the API Key section to generate or copy your token.

**Q: Which model should I use for multiple languages?**
The `eleven_multilingual_v2` model is recommended for high-quality speech generation in over 29 different languages.

**Q: Can I get a direct download link for a past generation?**
Yes! Use the `get_download_link` tool with a history item ID to retrieve a temporary URL for the audio file.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elevenlabs-alternative](https://vinkius.com/mcp/elevenlabs-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `elevenlabs-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ElevenLabs** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "elevenlabs-alternative": {
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
