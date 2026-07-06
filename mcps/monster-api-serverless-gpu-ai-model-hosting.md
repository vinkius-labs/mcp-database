# Monster API (Serverless GPU & AI Model Hosting) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/monster-api-serverless-gpu-ai-model-hosting)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Access powerful AI models for image generation, text-to-speech, and transcription via serverless GPU infrastructure.

## Description
Connect to **Monster API** to leverage high-performance AI models without managing infrastructure. This MCP server allows your AI agent to generate visuals, audio, and transcriptions using top-tier models like SDXL, Sunno Bark, and Whisper.

### What you can do

- **Image Generation** — Create high-quality images using SDXL with custom aspect ratios and sampling steps.
- **Image-to-Image** — Modify existing images by providing a starting image and a text prompt to guide the transformation.
- **Speech Synthesis** — Convert text into natural-sounding audio using Sunno Bark for voiceovers and narration.
- **Audio Transcription** — Transcribe or translate audio files into text, SRT, or VTT formats using Whisper.
- **Job Management** — Track the progress of asynchronous AI tasks and retrieve results once processing is complete.

### How it works

1. Subscribe to this server
2. Enter your Monster API Key
3. Start generating AI assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Integrate state-of-the-art AI generation into your apps without managing GPUs or complex deployments.
- **Content Creators** — Generate unique images and voiceovers directly within your workspace using natural language.
- **Product Teams** — Rapidly prototype AI-powered features like automated transcription or image editing.


## Available Tools (5)
- **generate_sunno_bark**: Returns a process_id to poll for status.

Convert text into natural-sounding speech (TTS)
- **generate_whisper**: Returns a process_id to poll for status.

Transcribe audio to text using Whisper
- **get_job_status**: Once status is COMPLETED, the response contains the output URL.

Check the status of an asynchronous generation job
- **generate_image_to_image**: Returns a process_id to poll for status.

Modify an existing image based on a prompt
- **generate_sdxl**: Returns a process_id to poll for status.

Generate an image from text using SDXL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Monster API (Serverless GPU & AI Model Hosting)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a high-quality image of a cyberpunk city at night using SDXL in landscape mode."

**🤖 AI Agent:**
> I've submitted the SDXL generation job. Your process ID is `abc-123`. I'll poll the status for you to retrieve the image URL.

---

**👤 You:**
> "Transcribe this audio file into SRT format: https://example.com/audio.mp3"

**🤖 AI Agent:**
> Whisper transcription job started. Process ID: `trans-789`. I will let you know when the SRT file is ready.

---

**👤 You:**
> "Check the status of my generation job with process ID 'job-xyz-456'."

**🤖 AI Agent:**
> The job `job-xyz-456` is COMPLETED. You can access your generated asset here: [URL]


## ❓ FAQ

**Q: How do I get the final result of an image generation job?**
Since generation is asynchronous, the tool returns a `process_id`. You must use the `get_job_status` tool with that ID to check if the status is 'COMPLETED' and retrieve the output URL.

**Q: Can I specify the dimensions of the generated images?**
Yes, when using `generate_sdxl`, you can provide an `aspect_ratio` parameter such as 'square', 'landscape', or 'portrait' to control the output shape.

**Q: What transcription formats does the Whisper tool support?**
The `generate_whisper` tool allows you to choose between 'text', 'srt', and 'vtt' formats via the `transcription_format` parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/monster-api-serverless-gpu-ai-model-hosting](https://vinkius.com/mcp/monster-api-serverless-gpu-ai-model-hosting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Monster API (Serverless GPU & AI Model Hosting)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `monster-api-serverless-gpu-ai-model-hosting` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Monster API (Serverless GPU & AI Model Hosting)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "monster-api-serverless-gpu-ai-model-hosting": {
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
