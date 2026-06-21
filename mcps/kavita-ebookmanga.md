# Kavita (eBook/Manga) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kavita-ebookmanga)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Manage your Kavita media server—scan libraries, check API status, and authenticate sessions directly from your AI agent.

## Description
Connect your **Kavita** instance to any AI agent to automate library management and monitor your eBook and Manga collection through natural conversation.

### What you can do

- **Library Maintenance** — Trigger full scans of all your libraries or target a specific library by ID to detect new content immediately.
- **API Monitoring** — Check the expiration date of your API keys to ensure uninterrupted access to your media server.
- **Session Management** — Authenticate and retrieve JWT tokens for secure, session-based interactions with the Kavita API.

### How it works

1. Subscribe to this server
2. Enter your Kavita Server URL and API Key
3. Start managing your digital library from Claude, Cursor, or any MCP-compatible client

No more manual clicks in the web UI just to refresh your latest manga chapters. Your AI acts as your personal digital librarian.

### Who is this for?

- **Self-Hosters** — automate the maintenance of your media server without leaving your workspace.
- **Manga & Comic Collectors** — ensure your latest releases are indexed and ready to read as soon as they hit your storage.
- **Developers** — integrate Kavita management into your coding workflows or custom automation scripts.


## Available Tools (4)
- **check_authkey_expires**: Check API key expiration date
- **authenticate**: Authenticate and receive a JWT token
- **scan_all_libraries**: Trigger a scan of all libraries
- **scan_library**: Trigger a scan for a specific library


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kavita (eBook/Manga)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan all my Kavita libraries for new manga."

**🤖 AI Agent:**
> I've triggered a global scan for all your libraries. Kavita is now processing your folders to detect any new or updated files.

---

**👤 You:**
> "Check when my Kavita API key expires."

**🤖 AI Agent:**
> I've checked your API key status. It is set to expire on 2025-12-31. You have plenty of time before needing a refresh.

---

**👤 You:**
> "Trigger a scan for library ID 5."

**🤖 AI Agent:**
> Targeted scan for Library ID 5 has been started. I will let you know if any issues occur during the process.


## ❓ FAQ

**Q: Can I trigger a scan for just one specific library?**
Yes! Use the `scan_library` tool and provide the specific Library ID. The agent will trigger a targeted scan to detect new or changed content in that folder only.

**Q: How do I check if my API key is still valid?**
You can run the `check_authkey_expires` tool. It will return the exact expiration timestamp for your current API key, helping you avoid service interruptions.

**Q: Can I refresh my entire collection at once?**
Absolutely. Use the `scan_all_libraries` tool to trigger a global scan across all configured libraries in your Kavita instance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kavita-ebookmanga](https://vinkius.com/mcp/kavita-ebookmanga)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kavita (eBook/Manga)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kavita-ebookmanga` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kavita (eBook/Manga)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kavita-ebookmanga": {
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
