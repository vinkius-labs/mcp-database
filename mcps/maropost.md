# Maropost MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/maropost)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate marketing and commerce via Maropost — manage contacts, campaigns, and workflows.

## Description
Connect your **Maropost** account to any AI agent and take full control of your marketing automation through natural conversation.

### What you can do

- **Contact Management** — Get contact details, list contacts in specific lists, and create/update records
- **Campaign Management** — List all campaigns and fetch detailed configuration and status
- **List Management** — Query contact lists and their specific details
- **Automation & Reports** — Access workflows and retrieve detailed performance reports

### How it works

1. Subscribe to this server
2. Enter your Maropost Account ID and Auth Token (API Key)
3. Start managing your marketing automation from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **create_contact**: Create or update a contact
- **get_campaign_details**: Get campaign details by ID
- **get_contact**: Get contact details by email
- **get_list_details**: Get list details by ID
- **get_report_details**: Get report details by ID
- **get_workflow_details**: Get workflow details by ID
- **list_campaigns**: List all campaigns
- **list_contacts_in_list**: List contacts in a specific list
- **list_lists**: List all contact lists
- **list_reports**: List all reports
- **list_workflows**: List all workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Maropost** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find contact details for john.doe@example.com."

**🤖 AI Agent:**
> Fetching contact info... I found John Doe in your database. He is currently subscribed to 2 lists.

---

**👤 You:**
> "List all active campaigns in Maropost."

**🤖 AI Agent:**
> Querying campaigns... You have 5 campaigns listed, including 'Weekly Newsletter' and 'Holiday Promotion'.

---

**👤 You:**
> "Show performance report for campaign ID 987."

**🤖 AI Agent:**
> Retrieving report... Campaign 987 had a 25% open rate and a 5% click-through rate.


## ❓ FAQ

**Q: How do I find my Maropost Account ID?**
Your Account ID is the numeric ID found in your Maropost login URL or in your account settings.

**Q: Where do I find my Auth Token?**
Go to Maropost Settings > API to generate and copy your Auth Token.

**Q: Is my data secure with this integration?**
Yes. Your credentials are encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/maropost](https://vinkius.com/mcp/maropost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Maropost** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `maropost` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Maropost** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "maropost": {
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
