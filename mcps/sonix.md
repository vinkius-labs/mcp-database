# Sonix MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sonix)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sonix-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sonix-mcp)
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


## Available Tools
- **create_batch_summarization**: Create a batch summarization for a folder
- **create_folder**: Create a new folder
- **create_media_export**: Create a media export
- **create_share**: Share a media file with a user
- **create_summarization**: Create a summarization for a media file
- **create_translation**: Create a translation for a media file
- **create_video_burn_in**: Create a video burn-in (subtitles on video)
- **delete_media**: Delete a media file
- **delete_share**: Remove a share from a media file
- **get_batch_summarization**: Get batch summarization details
- **get_media_export**: Get media export status
- **get_media**: Get media status and details
- **get_summarization**: Get summarization details
- **get_transcript_json**: Get JSON transcript with word-level timestamps
- **get_transcript_srt**: Get SRT transcript file
- **get_transcript_text**: Get plain text transcript
- **get_transcript_vtt**: Get VTT transcript file
- **get_translation**: Get translation status
- **get_video_burn_in**: Get video burn-in status
- **invite_user**: Invite a new user to the account
- **list_folders**: List all folders
- **list_media**: List media files
- **list_shares**: List shares for a media file
- **list_users**: List all users in the account
- **split_transcript**: Automatically split transcript into subtitles
- **submit_media**: Submit new media for transcription
- **update_folder**: Update a folder
- **update_media**: Update media attributes
- **update_transcript**: Update transcript words and speakers
- **update_user**: Update a user role


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


## Installation & Usage

To install and use the **Sonix** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sonix](https://vinkius.com/mcp/sonix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
