# Chili Piper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chili-piper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage scheduling and lead routing via Chili Piper — track meetings, monitor queues, and manage teams directly from any AI agent.

## Description
Connect your **Chili Piper** account to any AI agent and take full control of your scheduling and lead routing workflows through natural conversation. Streamline how your sales team connects with prospects.

### What you can do

- **Queue Oversight** — List and retrieve details for all active lead routing and booking queues natively
- **Meeting Intelligence** — Access recently booked meetings and retrieve detailed event metadata flawlessly
- **Router Management** — List all inbound routers used for form routing and lead distribution securely
- **Team Oversight** — Monitor all teams configured in your account and verify their member rosters flawlessly
- **Engagement Tracking** — Access meeting reminders and templates to ensure consistent prospect communication flawlessly
- **Account Visibility** — Retrieve core account information and user settings directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Chili Piper API Key (found in Admin Center > Integrations)
3. Start managing your scheduling workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Operations Managers** — monitor routing queues and verify lead distribution using natural language
- **Revenue Ops** — audit meeting volumes and team configurations without opening the admin center
- **Hiring Managers** — quickly look up meeting details and team rosters straight from their chat interface
- **Marketing Teams** — verify inbound router status and form integration health


## Available Tools
- **get_chili_account_info**: Retrieve core account and user information
- **get_meeting_details**: Get detailed information for a specific meeting
- **get_queue_details**: Get detailed information for a specific queue
- **list_inbound_routers**: List all inbound routers used for form routing
- **list_booked_meetings**: List recently booked meetings
- **list_chili_queues**: List all routing queues
- **list_meeting_reminders**: List configured meeting reminders and templates
- **list_chili_teams**: List all teams configured in the account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chili Piper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 booked meetings in Chili Piper."

**🤖 AI Agent:**
> Retrieving your recent meetings... I found 5 items: 'Demo with Acme' (Status: Booked), 'Discovery Call' (Status: Rescheduled), and 3 others. Would you like to see the details for the Acme demo?

---

**👤 You:**
> "Show me all active routing queues."

**🤖 AI Agent:**
> Checking your queues... You have 4 active routing queues: 'US Enterprise', 'EMEA Mid-Market', 'Global Trials', and 'Internal Sales'. Would you like to see the rules for any of these?

---

**👤 You:**
> "Who are the members of the 'Inside Sales' team?"

**🤖 AI Agent:**
> Retrieving 'Inside Sales' team roster... I found 5 members: John Doe, Sarah Smith, Mike Miller, Jane Jones, and Bob Black. All are currently active in routing.


## ❓ FAQ

**Q: Can I see my active routing queues through the agent?**
Yes! Use the `list_chili_queues` tool. The agent will return all configured queues in your account, allowing you to audit how leads are being distributed.

**Q: How do I check the details of a specific meeting?**
Use the `get_meeting_details` tool with the unique meeting ID. Your agent will fetch the full record, including the attendees, timestamp, and status.

**Q: Where do I find my Chili Piper API Key?**
Log in to your Chili Piper Admin Center and navigate to **Integrations**. You will find your API key there (it may be labeled as the Zapier API Key).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chili-piper](https://vinkius.com/mcp/chili-piper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chili Piper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `chili-piper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chili Piper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chili-piper": {
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
