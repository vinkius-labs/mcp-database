# Interact Software MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/interact-software)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage intranet people, content, and groups via Interact Software API.

## Description
Empower your AI agents to interact with your corporate intranet using Interact Software. This MCP server allows you to list people, retrieve content and news, manage groups and departments, and search across your organization directly through the Interact API. Ideal for automating internal communications and knowledge retrieval.


## Available Tools (10)
- **get_analytics**: Retrieves intranet usage analytics
- **get_person**: Retrieves details for a specific person
- **list_content**: Lists intranet content items
- **list_departments**: Lists all organization departments
- **list_events**: Lists upcoming intranet events
- **list_groups**: Lists all collaboration groups
- **list_locations**: Lists all organization locations
- **list_news**: Lists latest news articles
- **list_people**: Lists all people/users in the intranet
- **search**: Searches for content, people, and groups


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Interact Software** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all people in the 'Marketing' department."

**🤖 AI Agent:**
> I'll fetch the list of users in the marketing department for you.

---

**👤 You:**
> "Show me the latest news articles on the intranet."

**🤖 AI Agent:**
> I'll retrieve the latest news articles and updates from your corporate intranet.

---

**👤 You:**
> "Search for 'remote work policy' in Interact."

**🤖 AI Agent:**
> I'll perform a global search for that policy across the intranet.


## ❓ FAQ

**Q: How do I get Interact API credentials?**
You need to generate an API Key within your Interact intranet administration settings. You also need your tenant identifier and application ID (appid).

**Q: What is the 'appid'?**
The appid is the unique ID of the application or connector you created in Interact. You can find it in the URL when editing the connector.

**Q: Can I search across the intranet?**
Yes, the search tool allows you to perform global searches for content, people, and groups within your Interact intranet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/interact-software](https://vinkius.com/mcp/interact-software)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Interact Software** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `interact-software` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Interact Software** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "interact-software": {
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
