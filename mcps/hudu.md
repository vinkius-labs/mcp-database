# Hudu MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hudu)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Manage IT documentation, assets, and passwords via Hudu API.

## Description
Empower your AI agents to interact with your Hudu IT documentation. This MCP server allows you to list companies, retrieve asset details, manage contacts, view knowledge base articles, and access stored passwords directly through the Hudu API. Ideal for automating MSP workflows and IT management.


## Available Tools (10)
- **get_company**: Retrieves details for a specific company
- **list_activity_logs**: Lists activity logs
- **list_articles**: Lists knowledge base articles
- **list_assets**: Lists documented assets
- **list_companies**: Lists all companies in Hudu
- **list_contacts**: Lists contacts across all companies
- **list_networks**: Lists documented networks
- **list_passwords**: Lists stored passwords
- **list_procedures**: Lists documented procedures
- **list_websites**: Lists monitored websites


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hudu** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all companies documented in Hudu."

**🤖 AI Agent:**
> I'll fetch the list of companies for you.

---

**👤 You:**
> "Show me assets for company ID 123."

**🤖 AI Agent:**
> I'll retrieve the assets documented for that company.

---

**👤 You:**
> "Find knowledge base articles related to backup procedures."

**🤖 AI Agent:**
> I'll search your knowledge base for backup procedures.


## ❓ FAQ

**Q: How do I get Hudu API credentials?**
You can generate an API key in your Hudu dashboard under Account Settings > API. You also need your Hudu instance domain.

**Q: Can I see passwords with this MCP?**
Yes, the list_passwords tool provides access to documented passwords in your Hudu instance.

**Q: Does it support self-hosted Hudu?**
Yes, as long as your Hudu instance is accessible via the internet and the domain provided is correct.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hudu](https://vinkius.com/mcp/hudu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hudu** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hudu` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hudu** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hudu": {
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
