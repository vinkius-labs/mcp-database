# Kitetags MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kitetags)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Generate optimized hashtags for Instagram and TikTok posts with AI that analyzes trending tags and maximizes reach.

## Description
Connect your **Kitetags** account to any AI agent and take full control of your asset tracking infrastructure and automated smart tag workflows through natural conversation.

### What you can do

- **Tag Portfolio Orchestration** — List and manage your entire high-fidelity database of smart tags programmatically, retrieving detailed technical metadata and claim status
- **Location Intelligence** — Programmatically query and monitor the last known locations of your tagged assets to maintain a perfectly coordinated logistical overview
- **Group & Category Architecture** — Access your complete directory of tag groups and categories to oversee your organizational resource allocation in real-time
- **Smart Alert Monitoring** — Access real-time status updates and track tag activity directly through your agent for instant operational reporting
- **Operational Monitoring** — Verify account-level API connectivity and monitor tag volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Kitetags dashboard (Settings > API & Integrations)
3. Start orchestrating your assets from Claude, Cursor, or any MCP client

No more manual checking of individual tag locations or missing critical asset moves. Your AI acts as your dedicated logistics coordinator and tag architect.

### Who is this for?

- **Logistics Managers** — instantly retrieve asset summaries and monitor tag locations using natural language commands
- **Asset Controllers** — verify tag claim statuses and track group assignments without leaving your creative workspace
- **Growth Leads** — integrate high-speed smart tag data into custom inventory pipelines through simple AI queries


## Available Tools (12)
- **check_kitetags_status**: Verify connectivity
- **create_group**: Create a group
- **create_tag**: Create a tag
- **delete_group**: Delete a group
- **delete_tag**: Delete a tag
- **get_tag_analytics**: Get tag analytics
- **get_group**: Get group details
- **get_tag**: Get tag details
- **list_group_tags**: List tags in group
- **list_groups**: List groups
- **list_tags**: List tags
- **search_tags**: Search tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kitetags** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active smart tags in my Kitetags account."

**🤖 AI Agent:**
> I've retrieved your tags. You currently have 50 active smart tags, including 'Asset #123' and 'Warehouse B'. Would you like the detailed high-fidelity location metadata for any of them?

---

**👤 You:**
> "Show the last known location for tag ID 'tag_987'."

**🤖 AI Agent:**
> Accessing location intelligence... Tag tag_987 was last seen at 'Main Distribution Center' at 2:00 PM today. I've retrieved the high-fidelity GPS metadata for your review. Need help monitoring the group status?

---

**👤 You:**
> "List all tag groups and their current member counts."

**🤖 AI Agent:**
> Group directory orchestrated! I've identified 5 active high-fidelity groups, including 'High Value' (20 tags) and 'Electronics'. I've retrieved the technical metadata and categories for you. Shall I check for unassigned tags?


## ❓ FAQ

**Q: How do I find my Kitetags API Key?**
Log in to your account, navigate to **Settings** > **API & Integrations**, and copy your unique Access Token.

**Q: Can I see last known locations via AI?**
Yes! The `list_kitetags_tags` tool provides high-fidelity location metadata and timestamps for all your smart tags.

**Q: How do I list my tag groups?**
Use the `list_kitetags_groups` tool to retrieve your complete high-fidelity directory along with the unique identifiers for all managed categories.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kitetags](https://vinkius.com/mcp/kitetags)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kitetags** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kitetags` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kitetags** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kitetags": {
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
