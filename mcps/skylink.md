# Skylink MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/skylink)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Connect your AI agents to Skylink to manage leads, deals, calls, contacts, tasks, and agent performance in a real estate CRM.

## Description
Empower your AI agents to completely manage your real estate pipeline using the Skylink CRM platform. With 22 robust tools spanning CRM and VoIP operations, your AI can now programmatically organize leads, analyze call logs, manage complex deals, and evaluate agent performance.

### What you can do
- Create, update, and filter real estate leads
- Manage the entire deal and contact lifecycle
- Access comprehensive call logs and VoIP analytics
- Track agent activity and performance metrics
- View full lead interaction timelines
- Assign and monitor team tasks

### How it works
1. Subscribe to this server
2. Enter your Skylink API Key (found in your provider dashboard)
3. Start closing more deals directly via Vinkius

### Who is it for?
Specifically built for real estate brokerages, property managers, and high-volume sales teams needing intelligent CRM automation and telephony integration.


## Available Tools
- **check_skylink_status**: Verify connectivity
- **create_contact**: Create a contact
- **create_deal**: Create a deal
- **create_lead**: Create a lead
- **create_task**: Create a task
- **get_account**: Get account info
- **get_call_analytics**: Get call analytics
- **get_call**: Get call details
- **get_contact**: Get contact details
- **get_deal**: Get deal details
- **get_lead_timeline**: Get lead timeline
- **get_lead**: Get lead details
- **get_agent_performance**: Get agent performance
- **list_activities**: List activities
- **list_calls**: List all calls
- **list_contacts**: List all contacts
- **list_deals**: List all deals
- **list_leads_by_status**: Filter leads by status
- **list_leads**: List all leads
- **list_tasks**: List tasks
- **update_deal**: Update a deal
- **update_lead**: Update a lead


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Skylink** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all new leads in Skylink that haven't been contacted yet."

**🤖 AI Agent:**
> I've fetched your uncontacted leads. You currently have 14 new leads awaiting outreach. The most recent is 'Acme Corp', assigned to John. Would you like me to draft an introductory email for them?

---

**👤 You:**
> "Show all deals in the 'negotiation' stage in Skylink with their values."

**🤖 AI Agent:**
> Running the pipeline query... You have 5 deals currently in negotiation, totaling $125,000 in potential revenue. The largest opportunity is 'TechFlow Upgrades' at $45,000. Do you want the full breakdown of these deals?

---

**👤 You:**
> "Show agent performance metrics in Skylink for this month."

**🤖 AI Agent:**
> Fetching team metrics... This month, Sarah leads with 142 calls made and 8 closed deals ($52k revenue). Mark follows with 95 calls and 4 closed deals ($28k revenue). Would you like to review the call outcome distributions?


## ❓ FAQ

**Q: How can my AI retrieve the list of new leads that haven't been contacted yet?**
Simply use the `list_new_leads` tool. Your agent will instantly retrieve all uncontacted prospects in your CRM, complete with contact details and source information, allowing you to prioritize outreach without opening the dashboard.

**Q: Is it possible to track the total value of deals currently in negotiation?**
Yes. By utilizing the `get_pipeline_deals` action and filtering by the 'negotiation' stage, your AI agent can compile all active opportunities along with their monetary value and estimated close dates.

**Q: Can I automatically monitor the performance and call metrics of my sales team?**
Absolutely. Ask the agent to run the `get_agent_metrics` tool. It will compile calls made, deals closed, and revenue generated per agent, giving you an immediate view of team accountability and coaching needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/skylink](https://vinkius.com/mcp/skylink)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Skylink** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `skylink` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Skylink** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "skylink": {
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
