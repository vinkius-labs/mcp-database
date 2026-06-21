# FileStack MCP Server

Upload, transform, and analyze files with Filestack—extract text via OCR, detect objects, and manage video transcoding directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/filestack)

## Overview
**Category:** image-video
**Tools Count:** 8

## Description
Connect your **Filestack** account to any AI agent to handle complex file workflows, from cloud uploads to advanced AI content analysis, through simple commands.

### What you can do

- **Smart Uploads** — Upload files directly from any public URL to your Filestack S3 storage using `upload_from_url`.
- **AI Intelligence** — Automatically extract text from documents (`get_ocr`), detect objects and features in images (`get_image_tags`), and check for unsafe content (`get_sfw_status`).
- **Image Transformations** — Generate optimized CDN URLs for resizing, blurring, or filtering images using `generate_transform_url` without manual editing.
- **Video Processing** — Initiate and monitor asynchronous video transcoding jobs (`start_video_transcode`) to convert files into web-ready formats like MP4 or HLS.
- **Metadata Inspection** — Retrieve deep technical details including dimensions, mime types, and file sizes with `get_metadata`.

### How it works

1. Subscribe to this server
2. Enter your Filestack API Key (and optional Policy/Signature for security)
3. Start processing assets directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — Automate asset pipelines and generate transformation URLs directly from the code editor.
- **Content Moderators** — Use AI to automatically flag unsafe images or tag visual assets at scale.
- **Data Engineers** — Extract structured text from scanned documents and images using OCR for downstream processing.


## Available Tools
- **get_image_tags**: Detect objects and features in an image
- **get_metadata**: Get metadata for a Filestack file
- **get_ocr**: Extract printed or handwritten text (OCR)
- **get_sfw_status**: Detect unsafe content (Safe for Work)
- **generate_transform_url**: g., resize=width:400). Does not execute the request, just returns the URL.

Generate a Filestack transformation URL
- **upload_from_url**: Upload a file to Filestack from a public URL
- **get_video_status**: Poll status of a video transcoding job
- **start_video_transcode**: Returns a UUID that must be used to poll for status.

Start asynchronous video/audio transcoding


## Installation & Usage

To install and use the **FileStack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/filestack](https://vinkius.com/mcp/filestack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
