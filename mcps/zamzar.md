# Zamzar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zamzar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Convert files between 1100+ formats — transform documents, images, videos, and audio directly through your AI agent.

## Description
Connect your **Zamzar** developer account to any AI agent and automate complex file conversion workflows using natural language. Zamzar supports over 1100 formats including PDF, DOCX, PNG, MP4, and more.

### What you can do

- **Format Discovery** — Use `list_formats` to see all supported conversions or `get_format` to check specific target options and credit costs.
- **File Conversion** — Trigger `start_job` to convert files from any public URL or S3 URI to your desired output format.
- **Status Monitoring** — Track the progress of your conversions with `get_job`, monitoring states from initialising to successful.
- **Content Retrieval** — Once a conversion is finished, use `get_file_content` to download the binary data of your new file.

### How it works

1. Subscribe to this server
2. Enter your Zamzar API Key
3. Start converting files directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Quickly convert images or videos to web-ready formats without leaving your workflow.
- **Developers** — Automate document processing and file transformations within your coding environment.
- **Business Professionals** — Instantly turn PDFs into editable documents or spreadsheets via simple chat commands.


## Available Tools
- **get_file_content**: Returns metadata about the downloaded file.

Download the converted file content
- **get_format**: Retrieve details for a specific format
- **get_job**: Statuses include initialising, converting, successful, failed.

Retrieve the status of a specific job
- **list_formats**: List all supported file formats
- **start_job**: Start a file conversion job


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zamzar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all supported file formats available on Zamzar."

**🤖 AI Agent:**
> I've retrieved the list of supported formats. Zamzar supports over 1100 formats including documents (pdf, docx), images (jpg, png), and videos (mp4, avi). Is there a specific format you're looking for?

---

**👤 You:**
> "Convert this image URL https://example.com/image.gif to a PNG file."

**🤖 AI Agent:**
> I've started the conversion job for your GIF to PNG. The Job ID is 456789. I'll monitor the status for you, or you can ask me to check it anytime using `get_job`.

---

**👤 You:**
> "Check the status of conversion job 456789 and download it if ready."

**🤖 AI Agent:**
> The job 456789 is now 'successful'. I am now retrieving the file content for you using the associated file ID.


## ❓ FAQ

**Q: How can I check if Zamzar supports converting a specific file type?**
You can use the `get_format` tool by providing the extension (e.g., 'pdf'). The agent will return all possible target formats and the associated credit cost for that conversion.

**Q: How do I know when my file conversion is finished and ready for download?**
After starting a job, use the `get_job` tool with your Job ID. It will report the current status. Once it shows 'successful', you can proceed to download the file.

**Q: Can I download the converted file directly through the AI?**
Yes. Once the job is successful, use the `get_file_content` tool with the resulting File ID to retrieve the binary data and metadata of the converted file.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zamzar](https://vinkius.com/mcp/zamzar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zamzar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zamzar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zamzar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zamzar": {
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
