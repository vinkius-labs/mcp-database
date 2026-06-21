# iLEVEL (S&P Global) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ilevel-sp-global)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage private equity investments, portfolios, and funds via iLEVEL API.

## Description
Empower your AI agents to interact with your iLEVEL private equity data. This MCP server allows you to list investments, retrieve entity details, manage portfolios, and view fund information directly through the iLEVEL API. Ideal for automating financial reporting and portfolio monitoring.


## Available Tools (10)
- **get_investment**: Retrieves details for a specific investment
- **get_status**: Gets the iLEVEL system status
- **get_version**: Gets the iLEVEL API version
- **list_assets**: Lists all assets
- **list_contacts**: Lists all contacts
- **list_entities**: Lists all legal entities
- **list_funds**: Lists all funds
- **list_investments**: Lists all investments
- **list_portfolios**: Lists all portfolios
- **list_users**: Lists all users in the system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **iLEVEL (S&P Global)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active investments in my iLEVEL portfolio."

**🤖 AI Agent:**
> I'll fetch the list of investments for you.

---

**👤 You:**
> "Show me the details for the 'Alpha Fund' entity."

**🤖 AI Agent:**
> I'll retrieve the entity information from iLEVEL.

---

**👤 You:**
> "Check the system status and API version."

**🤖 AI Agent:**
> I'll look up the current system status and version details for you.


## ❓ FAQ

**Q: How do I get iLEVEL API credentials?**
You need to contact your iLEVEL account manager or S&P Global support to enable Web Services access and obtain your API username and key.

**Q: Is the instance domain required?**
Yes, each firm has a specific iLEVEL instance URL (e.g., firmname.ilevelconnect.com) that must be provided during setup.

**Q: Can I see all my investments?**
Yes, the list_investments tool provides access to the full list of investments documented in your iLEVEL instance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ilevel-sp-global](https://vinkius.com/mcp/ilevel-sp-global)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **iLEVEL (S&P Global)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ilevel-sp-global` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **iLEVEL (S&P Global)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ilevel-sp-global": {
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
