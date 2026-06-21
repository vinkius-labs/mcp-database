# Convertio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/convertio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Enable your AI agent to convert images, documents, audio, and video files across hundreds of formats using the Convertio API.

## Description
Connect your AI agent to **Convertio**, the versatile file conversion platform supporting over 300 formats.

### What you can do

- **Document Conversion** — Convert Word documents to PDF, markdown to HTML, or any text format instantly.
- **Media Encoding** — Compress audio files or convert images from SVG to PNG/JPG.
- **Status Tracking** — Query conversion progress and retrieve the download link when ready.

### How it works

1. Add the Convertio integration to your AI toolset.
2. Provide your Convertio API Key.
3. Ask your agent to convert files by URL and it handles the rest.

### Who is this for?

- **Media Managers** — Quickly adapt assets into web-friendly formats without heavy editing suites.
- **Developers** — Automate file normalization pipelines for user uploads.
- **Content Creators** — Convert proprietary media formats into universal extensions via chat.


## Available Tools (8)
- **convert_file**: Start a new file conversion job
- **quick_convert_to_jpg**: Quickly convert any image URL to JPG
- **quick_convert_to_pdf**: Quickly convert any document URL to PDF
- **delete_conversion_job**: Remove a job and its file from Convertio servers
- **get_account_balance**: Check your Convertio API credit balance
- **get_conversion_status**: Check the status of a conversion job
- **list_common_formats**: List common supported formats for conversion
- **list_active_jobs**: List your current active conversion jobs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Convertio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert this SVG to PNG: 'https://example.com/logo.svg'"

**🤖 AI Agent:**
> I've sent the SVG file to Convertio for PNG conversion. Conversion ID: 'a8s9df7s9'. Status: encoding. I'll notify you when the download link is ready.

---

**👤 You:**
> "Check the status of conversion 'a8s9df7s9'."

**🤖 AI Agent:**
> Conversion 'a8s9df7s9' is complete! File size: 45 KB. Download your PNG here: [Download Link]. Note: the link expires in 24 hours.

---

**👤 You:**
> "How many conversion credits do I have left in my Convertio account?"

**🤖 AI Agent:**
> You currently have 450 credits remaining. Your plan allows for up to 25 concurrent conversions. Would you like to see a list of your most recent jobs?


## ❓ FAQ

**Q: Where do I find my Convertio API Key?**
Log in to the Convertio developer dashboard at developers.convertio.co. Go to 'API Keys' in the account menu, click 'Generate', copy the key, and paste it below.

**Q: Are there file size limitations?**
Yes. Limits depend on your Convertio billing plan. Free tiers have strict file size limits and usage quotas. The integration passes files through the API transparently — your plan determines the max capacity.

**Q: Does the agent download the converted file automatically?**
No. For security, the agent provides you with the download URL once the conversion finishes. You decide when and where to save the file.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/convertio](https://vinkius.com/mcp/convertio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Convertio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `convertio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Convertio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "convertio": {
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
