# Maestra MCP Server

Automate transcription, translation, and AI voiceovers via the Maestra.ai REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/maestra)

## Overview
**Category:** artificial-intelligence
**Tools Count:** 8

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


## Available Tools
- **export_transcription_results**: Get an export link for a processed file
- **list_maestra_files**: List all audio and video files in your Maestra account
- **list_account_folders**: List all folders in your account
- **get_file_details**: Get details and status for a specific file
- **translate_transcription**: Translate an existing transcription into a new language
- **upload_media_for_transcription**: Requires a public file URL and target source language.

Upload a new file for transcription
- **generate_ai_voiceover**: Generate a synthetic voiceover for a media file
- **list_available_ai_voices**: List all available synthetic AI voices


## Installation & Usage

To install and use the **Maestra** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/maestra](https://vinkius.com/mcp/maestra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
