# Ontraport MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ontraport)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage marketing and sales via Ontraport — list contacts, track campaigns, and monitor transactions directly from any AI agent.

## Description
Connect your **Ontraport** account to any AI agent and take full control of your business automation workflows through natural conversation.

### What you can do

- **Contact Management** — List, retrieve, and create contacts to maintain your CRM data effortlessly.
- **Campaign & Sequence Tracking** — List marketing campaigns and automation sequences to oversee your customer journeys.
- **Sales Monitoring** — List transactions and track sales performance in real-time.
- **Content Oversight** — List landing pages, forms, and messages to maintain a bird's-eye view of your marketing assets.
- **Task Management** — List assigned tasks to stay on top of your team's operational needs.

### How it works

1. Subscribe to this server
2. Enter your Ontraport App ID and API Key
3. Start managing your business from Claude, Cursor, or any MCP client

### Who is this for?

- **Business Owners** — quickly check sales transactions or campaign status without opening the dashboard.
- **Marketing Managers** — audit active sequences and landing pages while planning new strategies.
- **Sales Teams** — lookup contact details or check pending tasks directly from your workspace.


## Available Tools
- **create_contact**: Create a new contact
- **get_contact**: Get details for a specific contact
- **list_campaigns**: List marketing campaigns
- **list_contacts**: List Ontraport contacts
- **list_forms**: List lead capture forms
- **list_landing_pages**: List Ontraport landing pages
- **list_messages**: List email/SMS messages
- **list_sequences**: List automation sequences
- **list_tasks**: List assigned tasks
- **list_transactions**: List sales transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ontraport** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 contacts added to my Ontraport account."

**🤖 AI Agent:**
> I've retrieved the latest contacts. Here are the 5 most recent additions, including their names, email addresses, and subscription status.

---

**👤 You:**
> "Check the status of my active marketing campaigns."

**🤖 AI Agent:**
> You have 3 active campaigns: 'Spring Launch', 'Referral Rewards', and 'Newsletter Funnel'. Would you like detailed performance stats for any of them?

---

**👤 You:**
> "List all sales transactions from today."

**🤖 AI Agent:**
> I've fetched the transaction list for today. There were 12 sales processed, totaling $1,450.00. Would you like a breakdown of the items sold?


## ❓ FAQ

**Q: Where do I find my App ID and API Key?**
In Ontraport, go to **Administration** > **Integrations** > **Ontraport API Instructions and Key Manager**. Create a new key to get both the App ID and the API Key.

**Q: Can I target custom objects with these tools?**
Currently, these tools are optimized for core objects like Contacts (0), Tasks (1), and Sequences (5). Support for other custom objects can be added by specifying their respective Object IDs in future updates.

**Q: Does this support creating new contacts?**
Yes! Use the `create_contact` action. You can provide an email address along with optional first and last names to add a new person to your Ontraport CRM.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ontraport](https://vinkius.com/mcp/ontraport)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ontraport** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ontraport` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ontraport** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ontraport": {
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
