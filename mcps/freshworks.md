# Freshworks MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freshworks)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage unified CRM and support via Freshworks — track sales deals and accounts, handle helpdesk tickets, and manage contacts directly from any AI agent.

## Description
Connect your **Freshworks** account to any AI agent and take full control of your unified sales CRM and customer support workflows through natural conversation.

### What you can do

- **Unified Ticket Orchestration** — Retrieve the global array of all active helpdesk tickets and fetch sub-entry details to view full customer interactions natively
- **Sales Pipeline Auditing** — Extract explicit Deal pipeline records tracking ongoing sales cycles and revenue forecasts inside the Freshworks CRM
- **Account & Company Management** — Identify and manage hierarchical organization records, binding multiple contacts and verifying sales accounts limitlessly
- **CRM Contact Oversight** — Enumerate end-users recorded in the Sales CRM partition and retrieve their profiles and historical interaction metadata synchronousy
- **Helpdesk Contact Navigation** — List official support contacts registered in the Helpdesk partition, linking service histories and previous ticket profiles flawlessy
- **Agent & Group Management** — Identify connected support agents and audit agent grouping configurations handling specific support queues securely
- **Sales Intelligence** — Retrieve detailed metrics for sales accounts and deals to monitor your business growth and customer lifecycle stages natively

### How it works

1. Subscribe to this server
2. Enter your Freshworks Domain prefix and API Key (found in Profile Settings > API Key)
3. Start managing your unified CRM and support from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Managers** — monitor deals and sales account health without manual CRM navigation
- **Support Leads** — track ticket volumes and manage agent groups using natural language conversation
- **Customer Success Teams** — quickly look up combined sales and support histories to resolve inquiries in real-time
- **Operations Teams** — audit company organizational structures and verify contact records across the platform


## Available Tools
- **list_tickets**: List all helpdesk tickets
- **get_ticket**: Get ticket details
- **list_helpdesk_contacts**: List helpdesk contacts
- **list_agents**: List all support agents
- **list_groups**: List all agent groups
- **list_companies**: List all companies
- **list_crm_contacts**: List CRM contacts
- **list_deals**: List all sales deals
- **list_accounts**: List all sales accounts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freshworks** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my active sales deals in Freshworks"

**🤖 AI Agent:**
> Retrieving deals... I found 5 active opportunities including 'Enterprise Expansion' ($50k, Stage: Negotiation) and 'Mid-Market License' ($12k, Stage: Discovery). Would you like the contact info for the enterprise deal?

---

**👤 You:**
> "List the last 3 support tickets"

**🤖 AI Agent:**
> Retrieving tickets... Here are the 3 most recent: 'Cannot reset password' (ID: 101, Status: Open), 'Question about API' (ID: 102, Status: Pending), and 'Feature Request' (ID: 103, Status: Resolved). Which one would you like more details on?

---

**👤 You:**
> "Find CRM contact 'John Smith'"

**🤖 AI Agent:**
> Found contact! John Smith is a 'Decision Maker' at 'Acme Corp'. He has 2 active deals and 1 closed support ticket. I can retrieve his full profile or communication history for you.


## ❓ FAQ

**Q: Can my agent list both sales deals and support tickets via Freshworks?**
Yes. This server provides tools for both. Use 'list_deals' to see your sales pipeline and 'list_tickets' to see helpdesk activity. The agent fetches data from both partitions within your unified Freshworks instance.

**Q: How do I check the health of a specific sales account via chat?**
Use the 'list_accounts' tool to find the account and then ask for its detailed metrics. Your agent can retrieve hierarchical account limits and associated contact data to help you verify its status natively.

**Q: Can I audit agent groups and their queues through the agent?**
Absolutely. Use the 'list_groups' tool. Your agent will execute bulk iterations tracking explicitly registered agent grouping configurations, allowing you to monitor how support queues are handled securely.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freshworks](https://vinkius.com/mcp/freshworks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Freshworks** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `freshworks` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Freshworks** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freshworks": {
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
