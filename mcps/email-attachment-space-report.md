# Email Attachment Space Report MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/email-attachment-space-report)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Summarize email attachment storage usage by sender, type, and size.

## Description
This MCP server provides tools to analyze email attachment metadata. Use `analyze_attachment_totals` to get a high-level overview of storage consumption, `find_largest_attachments` to identify heavy files, `group_by_category` to break down usage by file type or label, and `filter_large_files` to find specific attachments exceeding a size threshold.


## Available Tools (4)
- **analyze_attachment_totals**: Provides a high-level summary of total storage usage across all provided records
- **filter_large_files**: Retrieves a list of all attachments that exceed a specific size limit
- **find_largest_attachments**: Identifies the specific files consuming the most space
- **group_by_category**: Breaks down storage consumption by file type or organizational label


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Email Attachment Space Report** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much total space are my email attachments using?"

**🤖 AI Agent:**
> The total storage usage for the provided attachments is 450 MB across 12 files.

---

**👤 You:**
> "Show me the top 3 largest attachments."

**🤖 AI Agent:**
> The largest attachments are: report.pdf (50 MB) from alice@example.com, video.mp4 (40 MB) from bob@example.com, and image.png (15 MB) from charlie@example.com.

---

**👤 You:**
> "Which files are larger than 10 MB?"

**🤖 AI Agent:**
> There are 2 files larger than 10 MB: presentation.pptx (12 MB) and archive.zip (25 MB).


## ❓ FAQ

**Q: What kind of data does this server process?**
It processes attachment records containing sender identity, timestamp, file size, file type, and organizational labels.

**Q: How can I find the biggest files in my list?**
You can use the `find_largest_attachments` tool to retrieve a ranked list of the largest files.

**Q: Can I group my storage usage by file extension?**
Yes, the `group_by_category` tool allows you to group data by either 'fileType' or 'label'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/email-attachment-space-report](https://vinkius.com/en/ai-agent-connect/email-attachment-space-report)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Email Attachment Space Report** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `email-attachment-space-report` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Email Attachment Space Report** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "email-attachment-space-report": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
