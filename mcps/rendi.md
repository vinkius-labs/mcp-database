# Rendi MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rendi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rendi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rendi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Process and transform images with an API that resizes, crops, converts formats, and applies filters for web and mobile applications.

## Description
Connect your **Rendi** account to any AI agent and take full control of your cloud-based media processing and FFmpeg orchestration through natural conversation. Rendi provides a serverless platform for executing professional video and audio commands, allowing you to convert formats, generate thumbnails, and probe media metadata directly from your chat interface.

### What you can do

- **FFmpeg Command Orchestration** — Run any standard FFmpeg command in the cloud programmatically without managing server infrastructure.
- **Media Format Intelligence** — Convert videos to audio, generate GIFs, and create thumbnails directly from the AI interface using simple natural language.
- **Chained Workflow Control** — Execute multiple media commands in a single request to automate complex processing pipelines.
- **FFprobe & Metadata Analysis** — Analyze media files and retrieve technical metadata to ensure your assets meet professional standards.
- **Operational Monitoring** — Track system activity and manage temporary cloud storage files using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Rendi API Key from your dashboard settings
3. Start processing media files from Claude, Cursor, or any MCP-compatible client

No more manual terminal work or cloud worker configuration. Your AI acts as a dedicated media engineer or technical content coordinator.

### Who is this for?

- **Content Engineers & Developers** — quickly test FFmpeg parameters and monitor processing results without writing boilerplate code.
- **Video Producers** — automate the generation of previews and technical analysis via natural conversation.
- **Operations Teams** — streamline the retrieval of media metadata and monitor processing health directly within the chat.


## Available Tools
- **convert_video_to_audio**: Quickly convert a video to audio
- **delete_file**: Delete a file from Rendi storage
- **ffprobe**: Analyze a media file using ffprobe
- **generate_thumbnail**: Generate a thumbnail from a video
- **get_command_status**: Once completed, it provides the storage URL for output files.

Get status of an FFmpeg command
- **get_file_details**: Get details for a stored file
- **get_file_info**: Get metadata and details for a specific file
- **list_commands**: List all submitted FFmpeg commands
- **list_files**: List all files in Rendi storage
- **run_chained_ffmpeg_commands**: Run multiple chained FFmpeg commands
- **run_ffmpeg_command**: Returns a command ID to poll for status.

Run a single FFmpeg command in the cloud


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rendi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this media file for technical metadata: https://example.com/video.mp4"

**🤖 AI Agent:**
> Running ffprobe analysis... I've retrieved the metadata. The video has a resolution of 1920x1080 at 30fps using the H.264 codec. Would you like me to check the audio stream details?

---

**👤 You:**
> "Convert this MP4 video to WebM format with H265 encoding and reduce the file size by 50%."

**🤖 AI Agent:**
> FFmpeg conversion completed. Input: video.mp4 (1080p, H264, 245 MB, 12:34 duration). Output: video.webm (1080p, VP9/H265, 118 MB, 51.8% size reduction). Encoding settings: CRF 28, 2-pass encoding, libvpx-vp9 codec. Quality assessment: SSIM 0.96 (excellent visual fidelity). Processing time: 4 minutes 23 seconds. The output file maintains original audio quality (AAC 128kbps converted to Opus 128kbps). Download ready.

---

**👤 You:**
> "Analyze the media properties of the uploaded video file and show me all codec and stream details."

**🤖 AI Agent:**
> FFprobe analysis complete. File: presentation.mp4. Container: MPEG-4 Part 14. Duration: 45:12. Size: 1.2 GB. Video stream: H.264 (High Profile), 1920x1080, 30fps, 3.2 Mbps bitrate, YUV420p color space. Audio stream 1: AAC LC, 48kHz, stereo, 192 kbps. Audio stream 2: AAC LC, 48kHz, 5.1 surround, 384 kbps. Subtitle stream: SRT (English). Metadata: creation date May 10, 2025, encoder: HandBrake 1.7.3.


## Installation & Usage

To install and use the **Rendi** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rendi](https://vinkius.com/mcp/rendi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
