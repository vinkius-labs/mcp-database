# Maestra MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/maestra)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Automate transcription, translation, and AI voiceovers via the Maestra.ai REST API.

## Description
Connect your **Maestra.ai** account to any AI agent to automate your media processing workflows. This MCP server enables your agent to upload audio/video files for transcription, translate transcripts into 125+ languages, and generate synthetic AI voiceovers directly from natural language interfaces.

### What you can do

- **Automated Transcription** — Upload media files via public URLs and receive accurate, speaker-aware transcripts instantly
- **Global Translation** — Translate existing transcriptions into over 125 different languages to reach a worldwide audience
- **AI Dubbing** — Generate high-quality synthetic voiceovers for your media using a wide range of available AI voices
- **Asset Management** — List all files in your account, monitor processing statuses, and organize content into folders
- **Result Export** — Generate temporary download links for results in formats like SRT, VTT, PDF, and JSON

### How it works

1. Subscribe to this server
2. Enter your Maestra.ai API Key
3. Start processing your media from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Quickly generate subtitles and translations for your videos via natural language commands
- **Developers** — Integrate automated media processing and dubbing logic into your custom applications
- **Localization Teams** — Automate the workflow of translating and re-voicing global media assets efficiently


## Available Tools (8)
- **export_transcription_results**: Get an export link for a processed file
- **list_maestra_files**: List all audio and video files in your Maestra account
- **list_account_folders**: List all folders in your account
- **get_file_details**: Get details and status for a specific file
- **translate_transcription**: Translate an existing transcription into a new language
- **upload_media_for_transcription**: Requires a public file URL and target source language.

Upload a new file for transcription
- **generate_ai_voiceover**: Generate a synthetic voiceover for a media file
- **list_available_ai_voices**: List all available synthetic AI voices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Maestra** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Upload the video at 'https://example.com/video.mp4' for English transcription in Maestra."

**🤖 AI Agent:**
> I've initiated the upload for your video. Maestra is now processing the file for English transcription. The file ID is 'vid-12345'.

---

**👤 You:**
> "List all available AI voices for French."

**🤖 AI Agent:**
> I found 8 synthetic voices for French, including 'Claire (Female)', 'Mathieu (Male)', and 'Amelie (Female)'. Which one would you like to use for your voiceover?

---

**👤 You:**
> "Get an SRT export link for file ID 'vid-12345'."

**🤖 AI Agent:**
> I've generated the export link for your subtitles. You can download the SRT file here: https://api.maestra.ai/temp/vid-12345.srt


## ❓ FAQ

**Q: How do I start a transcription for a public video?**
Use the `upload_media_for_transcription` tool and provide the public `file_url` along with the source language code (e.g., 'en' for English).

**Q: Can I choose which AI voice to use for dubbing?**
Yes, first use the `list_available_ai_voices` tool to find a voice ID that matches your target language and gender, then provide it to the `generate_ai_voiceover` tool.

**Q: What formats can I export my transcripts in?**
The `export_transcription_results` tool supports formats such as 'srt', 'vtt', 'txt', 'pdf', and 'json'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/maestra](https://vinkius.com/mcp/maestra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Maestra** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `maestra` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Maestra** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "maestra": {
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
