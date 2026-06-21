# Bright Pattern MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bright-pattern)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Orchestrate your contact center via Bright Pattern — manage users, track interactions, and monitor real-time stats directly from any AI agent.

## Description
Connect your **Bright Pattern** contact center account to any AI agent and orchestrate your customer service, interaction management, and operational reporting workflows through natural conversation.

### What you can do

- **User & Team Oversight** — List and retrieve detailed profiles for agents, supervisors, and teams managed within the platform.
- **Interaction Tracking** — Query and inspect recent voice, chat, and SMS interactions to monitor service quality.
- **Real-time Statistics** — Access core operational metrics for services, agents, and campaigns directly from your workspace.
- **Service Configuration** — List configured services, campaigns, and skills to verify your contact center setup.
- **Tenant Insights** — Retrieve core tenant information and configuration metadata using natural language.

### How it works

1. Subscribe to this server
2. Enter your Bright Pattern Tenant Domain, Client ID, and Client Secret
3. Start managing your contact center operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Contact Center Managers** — quickly check real-time stats and agent statuses without manual dashboard monitoring.
- **Quality Assurance Leads** — retrieve interaction details and recordings straight from their workflow tools.
- **Ops Engineers** — verify tenant configurations and user settings using natural language.


## Available Tools
- **get_tenant_config**: Retrieve core tenant configuration
- **get_interaction_details**: Get metadata for a specific interaction
- **get_realtime_stats**: Get real-time contact center statistics
- **get_user**: Get details of a specific user
- **list_campaigns**: List all outbound campaigns
- **list_interactions**: List recent interactions (calls, chats)
- **list_services**: List all contact center services
- **list_skills**: List all configured agent skills
- **list_teams**: List all agent teams
- **list_users**: List all contact center users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bright Pattern** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active agents in Bright Pattern."

**🤖 AI Agent:**
> I've retrieved your users. You have 15 agents configured, including 'Alice Johnson' (ID: user_1) and 'Mark Smith' (ID: user_2). Would you like to check the status for any of them?

---

**👤 You:**
> "Show real-time statistics for the contact center."

**🤖 AI Agent:**
> Retrieving statistics... Currently, there are 5 calls in queue, average wait time is 45 seconds, and 12 agents are logged in and ready.

---

**👤 You:**
> "Get details for interaction ID int_99283."

**🤖 AI Agent:**
> Interaction int_99283 was a 5-minute voice call from +15550199 handled by agent Alice. The sentiment analysis indicates a positive customer experience.


## ❓ FAQ

**Q: Can I check real-time statistics for my services using the agent?**
Yes! Use the `get_realtime_stats` tool. Your agent will fetch the core operational metrics, allowing you to see current call volumes and agent availability directly.

**Q: How do I list all the agents in a specific team?**
Simply ask the agent to `list_users`. You can then filter for the relevant team metadata or use the `list_teams` tool to see the team structure and then inspect individual members.

**Q: Does the integration allow managing agent skills?**
Currently, the toolset focuses on querying and monitoring (Read-Only). Use the `list_skills` tool to retrieve the configured skills, but assignments or updates must be done through the Bright Pattern Administrator portal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bright-pattern](https://vinkius.com/mcp/bright-pattern)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bright Pattern** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bright-pattern` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bright Pattern** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bright-pattern": {
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
