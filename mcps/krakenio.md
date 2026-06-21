# Kraken.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/krakenio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimize, compress, and resize images via URL or direct upload using the Kraken.io API.

## Description
Connect **Kraken.io** to your AI agent to automate image processing. Reduce page load times and save storage space by compressing images with industry-leading algorithms.

### What you can do

- **URL Optimization** — Provide a link to any image and get an optimized version back instantly via the `optimize_url` tool
- **Direct Uploads** — Process base64 encoded images directly from your workflow using `upload_image` 
- **Smart Resizing** — Resize images to specific dimensions using various strategies (exact, portrait, landscape, etc.) during optimization
- **Quota Management** — Monitor your plan usage, total quota, and remaining balance with `get_user_status` 
- **Sandbox Testing** — Use the 'dev' mode to test your integration without consuming your paid quota

### How it works

1. Subscribe to this server
2. Enter your Kraken.io API Key and API Secret
3. Start optimizing images from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web Developers** — automate image optimization in content workflows to improve Core Web Vitals
- **Content Managers** — ensure all uploaded assets are compressed and resized correctly without manual tools
- **Designers** — quickly generate web-ready versions of high-resolution assets through natural conversation


## Available Tools
- **get_user_status**: io account.

Get Kraken.io user status and quota
- **optimize_url**: io. Supports lossy/lossless compression, resizing, and format conversion.

Optimize an image from a URL
- **upload_image**: io.

Upload and optimize a base64 encoded image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kraken.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Optimize this image URL: https://example.com/photo.jpg using lossy compression."

**🤖 AI Agent:**
> I've optimized the image. The original size was 1.2MB and the new size is 450KB (62% reduction). You can download it here: [URL]

---

**👤 You:**
> "Check my Kraken.io account status and remaining quota."

**🤖 AI Agent:**
> Your account is on the 'Micro' plan. You have used 150MB out of 500MB total quota, leaving you with 350MB remaining for this month.

---

**👤 You:**
> "Upload this base64 image as 'profile.png' and resize it to 200x200 using the 'exact' strategy."

**🤖 AI Agent:**
> The image has been uploaded, resized to 200x200, and optimized. The final file is ready at: [URL]


## ❓ FAQ

**Q: How can I check my remaining Kraken.io quota?**
Use the `get_user_status` tool. It will return your plan name, total quota, used quota, and exactly how much remains in your account.

**Q: Can I resize an image while it's being optimized?**
Yes! Both `optimize_url` and `upload_image` support a `resize` parameter. You can specify width, height, and a strategy like 'exact', 'portrait', or 'landscape'.

**Q: Is there a way to test the API without using my paid credits?**
Yes, you can set the `dev` parameter to true in your optimization requests. This uses the API Sandbox, which returns randomized results and does not consume your quota.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/krakenio](https://vinkius.com/mcp/krakenio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kraken.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `krakenio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kraken.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "krakenio": {
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
