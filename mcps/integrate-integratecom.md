# Integrate (Integrate.com) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/integrate-integratecom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage marketing campaigns, leads, and sources via Integrate.com API.

## Description
Empower your AI agents to manage your B2B marketing orchestration with Integrate.com. This MCP server allows you to list campaigns, track leads, monitor sources and media partners, and view system status directly through the Integrate API. Ideal for automating marketing operations and lead flow monitoring.


## Available Tools (10)
- **get_lead**: Retrieves details for a specific lead
- **get_system_status**: Gets the current Integrate system status
- **list_campaigns**: Lists all marketing campaigns
- **list_dispositions**: Lists all lead dispositions (rejected, valid, etc.)
- **list_leads**: Lists all marketing leads
- **list_media_partners**: Lists all registered media partners
- **list_reports**: Lists available marketing reports
- **list_segments**: Lists all defined audience segments
- **list_sources**: Lists all configured lead sources
- **list_users**: Lists all users in the organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Integrate (Integrate.com)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active campaigns in my Integrate.com account."

**🤖 AI Agent:**
> I'll fetch the list of your active marketing campaigns for you.

---

**👤 You:**
> "Show me the last 5 leads processed."

**🤖 AI Agent:**
> I'll retrieve the most recent leads and their current statuses.

---

**👤 You:**
> "Check the system status of the Integrate platform."

**🤖 AI Agent:**
> I'll look up the current operational status of the Integrate API.


## ❓ FAQ

**Q: How do I get Integrate.com API credentials?**
Log in to your Integrate account and navigate to Settings > API Keys to generate your unique API key.

**Q: Can I see lead dispositions?**
Yes, the list_dispositions tool provides access to the status and validation results of your leads.

**Q: Is system status monitored?**
Yes, you can use the get_system_status tool to check the operational health of the Integrate platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/integrate-integratecom](https://vinkius.com/mcp/integrate-integratecom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Integrate (Integrate.com)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `integrate-integratecom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Integrate (Integrate.com)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "integrate-integratecom": {
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
