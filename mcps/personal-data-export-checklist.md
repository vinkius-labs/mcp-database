# Personal Data Export Checklist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/personal-data-export-checklist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and manage data portability requests from digital services.

## Description
This MCP server provides a centralized system for managing data portability requests. Users can use `create_export_task` to initiate tracking for requests from various platforms, monitor active requests with `list_pending_requests`, and retrieve completed data via `list_available_downloads`. It also includes `get_expiry_reminders` to ensure users do not miss their download windows.


## Available Tools (4)
- **create_export_task**: Initiate a new tracking entry for a data portability request
- **get_expiry_reminders**: Alert the user to downloads that are nearing their expiration limit
- **list_available_downloads**: Identify all completed requests where the data is ready for retrieval
- **list_pending_requests**: View all active data requests that have not yet resulted in a completed download


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Personal Data Export Checklist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just requested my contact info from my social media account. Can you track this for me?"

**🤖 AI Agent:**
> I have created a new export task for your social media contact information request.

---

**👤 You:**
> "Are there any data downloads ready for me right now?"

**🤖 AI Agent:**
> You have 2 completed downloads available for retrieval.

---

**👤 You:**
> "Show me all my pending data export requests."

**🤖 AI Agent:**
> You have 3 pending requests: Cloud Storage (due tomorrow), Email (due in 3 days), and Messaging (due in 5 days).


## ❓ FAQ

**Q: How do I start a new data request tracking?**
You can use the `create_export_task` tool to log a new request, specifying the service, data categories, and expected timelines.

**Q: How can I see if my data is ready to download?**
Use the `list_available_downloads` tool to see all completed requests that have valid download links.

**Q: Will I be notified before a download link expires?**
Yes, you can use `get_expiry_reminders` to identify downloads that are approaching their expiration date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/personal-data-export-checklist](https://vinkius.com/en/ai-agent-connect/personal-data-export-checklist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Personal Data Export Checklist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `personal-data-export-checklist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Personal Data Export Checklist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "personal-data-export-checklist": {
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
