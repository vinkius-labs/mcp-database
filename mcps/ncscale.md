# ncScale MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ncscale)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Monitor and observe your no-code stack via ncScale — track logs, alerts, and tickets directly from your AI agent.

## Description
Connect your **ncScale** observability platform to your AI agent and gain full visibility into your no-code infrastructure through natural conversation.

### What you can do

- **Node Monitoring** — List all no-code elements (nodes) being monitored and get detailed configuration and status updates.
- **Real-time Logs** — Access recent activity and execution logs across your entire no-code stack.
- **Incident Management** — Track active alerts and associated support tickets to ensure high availability.
- **Dashboards & Insights** — View your custom observability dashboards and workspace metadata.
- **Integration Oversight** — Monitor third-party tools (Bubble, Airtable, etc.) connected to your ncScale account.
- **Deep Inspection** — Fetch complete metadata for specific nodes or alerts using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your ncScale API Key and Workspace ID
3. Start monitoring your no-code stack from Claude, Cursor, or any MCP client

### Who is this for?

- **No-Code Developers** — quickly check logs or node statuses without opening the ncScale dashboard.
- **Operations Teams** — monitor alerts and incidents across the no-code ecosystem in real-time.
- **Workspace Admins** — verify integrations and user access through natural language commands.


## Available Tools
- **get_alert**: Get specific alert info
- **get_node**: Get specific node details
- **get_workspace_info**: Get workspace metadata
- **list_alerts**: List active monitoring alerts
- **list_dashboards**: List observability dashboards
- **list_integrations**: g., Bubble, Airtable) connected to ncScale.

List active integrations
- **list_logs**: List monitoring logs
- **list_nodes**: List monitored no-code nodes
- **list_tickets**: List monitoring tickets
- **list_users**: List workspace users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ncScale** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all monitored nodes in my ncScale workspace."

**🤖 AI Agent:**
> I've retrieved your monitored nodes. You have 15 elements under observation, including 'Main Bubble App', 'CRM Sync Workflow', and 'Marketing Database'. Would you like the current status for the Bubble app?

---

**👤 You:**
> "Show me the latest monitoring logs."

**🤖 AI Agent:**
> Fetching logs... I found several recent entries: 'Execution Success' for Workflow-A, 'Rate Limit Warning' for API-B, and a 'Payload Error' detected 5 minutes ago. Shall I get the full details for the payload error?

---

**👤 You:**
> "Check if there are any active alerts right now."

**🤖 AI Agent:**
> Checking alerts... You have 1 active critical alert: 'Database Connection Timeout' (Node: Production DB). There is also a pending support ticket associated with this incident. Would you like the ticket details?


## ❓ FAQ

**Q: How do I find my ncScale API Key?**
Log in to your ncScale account, go to your profile settings, and you will find your API Key there. Ensure you also note your Workspace ID from the URL or settings.

**Q: What no-code tools can I monitor with this server?**
You can monitor any tool currently integrated with your ncScale workspace, such as Bubble, Airtable, Make, Zapier, and more.

**Q: Can I see active incidents?**
Yes! Use the `list_alerts` tool to see all active monitoring alerts and `list_tickets` to track associated support and maintenance tasks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ncscale](https://vinkius.com/mcp/ncscale)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ncScale** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ncscale` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ncScale** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ncscale": {
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
