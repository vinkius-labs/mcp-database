# Vectorizer AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vectorizer-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Convert bitmap images (JPG, PNG) into high-quality vector graphics (SVG, EPS, PDF, DXF) using AI-powered tracing.

## Description
Connect to **Vectorizer AI** to transform pixel-based images into clean, scalable vector graphics directly from your AI agent. This server leverages powerful AI algorithms to trace bitmaps and produce professional-grade SVG, EPS, PDF, and DXF files.

### What you can do

- **Vectorization** — Convert JPG, PNG, or BMP files into vectors with precise control over colors, shapes, and stacking.
- **Format Conversion** — Export to multiple industry-standard formats including SVG, EPS, PDF, and DXF.
- **Advanced Processing** — Fine-tune results with custom palettes, minimum shape areas, and specific draw styles.
- **Account Management** — Check your API credit balance and manage stored images.

### How it works

1. Subscribe to this server
2. Enter your Vectorizer AI API ID and API Secret
3. Start vectorizing images from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Graphic Designers** — Quickly convert client logos or sketches into editable vector formats.
- **Engineers & Makers** — Generate DXF files for CNC or laser cutting directly from reference images.
- **Content Creators** — Upscale low-resolution assets into infinitely scalable graphics.


## Available Tools (4)
- **download_image**: Download a production result or additional formats
- **vectorize_image**: Vectorize a bitmap image to SVG/EPS/PDF/DXF
- **get_account_status**: Fetch subscription status and remaining credits
- **delete_image**: AI servers using its image token.

Manually delete an image stored via policy.retention_days > 0


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vectorizer AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Vectorize this logo from https://example.com/logo.png into an SVG."

**🤖 AI Agent:**
> I've started the vectorization process for your image. The AI is tracing the bitmap to create a clean SVG file. You can download the result using the provided token.

---

**👤 You:**
> "I have an image token 'v_12345'. Can you download it as a DXF file for CNC?"

**🤖 AI Agent:**
> Fetching the DXF version for token 'v_12345'... I've generated the download link for your CNC-compatible file.

---

**👤 You:**
> "Check my Vectorizer AI account balance."

**🤖 AI Agent:**
> Your Vectorizer AI account currently has 450 credits remaining. Your account status is active.


## ❓ FAQ

**Q: Can I convert a PNG to SVG directly?**
Yes, use the `vectorize_image` tool and set the `output_file_format` to 'svg'. The AI will process the bitmap and return a high-quality vector result.

**Q: How do I download a different format for an image I already processed?**
Use the `download_image` tool with the `image_token` from your previous request. You can specify a new `output_file_format` like 'dxf' or 'pdf' without re-uploading the image.

**Q: How do I check my remaining API credits?**
Run the `get_account` tool. It will return your current credit balance and account status directly from Vectorizer AI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vectorizer-ai](https://vinkius.com/mcp/vectorizer-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vectorizer AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vectorizer-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vectorizer AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vectorizer-ai": {
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
