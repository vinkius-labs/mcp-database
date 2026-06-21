# Chili Piper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chili-piper-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Automate demand conversion via Chili Piper — manage concierge routes, distribution queues, and generate instant booking links directly from any AI agent.

## Description
Connect your **Chili Piper** account to any AI agent and turn inbound leads into meetings through natural conversation.

### What you can do

- **Concierge Routes** — List and audit your inbound routing rules that dictate how leads connect with your team
- **Distribution Queues** — Manage SDR and AE groups, check weights, and monitor round-robin distributions
- **Instant Booking** — Generate ephemeral booking links for specific leads and routes directly in your chat
- **Meeting Management** — List scheduled meetings, check status (Booked, No-Show), and handle cancellations with reasons
- **Team Availability** — Check any member's free slots and availability windows across Google or Outlook calendars

### How it works

1. Subscribe to this server
2. Enter your Chili Piper API Key (labeled as 'Zapier API Key' in the Admin Center) and your organization domain
3. Start routing and scheduling from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Operations** — audit routing logic and queue weights without digging through complex admin menus
- **SDR & BDR Teams** — generate booking links for prospects instantly during a research or outreach flow
- **Sales Leaders** — monitor meeting status and team availability to optimize lead distribution
- **Marketing Teams** — verify that Concierge rules are correctly mapping leads to the right account executives


## Available Tools
- **list_routes**: Identify bounded logical arrays managing top-level unified Concierge rules in Chili Piper
- **get_route_details**: Perform structural extraction of properties driving active Router mapping
- **list_queues**: Identify precise active arrays spanning native Round-Robin grouping
- **get_queue_details**: Get an explicit full Chili Piper Queue layout including weight distributions
- **generate_booking_link**: Provision a highly-available JSON Payload generating hard Calendar links
- **list_meetings**: Enumerate explicitly attached structured rules exporting active scheduling lists
- **get_meeting_details**: Retrieve the exact structural matching verifying explicit Meeting payloads
- **cancel_meeting**: Irreversibly vaporize explicit validations extracting active scheduling blocks
- **list_members**: Retrieve explicit Cloud logging tracing explicit Member accounts
- **get_availability**: Retrieve explicit analytics/statistics representing physical white-space


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chili Piper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Concierge routes"

**🤖 AI Agent:**
> I found 5 Concierge routes. The active ones are: 'Inbound Demo' (ID: route_1), 'Customer Support' (ID: route_2), and 'Partner Program' (ID: route_3). Would you like to see the logic for any of these?

---

**👤 You:**
> "Generate a booking link for sarah@example.com using the 'Inbound Demo' route"

**🤖 AI Agent:**
> Booking link generated for Sarah: https://mycompany.chilipiper.com/book/me/sarah-demo?email=sarah@example.com. This link is ready to be shared.

---

**👤 You:**
> "What is the availability of rep @JohnDoe for tomorrow?"

**🤖 AI Agent:**
> John Doe has 4 free slots tomorrow: 10:00 AM, 11:30 AM, 2:00 PM, and 4:30 PM. All times are in his local timezone (EST).


## ❓ FAQ

**Q: Can my agent check why a specific rep is not getting leads?**
Yes. Ask your agent to get queue details for your distribution group. It surfaces the weights and distribution history for each member, allowing you to quickly spot misconfigured weights or availability issues that block lead routing.

**Q: How do I generate a booking link for a prospect during a chat?**
Provide your agent with the prospect's email and name, and specify a Concierge route. The agent calls the Chili Piper API to generate a personalized, ephemeral booking link that you can share immediately in your outreach.

**Q: Can I audit all meetings that ended as a 'No-Show' this week?**
Absolutely. List your meetings for the desired date range and ask your agent to filter for No-Show status. It aggregates the data directly from Chili Piper, helping you track pipeline health without manual exports.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chili-piper-1](https://vinkius.com/mcp/chili-piper-1)
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
3. Set Type to "SSE", enter `chili-piper-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chili Piper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chili-piper-1": {
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
