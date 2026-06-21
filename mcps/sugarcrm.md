# SugarCRM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sugarcrm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Intelligent CRM platform for sales and marketing.

## Description
The SugarCRM MCP server links your AI agent to your enterprise sales ecosystem. Query customer records, manage opportunities, and log call notes instantly without breaking your conversational flow.


## Available Tools (12)
- **create_account**: Create a new account
- **get_account**: Retrieve details for a specific account
- **get_contact**: Retrieve details for a specific contact
- **get_lead**: Retrieve details for a specific lead
- **get_me**: Check API connectivity and get current user info
- **get_opportunity**: Retrieve details for a specific opportunity
- **list_accounts**: List all accounts (companies)
- **list_contacts**: List all contacts
- **list_leads**: List all leads
- **list_opportunities**: List all sales opportunities
- **list_tasks**: List all tasks
- **search_global**: Perform a global search across all modules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SugarCRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Open Opportunities closing this month."

**🤖 AI Agent:**
> You have 4 Open Opportunities closing this month, with a total pipeline value of $120,000.

---

**👤 You:**
> "Fetch the contact details for 'Jane Smith'."

**🤖 AI Agent:**
> Jane Smith is the VP of Engineering at TechCorp. Email: jane@techcorp.com, Phone: 555-0192.

---

**👤 You:**
> "Log a call with Jane Smith: 'Discussed Q3 expansion'."

**🤖 AI Agent:**
> Call log has been created successfully and linked to Jane Smith's contact record.


## ❓ FAQ

**Q: Can I retrieve the details of a specific Account?**
Yes! Supply the Account name or ID and the AI will extract all relevant firmographics and recent activities.

**Q: How do I log a call or meeting?**
You can tell the agent to 'Log a call with John Doe', provide the summary, and the integration will create the activity record in SugarCRM.

**Q: Is it possible to update an Opportunity's status?**
Yes, by passing the Opportunity ID, the AI can transition it to 'Closed Won' or any other active stage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sugarcrm](https://vinkius.com/mcp/sugarcrm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SugarCRM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sugarcrm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SugarCRM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sugarcrm": {
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
