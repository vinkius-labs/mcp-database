# Lovo AI (Genny TTS & Voice Synthesis API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lovo-ai-genny-tts-voice-synthesis-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate high-quality AI voices and text-to-speech synthesis directly from your AI agent using Lovo AI's Genny API.

## Description
Connect **Lovo AI (Genny)** to your AI agent to transform text into lifelike speech. This server allows you to browse hundreds of premium voices and manage speech synthesis jobs through natural conversation.

### What you can do

- **Voice Discovery** — Use `list_voices` to browse all available AI speakers, filtering by language, gender, and style.
- **Speaker Details** — Use `get_speaker` to retrieve deep metadata for a specific voice ID to ensure the perfect tone for your content.
- **Speech Synthesis** — Use `create_tts_job` to convert text into audio with granular control over speed and emotional styles (e.g., cheerful, sad, professional).
- **Job Monitoring** — Use `get_tts_job` to track the status of your audio generation and retrieve the final output URLs once ready.

### How it works

1. Subscribe to this server
2. Enter your Lovo Genny API Key
3. Start generating professional voiceovers from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Generate narrations for videos or podcasts directly from your script-writing interface.
- **Developers** — Integrate high-fidelity voice synthesis into applications without leaving the code editor.
- **Marketers** — Quickly produce localized audio versions of ad copy and social media content.


## Available Tools (4)
- **list_voices**: List all available voices
- **create_tts_job**: Submit a text-to-speech synthesis job
- **get_tts_job**: Check the status of a previously submitted TTS job
- **get_speaker**: Get detailed information about a specific speaker


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lovo AI (Genny TTS & Voice Synthesis API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available English voices in Lovo AI."

**🤖 AI Agent:**
> I've retrieved the list of voices. You have access to speakers like 'Sophia' (ID: 632...), 'Mateo' (ID: 634...), and many others. Would you like to filter them by style or gender?

---

**👤 You:**
> "Create a TTS job for the text 'Welcome to the future of AI' using speaker ID 632c... with a cheerful style."

**🤖 AI Agent:**
> The TTS job has been submitted successfully. The Job ID is 'job_789abc'. I will monitor the status for you. Would you like me to check if it's finished now?

---

**👤 You:**
> "Check the status and get the audio link for job ID job_789abc."

**🤖 AI Agent:**
> The job 'job_789abc' is now complete! You can access your audio file here: [Audio URL]. The synthesis used the 'cheerful' style as requested.


## ❓ FAQ

**Q: How can I find the right voice ID for my project?**
Use the `list_voices` tool. It returns a comprehensive list of speakers including their IDs, names, and supported styles. You can then use `get_speaker` with a specific ID to see more detailed information.

**Q: Can I adjust the emotion or speed of the generated voice?**
Yes! When using `create_tts_job`, you can provide an optional `speed` (number) and `style` (e.g., 'cheerful', 'sad', 'normal') to customize the output to your needs.

**Q: How do I get the final audio file once the job is submitted?**
After creating a job, use the `get_tts_job` tool with the returned Job ID. Once the status is 'completed', the response will include the URLs to download your synthesized audio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lovo-ai-genny-tts-voice-synthesis-api](https://vinkius.com/mcp/lovo-ai-genny-tts-voice-synthesis-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lovo AI (Genny TTS & Voice Synthesis API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lovo-ai-genny-tts-voice-synthesis-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lovo AI (Genny TTS & Voice Synthesis API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lovo-ai-genny-tts-voice-synthesis-api": {
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
