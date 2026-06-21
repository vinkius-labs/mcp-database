# ActiveCampaign MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/activecampaign)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Marketing automation and CRM — manage contacts, deals, lists, and automations via AI.

## Description
Connect your **ActiveCampaign** account to your AI agent to unlock powerful marketing and sales automation. From creating new contacts to auditing deal pipelines and managing email lists, your agent handles customer lifecycle management through natural conversation.

### What you can do

- **Contact Management** — Create, update, and list contacts, including adding tags and assigning to specific lists
- **Deal Tracking** — Monitor your sales pipeline by listing and retrieving details for deals across different stages
- **Automation Oversight** — Audit active automations and ensure your customer journeys are running smoothly
- **List Management** — Manage email lists and track subscriber growth and engagement patterns
- **CRM Integration** — Quickly look up customer history and technical metadata to support sales outreach

### How it works

1. Subscribe to this server
2. Enter your ActiveCampaign API URL and API Token
3. Start managing your marketing and sales workflows through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Operations** — automate contact provisioning and list management effortlessly
- **Sales Teams** — research deals and update contact details directly from chat
- **Customer Success** — monitor account automations and ensure high engagement levels
- **Small Business Owners** — manage their CRM and marketing campaigns using natural language


## Available Tools
- **list_contacts**: Retrieve and search active contacts in ActiveCampaign, optionally filtering by email address
- **create_contact**: Only email is strictly required.

Add a new person to your ActiveCampaign account with basic profile details
- **list_deals**: Retrieve active opportunities and deals from your ActiveCampaign sales pipeline
- **add_contact_to_list**: Requires both the Contact ID and the List ID.

Subscribe an existing ActiveCampaign contact to a specific mailing list
- **add_tag_to_contact**: Requires both the Contact ID and the Tag ID.

Apply a specific tag to an ActiveCampaign contact profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ActiveCampaign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for a contact with email 'john.doe@example.com'."

**🤖 AI Agent:**
> I've found the contact John Doe. He is currently subscribed to 2 lists and has 3 active deals in your sales pipeline. Would you like to see the details of his recent interactions?


## ❓ FAQ

**Q: How do I add a tag to a contact?**
Use the `add_tag_to_contact` tool and provide the contact ID and the tag ID. Your agent will associate the tag with that specific contact in ActiveCampaign.

**Q: What is the API rate limit for ActiveCampaign?**
ActiveCampaign enforces a standard limit of 5 requests per second per account. Exceeding this returns a 429 error code.

**Q: Should I use API version 1 or 3?**
While version 1 is still technically supported, we always recommend (and this agent defaults to) RESTful API version 3 for performance and stability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/activecampaign](https://vinkius.com/mcp/activecampaign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ActiveCampaign** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `activecampaign` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ActiveCampaign** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "activecampaign": {
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
