# Huginn (IFTTT Alternative) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/huginn-ifttt-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate workflows with Huginn — manage agents, trigger webhooks, and orchestrate complex scenarios directly from your AI agent.

## Description
Connect your self-hosted **Huginn** instance to any AI agent and take full control of your automation pipelines through natural conversation. Huginn is the powerful, open-source alternative to IFTTT and Zapier that lives on your own server.

### What you can do

- **Agent Management** — List, create, update, and delete agents. Manually trigger runs for any agent in your system.
- **Webhook Integration** — Send arbitrary JSON data to your Webhook Agents to kick off complex backend workflows.
- **Event Monitoring** — Inspect recent events, view detailed payloads, and re-emit events to downstream agents for debugging or re-processing.
- **Scenario Orchestration** — List all scenarios and export or import entire agent groups as JSON for easy backup and migration.
- **System Visibility** — Get complete metadata for any agent or event to understand exactly how your data is flowing.

### How it works

1. Subscribe to this server
2. Provide your Huginn Base URL and API Token
3. Start orchestrating your private automation cloud from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — Monitor system events and trigger recovery workflows without leaving the terminal or chat.
- **Data Enthusiasts** — Manage web-scraping agents and inspect captured data payloads via natural language.
- **Automation Power Users** — Orchestrate complex multi-step scenarios and migrate configurations between instances seamlessly.


## Available Tools
- **list_events**: List recent Huginn events
- **create_agent**: Create a new Huginn agent
- **delete_agent**: Delete a Huginn agent
- **export_scenario**: Export a Huginn scenario as JSON
- **get_agent**: Get details for a specific Huginn agent
- **get_event**: Get details for a specific Huginn event
- **import_scenario**: Import a Huginn scenario from JSON
- **list_agents**: List all Huginn agents
- **list_scenarios**: List all Huginn scenarios
- **reemit_event**: Re-emit an existing Huginn event
- **run_agent**: Manually trigger a Huginn agent to run
- **trigger_webhook**: Trigger a Huginn Webhook Agent
- **update_agent**: Update an existing Huginn agent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Huginn (IFTTT Alternative)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Huginn agents and their current status."

**🤖 AI Agent:**
> I've retrieved your agents. You have 3 active agents: 'Weather Notifier' (ID: 12), 'eBay Scraper' (ID: 15), and 'Slack Webhook' (ID: 20). All are currently in good standing.

---

**👤 You:**
> "Trigger the webhook agent 42 with secret 'top-secret' and payload {"action": "deploy"}."

**🤖 AI Agent:**
> Successfully triggered Webhook Agent 42. The payload has been sent and the workflow is now processing.

---

**👤 You:**
> "Export the scenario with ID 5 so I can back it up."

**🤖 AI Agent:**
> I have exported the scenario 'Home Automation' (ID: 5). Here is the JSON configuration containing all associated agents and settings.


## ❓ FAQ

**Q: How do I trigger a specific Webhook Agent with data?**
Use the `trigger_webhook` tool. You will need the `user_id`, the `agent_id`, and the `secret` defined in that agent's configuration, along with the JSON payload you want to send.

**Q: Can I see what data my agents have collected recently?**
Yes! Use the `list_events` tool to see a list of recent activity, or `get_event` with a specific ID to see the full JSON payload of a single event.

**Q: Is it possible to run an agent immediately without waiting for its schedule?**
Absolutely. Use the `run_agent` tool with the Agent ID to force an immediate execution of that specific agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/huginn-ifttt-alternative](https://vinkius.com/mcp/huginn-ifttt-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Huginn (IFTTT Alternative)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `huginn-ifttt-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Huginn (IFTTT Alternative)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "huginn-ifttt-alternative": {
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
