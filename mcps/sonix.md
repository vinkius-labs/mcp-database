# Sonix MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sonix)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Automate transcription, translation, and media management via Sonix — transcribe audio/video, generate subtitles, and create AI summaries directly from any AI agent.

## Description
Connect your **Sonix** account to any AI agent to streamline your media post-production and accessibility workflows through natural conversation.

### What you can do

- **Transcription & Subtitles** — Generate plain text, SRT, VTT, or JSON transcripts from audio and video files with full control over speaker labels and timestamps.
- **Media Management** — List, upload, update, and organize your media library into folders directly from your workspace.
- **AI Summarization** — Create concise summaries for individual files or process multiple recordings at once using batch summarization tools.
- **Translation** — Automatically translate your transcripts into dozens of languages to reach a global audience.
- **Video Burn-in** — Initiate video burn-in processes for subtitles to create ready-to-share social media content.
- **Collaboration** — Manage team access by listing users, inviting new members, and creating secure share links for your media.

### How it works

1. Subscribe to this server
2. Enter your Sonix API Key
3. Start processing media from Claude, Cursor, or any MCP-compatible client

No more manual uploading and waiting in browser tabs. Your AI acts as a media assistant, handling the heavy lifting of transcription and organization.

### Who is this for?

- **Content Creators** — instantly generate subtitles and summaries for YouTube, podcasts, or social media clips.
- **Researchers & Journalists** — quickly search through hours of interviews and extract text transcripts for analysis.
- **Product Teams** — summarize user feedback calls and share insights with the team via automated links.


## Available Tools (30)
- **create_batch_summarization**: Supply the folder ID and the summarization prompt.

Create a batch summarization for a folder
- **create_summarization**: Provide the media ID and optionally a custom prompt.

Create a summarization for a media file
- **create_video_burn_in**: Supply the media ID and required styling parameters.

Create a video burn-in (subtitles on video)
- **get_transcript_vtt**: Specify the media ID and desired formatting options.

Get VTT transcript file
- **list_users**: List all users in the account
- **split_transcript**: Provide the media ID and desired subtitle formatting parameters.

Automatically split transcript into subtitles
- **submit_media**: Provide the file URL and name. Do not submit media without a file URL.

Submit new media for transcription
- **create_media_export**: Provide the media ID and optionally remove strikethrough text.

Create a media export
- **create_translation**: Provide the media ID and target language code.

Create a translation for a media file
- **get_video_burn_in**: Provide the unique export ID to check the status.

Get video burn-in status
- **invite_user**: Requires both email and role.

Invite a new user to the account
- **list_folders**: List all folders
- **update_folder**: Provide the folder ID and the new name.

Update a folder
- **create_folder**: Specify the name and optional parent folder ID.

Create a new folder
- **create_share**: Requires the media ID and the recipient’s email address.

Share a media file with a user
- **delete_media**: the deletion.

Delete a media file
- **delete_share**: Must provide both media ID and target email.

Remove a share from a media file
- **get_batch_summarization**: Provide the batch ID.

Get batch summarization details
- **get_media_export**: Use the unique export ID to query the status.

Get media export status
- **get_media**: Use the specific media ID for the query.

Get media status and details
- **get_summarization**: Use the provided summarization ID.

Get summarization details
- **get_transcript_json**: Use the media ID to fetch word-level timestamps.

Get JSON transcript with word-level timestamps
- **get_transcript_srt**: Specify the media ID and desired formatting options.

Get SRT transcript file
- **get_transcript_text**: Provide the media ID to fetch the content.

Get plain text transcript
- **get_translation**: Supply the media ID and target language code.

Get translation status
- **list_media**: List media files
- **list_shares**: List shares for a media file
- **update_media**: Specify the media ID and at least one attribute to update.

Update media attributes
- **update_transcript**: Provide the media ID and the JSON array containing word/speaker updates.

Update transcript words and speakers
- **update_user**: Must provide both the user ID and the desired role.

Update a user role


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sonix** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my most recent media files in Sonix."

**🤖 AI Agent:**
> I've retrieved your media list. You have 5 recent files, including 'Interview_v1.mp4' (ID: m123) and 'Keynote_Speech.mp3' (ID: m456). Would you like to get the transcript for any of these?

---

**👤 You:**
> "Transcribe this audio file: https://example.com/audio.mp3 in French."

**🤖 AI Agent:**
> I've submitted the media for transcription. The Media ID is 'm789' and the status is currently 'processing'. I can notify you once the French transcript is ready.

---

**👤 You:**
> "Generate a summary for media ID m123."

**🤖 AI Agent:**
> I've initiated the summarization for 'Interview_v1.mp4'. You can check the result using `get_summarization` with ID 's999' in a few moments.


## ❓ FAQ

**Q: Can I download subtitles for my videos in SRT format?**
Yes! Use the `get_transcript_srt` tool with your Media ID. You can also customize options like `speaker_display` and `max_characters` per line.

**Q: How do I translate an existing transcript to another language?**
Simply use the `create_translation` tool. Provide the `media_id` and the target language code (e.g., 'es' for Spanish) to start the automated translation process.

**Q: Is it possible to summarize multiple media files at once?**
Yes, use the `create_batch_summarization` tool. It allows you to submit multiple media IDs to generate AI summaries for all of them in a single operation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sonix](https://vinkius.com/en/ai-agent-connect/sonix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sonix** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sonix` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sonix** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sonix": {
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
