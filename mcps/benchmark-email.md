# Benchmark Email MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/benchmark-email)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate email marketing via Benchmark Email — manage contacts, lists, and campaigns directly from any AI agent.

## Description
Connect your **Benchmark Email** account to any AI agent and orchestrate your email marketing workflows through natural conversation.

### What you can do

- **Contact Management** — List, add, and update contacts within your mailing lists.
- **List Oversight** — Create and manage contact lists to organize your audience effectively.
- **Campaign Tracking** — List and inspect all email campaigns to monitor your marketing efforts.
- **Performance Reporting** — Retrieve detailed reports on opens, clicks, and overall engagement.
- **Template Discovery** — Access and list your saved email templates for consistent branding.

### How it works

1. Subscribe to this server
2. Enter your Benchmark Email API Key
3. Start managing your email marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — quickly check campaign performance and list growth without opening the dashboard.
- **Content Creators** — add new subscribers and manage templates straight from their workflow tools.
- **Growth Hackers** — automate contact list management and reporting using natural language.


## Available Tools
- **add_contact**: Add a new contact to a list
- **create_contact_list**: Create a new contact list
- **get_contact_list**: Get specific contact list details
- **get_email_details**: Get details of a specific email campaign
- **get_report_details**: Get details of a specific campaign report
- **list_contact_lists**: List all contact lists
- **list_contacts**: List contacts in a specific contact list
- **list_emails**: List all email campaigns
- **list_reports**: List all campaign reports
- **list_templates**: List all email templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Benchmark Email** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my contact lists in Benchmark Email."

**🤖 AI Agent:**
> I've retrieved your contact lists. You have 4 lists: 'Main Newsletter' (ID: list_1), 'Beta Users' (ID: list_2), 'Leads 2024' (ID: list_3), and 'Customers' (ID: list_4).

---

**👤 You:**
> "Add john.doe@example.com to the 'Beta Users' list."

**🤖 AI Agent:**
> I've successfully added 'john.doe@example.com' to the 'Beta Users' list (ID: list_2).

---

**👤 You:**
> "Show me the report for my last campaign."

**🤖 AI Agent:**
> Fetching report... Your last campaign 'Spring Sale' has an open rate of 22.5% and a CTR of 4.8%. 1,200 emails were delivered and 5 bounces were recorded.


## ❓ FAQ

**Q: Can I add a new contact to a specific list from the agent?**
Yes! Use the `add_contact` action with the List ID and contact details. Your agent will register the new subscriber in Benchmark Email instantly.

**Q: How do I see the latest results from my email campaigns?**
Simply ask the agent to `list_reports`. You can then use `get_report_details` with a specific Report ID to see opens, clicks, and other engagement metrics.

**Q: Does the integration allow me to send a new email campaign?**
Currently, the toolset focuses on management and auditing (listing campaigns, managing contacts, checking reports). Sending or scheduling active campaigns must be done through the Benchmark Email dashboard for safety.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/benchmark-email](https://vinkius.com/mcp/benchmark-email)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Benchmark Email** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `benchmark-email` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Benchmark Email** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "benchmark-email": {
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
