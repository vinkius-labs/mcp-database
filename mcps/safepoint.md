# Safepoint MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/safepoint)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Protect your business data with secure backup, disaster recovery, and cloud-to-cloud replication for critical SaaS applications.

## Description
Connect your **Safepoint** account to any AI agent and take full control of your lone worker safety orchestration and team monitoring through natural conversation. Safepoint provides a premier platform for protecting workers in high-risk or isolated environments, and this integration allows you to retrieve user metadata, monitor real-time safety alerts, and manage daily tasks directly from your chat interface.

### What you can do

- **Safety Alert & Emergency Orchestration** — Monitor real-time safety alerts and retrieve detailed incident metadata to ensure rapid response directly from the AI interface.
- **User & Team Lifecycle Management** — List all managed users and retrieve detailed profile metadata, including team assignments programmatically.
- **Task & Activity Intelligence** — Create and monitor safety tasks and retrieve live location metadata via natural language to keep your mobile workforce protected.
- **Historical Safety Oversight** — Access historical activity and event logs to maintain comprehensive compliance records and audit trails.
- **Operational Monitoring** — Track system activity and manage organizational safety metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Safepoint API Token from your web portal settings
3. Start managing your team safety from Claude, Cursor, or any MCP-compatible client

No more manual check-ins or siloed safety logs. Your AI acts as a dedicated safety coordinator or operations supervisor.

### Who is this for?

- **Health & Safety Officers** — quickly retrieve incident details and monitor worker statuses without switching apps.
- **Operations Managers** — automate the creation of daily safety tasks and track team locations via natural conversation.
- **Team Leads** — streamline the retrieval of user metadata and monitor real-time safety compliance directly within the chat.


## Available Tools
- **create_safety_task**: Create a new lone worker task
- **get_alert_details**: Get details for a specific alert
- **get_location**: Get details for a specific location
- **get_safepoint_user_details**: Get user details
- **list_safety_alerts**: List recent safety alerts
- **list_safety_events**: List recent safety events
- **list_safety_history**: List historical safety data
- **list_user_locations**: List current user locations
- **list_safety_tasks**: List all active safety tasks
- **list_safepoint_teams**: List all safety teams
- **list_safepoint_users**: List all users in the organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Safepoint** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active safety alerts in Safepoint."

**🤖 AI Agent:**
> I've retrieved your alerts. You have 2 active incidents: 'SOS Alert' (User: John) and 'Fall Detected' (User: Sarah). Would you like the precise location for any of them?

---

**👤 You:**
> "Show me all active safety alerts and their severity levels across all monitored locations."

**🤖 AI Agent:**
> 7 active safety alerts. Critical (2): "Fire alarm triggered" at Building A, Floor 3 (10:23 AM, emergency services notified), "Unauthorized access attempt" at Server Room B (10:45 AM, security team dispatched). High (2): "Environmental sensor warning" at Warehouse 2 (temperature 42°C), "Equipment malfunction" at Production Line 3. Medium (2): "Access badge expired" for 12 employees, "CCTV offline" at Parking Lot C. Low (1): "Scheduled maintenance reminder" for Building B HVAC. All locations monitored: 14.

---

**👤 You:**
> "Create a new safety task for the maintenance team to inspect all emergency exits in Building A."

**🤖 AI Agent:**
> Safety task created: "Emergency Exit Inspection - Building A". Assigned to: Maintenance Team (5 members). Location: Building A (8 emergency exits across 4 floors). Checklist: door functionality, signage visibility, pathway clearance, alarm testing, lighting verification. Due date: May 20, 2025. Priority: High (post-fire alarm incident). Compliance requirement: OSHA 1910.37. Previous inspection: March 15, 2025 (all passed). Photo documentation required for each exit.


## ❓ FAQ

**Q: Can my AI automatically find the last 5 safety alerts in Safepoint?**
Yes! Use the `list_alerts` tool. Your agent will respond with complete metadata for the most recent safety incidents, including status, location, and user details in seconds.

**Q: How do I check the live location for a specific worker?**
Simply ask the agent to run the `list_locations` action. It will retrieve the current GPS coordinates and activity status for all active workers in your team.

**Q: How do I find my Safepoint API Token?**
Log in to your Safepoint web portal, navigate to **Account** > **API Token**, and click **Generate** to create and copy your unique secret token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/safepoint](https://vinkius.com/mcp/safepoint)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Safepoint** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `safepoint` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Safepoint** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "safepoint": {
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
