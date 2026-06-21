# Clientify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clientify)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage sales and marketing via Clientify CRM — track contacts, monitor deals, and audit CRM activities directly from any AI agent.

## Description
Connect your **Clientify** CRM account to any AI agent and take full control of your sales and marketing automation through natural conversation. Streamline how you manage contacts, deals, and daily activities natively.

### What you can do

- **Contact Oversight** — List and retrieve details for all contacts including tags and status natively
- **Deal Intelligence** — Access and monitor sales opportunities and deal values flawlessly
- **Activity Auditing** — List and review CRM activities such as calls, emails, and meetings securely
- **Pipeline Logistics** — Monitor sales pipelines to understand your revenue flow flawlessly
- **Company Management** — List all companies stored in your account to maintain B2B relationships securely
- **User Visibility** — Access your own profile and CRM metadata directly within your workspace flawlessly

### How it works

1. Subscribe to this server
2. Enter your Clientify API Key (obtained from Settings > My Account > API)
3. Start managing your CRM data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Representatives** — monitor deal progress and review contact history using natural language
- **Marketing Managers** — audit lead segments and campaign activities without opening the dashboard
- **Account Executives** — quickly look up company details and recent stakeholder interactions straight from their chat interface
- **Sales Ops** — verify pipeline stages and monitor team activity


## Available Tools
- **get_contact_crm_details**: Get detailed information for a specific contact
- **get_deal_details**: Get detailed information for a specific sales deal
- **get_my_clientify_profile**: Retrieve information about the authenticated CRM user
- **list_crm_activities**: List CRM activities such as calls, emails, and meetings
- **list_clientify_companies**: List all companies stored in Clientify
- **list_clientify_contacts**: List all contacts in Clientify CRM
- **list_sales_deals**: List sales opportunities and deals
- **list_sales_pipelines**: List sales pipelines configured in the account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clientify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 sales deals in Clientify."

**🤖 AI Agent:**
> Retrieving your recent deals... I found 5 items: 'Expansion Project' ($5,000), 'New License' ($1,200), and 3 others. Would you like to see the pipeline status for any of these?

---

**👤 You:**
> "Show me the details for contact ID '12345'."

**🤖 AI Agent:**
> Checking profile for contact 12345... This is John Doe (john@example.com). He is tagged as a 'VIP Lead' and had a follow-up call scheduled for yesterday.

---

**👤 You:**
> "List all active CRM pipelines."

**🤖 AI Agent:**
> Retrieving pipelines... You have 2 active pipelines: 'Direct Sales' and 'Referral Program'. Each has multiple stages from 'Initial Contact' to 'Closed Won'.


## ❓ FAQ

**Q: Can I see the value of my sales pipeline through the agent?**
Yes! Use the `list_sales_deals` tool. The agent will return all open deals, and you can ask it to calculate the total value based on the amounts listed in Clientify.

**Q: How do I check the last interaction with a specific contact?**
Use the `get_contact_crm_details` tool. Your agent will fetch the contact's profile, including recent activities and tags, to give you full context on the relationship.

**Q: Where do I find my Clientify API Key?**
Log in to your Clientify account, go to **Settings**, select **My Account**, and navigate to the **API** section to generate and copy your token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clientify](https://vinkius.com/mcp/clientify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clientify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `clientify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clientify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clientify": {
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
