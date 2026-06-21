# Howuku MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/howuku)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Analyze user behavior via Howuku — track projects, recordings, and heatmaps.

## Description
Empower your AI agents to analyze user behavior on your websites. This MCP server connects to Howuku (now part of VWO) to list projects, retrieve session recordings, view heatmaps, and monitor user feedback and surveys. Perfect for UX researchers and product managers.


## Available Tools
- **get_me**: Gets current authenticated user info
- **get_project**: Retrieves details for a specific project
- **list_events**: Lists custom tracking events for a project
- **list_feedback**: Lists visual feedback items for a project
- **list_funnels**: Lists conversion funnels for a project
- **list_heatmaps**: Lists heatmaps for a project
- **list_organizations**: Lists organizations associated with your account
- **list_projects**: Lists Howuku projects (sites)
- **list_recordings**: Lists session recordings for a project
- **list_surveys**: Lists surveys for a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Howuku** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Howuku projects."

**🤖 AI Agent:**
> I'll fetch your project list for you.

---

**👤 You:**
> "Show me recent session recordings for project ID 123."

**🤖 AI Agent:**
> I'll retrieve the latest recordings for that project.

---

**👤 You:**
> "Check for any new user feedback on my site."

**🤖 AI Agent:**
> I'll check the feedback items for your projects.


## ❓ FAQ

**Q: Is this the same as VWO?**
Howuku was acquired by VWO. This MCP uses the Howuku API which is now part of the VWO ecosystem.

**Q: How do I get my Howuku API Key?**
You can find your API key in your Howuku/VWO dashboard under Account Settings > API Keys.

**Q: Can I see session recordings?**
The list_recordings tool provides metadata and links to view session recordings for your projects.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/howuku](https://vinkius.com/mcp/howuku)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Howuku** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `howuku` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Howuku** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "howuku": {
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
