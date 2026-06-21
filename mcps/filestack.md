# FileStack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/filestack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Upload, transform, and analyze files with Filestack—extract text via OCR, detect objects, and manage video transcoding directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FileStack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Upload this image to Filestack: https://example.com/photo.jpg"

**🤖 AI Agent:**
> I've uploaded the file. The new Filestack handle is `ABC123XYZ`. You can now use this handle for transformations or metadata analysis.

---

**👤 You:**
> "What objects are detected in the image with handle ABC123XYZ?"

**🤖 AI Agent:**
> Analyzing the image... I've detected several tags: 'mountain' (98% confidence), 'snow' (95%), and 'outdoor' (92%).

---

**👤 You:**
> "Convert the video ABC123XYZ to mp4 format."

**🤖 AI Agent:**
> I've started the transcoding job for handle ABC123XYZ using the 'mp4' preset. The job UUID is `job-550e8400`. You can check the status later using `get_video_status`.


## ❓ FAQ

**Q: How can I extract text from a scanned document or image?**
Use the `get_ocr` tool with the file handle. The AI will perform Optical Character Recognition and return the extracted text along with its coordinates.

**Q: Is there a way to check if an uploaded image contains adult or unsafe content?**
Yes, the `get_sfw_status` tool uses Filestack Intelligence to analyze the image and return a safety score, helping you moderate content automatically.

**Q: Can I resize an image without actually downloading and re-uploading it?**
Absolutely. Use `generate_transform_url` to create a specific CDN URL with tasks like `resize=width:400`. This allows the Filestack CDN to handle the transformation on the fly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/filestack](https://vinkius.com/mcp/filestack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FileStack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `filestack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FileStack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "filestack": {
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
