# ActiveTrail MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/activetrail)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Email and SMS marketing automation — manage contacts, campaigns, and group segments via AI.

## Description
Connect your **ActiveTrail** account to your AI agent to unlock professional email and SMS marketing capabilities. From creating detailed contact profiles to monitoring campaign performance and managing group segments, your agent handles your marketing ecosystem through natural conversation.

### What you can do

- **Contact Management** — Create, update, and list contacts to maintain a healthy and engaged subscriber base
- **Campaign Monitoring** — List active and past email or SMS campaigns and retrieve real-time performance statistics
- **Group Segmentation** — Manage contact groups and segments to ensure your messages reach the right audience
- **SMS Automation** — Send and track SMS messages directly from your chat interface for immediate customer outreach
- **Real-time Analytics** — Quickly audit opens, clicks, and engagement patterns for your marketing efforts

### How it works

1. Subscribe to this server
2. Enter your ActiveTrail API Token
3. Start managing your email and SMS marketing through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — automate campaign audits and list management effortlessly
- **Sales & Growth Teams** — quickly add leads to specific groups and trigger SMS notifications
- **Marketing Operations** — monitor account health and subscriber engagement patterns
- **Small Business Owners** — manage their entire digital marketing presence using simple commands


## Available Tools (5)
- **list_contacts**: Retrieve the full directory of subscribers from the ActiveTrail account
- **create_contact**: Email is required.

Add a new subscriber to the ActiveTrail system with email and personal details
- **list_campaigns**: Retrieve a list of sent and draft email or SMS campaigns in ActiveTrail
- **list_groups**: Retrieve the list of segments and groups configured in the ActiveTrail account
- **send_sms**: Requires the phone number and SMS body text.

Send an immediate SMS text message notification via the ActiveTrail gateway


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ActiveTrail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the performance of my last email campaign."

**🤖 AI Agent:**
> I've retrieved the stats for your 'Summer Sale' campaign. It reached 5,000 subscribers with an open rate of 22% and 450 total clicks. Would you like to see the bounce report?


## ❓ FAQ

**Q: How do I send an SMS via the agent?**
Use the `send_sms` tool and provide the recipient's phone number and the message body. Your agent will process the delivery through ActiveTrail's SMS gateway.

**Q: What are the API rate limits for ActiveTrail?**
ActiveTrail endpoints limit excessively high request rates. It is recommended to use pagination tools for large datasets and consult the official API documentation for specific constraints.

**Q: Can I configure webhooks using the agent?**
ActiveTrail refers to webhooks as 'Events'. While you can monitor campaign events, standard webhook setup needs to be done via the ActiveTrail integration settings panel.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/activetrail](https://vinkius.com/mcp/activetrail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ActiveTrail** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `activetrail` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ActiveTrail** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "activetrail": {
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
