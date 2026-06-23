# CallRail MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/callrail)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage call tracking via CallRail — track calls, manage leads, and monitor marketing attribution directly from any AI agent.

## Description
Connect your **CallRail** account to any AI agent and orchestrate your call tracking, lead management, and marketing attribution workflows through natural conversation.

### What you can do

- **Call Oversight** — List all tracked phone calls and retrieve detailed metadata, including durations, tracking numbers, and statuses.
- **Lead Management** — Access leads generated via web forms and monitor their conversion journey directly from your workspace.
- **Company Coordination** — List and retrieve detailed profiles for all companies and clients managed within the account.
- **Tracker Oversight** — Monitor all active tracking numbers and their respective sources to ensure data accuracy.
- **User & Team Management** — Access your directory of users and agents to maintain visibility across your organization.
- **Alert Monitoring** — Retrieve and monitor active account alerts to stay on top of critical issues.

### How it works

1. Subscribe to this server
2. Enter your CallRail API Key and Account ID
3. Start managing your marketing attribution from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Analysts** — quickly check call volumes or source performance without manual dashboard exports.
- **Sales Managers** — monitor lead quality and form submissions straight from their workflow tools.
- **Agency Leads** — orchestrate client companies and tracking numbers using natural language.


## Available Tools (10)
- **get_account_info**: Retrieve core account information
- **get_call_details**: Get details of a specific phone call
- **get_company_details**: Get details of a specific company
- **list_alerts**: List active account alerts
- **list_calls**: List all tracked phone calls
- **list_companies**: List all companies associated with the account
- **list_form_submissions**: List leads generated via web forms
- **list_tags**: List all lead and call tags
- **list_trackers**: List all tracking numbers and sources
- **list_users**: List all users in the account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CallRail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my calls from today in CallRail."

**🤖 AI Agent:**
> I've retrieved your calls. You have 15 calls today, with an average duration of 3 minutes. The top source is 'Google Organic'.

---

**👤 You:**
> "Show the details for form submission with ID 99283."

**🤖 AI Agent:**
> Form submission 99283 was from 'John Doe' (john@example.com) on March 20th. The landing page was '/pricing'.

---

**👤 You:**
> "List all the companies in my CallRail account."

**🤖 AI Agent:**
> Retrieving companies... You have 3 active companies: 'Vinkius North', 'Global Solutions', and 'Tech Corp'. Which one would you like to see calls for?


## ❓ FAQ

**Q: Can I check the source of a specific call using the agent?**
Yes! Use the `get_call_details` tool with the Call ID. Your agent will fetch the detailed metadata, which typically includes the `source` or `tracking_number` associated with the call.

**Q: How do I list all the leads from my website forms?**
Simply ask the agent to `list_form_submissions`. It will retrieve the latest leads captured through web forms from your CallRail account, including names and submission times.

**Q: Does the integration allow creating a new tracking number?**
The current toolset focuses on querying and monitoring (Read-Only) for marketing attribution analysis. Provisioning new numbers or changing core routing should be managed via the CallRail administrator dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/callrail](https://vinkius.com/mcp/callrail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CallRail** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `callrail` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CallRail** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "callrail": {
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
