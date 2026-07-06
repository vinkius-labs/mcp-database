# Splitwise MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/splitwise)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect your Splitwise account to AI agents to track expenses, check balances, and manage shared groups.

## Description
### What you can do
- **Track Expenses:** Give your AI agent the ability to check who owes who across your distinct groups.
- **Log Bills:** Ask your AI to calculate receipts and accurately add the expense directly into Splitwise with automatic percentage or custom splits.
- **Manage Friends & Groups:** Easily pull details of group members.

### How it works
1. Log into your Splitwise account.
2. Navigate to your Developer Applications settings to generate a personal API token.
3. Insert your Splitwise API Key directly into Vinkius vault.

### Who is this for?
Perfect for roommates, travel groups, and everyday individuals using AI tools like Claude/Cursor to parse complex grocery or travel receipts and directly sync them to Splitwise.


## Available Tools (10)
- **get_expenses**: List expenses
- **get_friend**: Get friend details
- **get_friends**: List all friends
- **get_group**: Get group details
- **get_groups**: List all groups
- **get_user**: Get user details by ID
- **create_expense**: Expects a stringified JSON object containing details like cost, description, format details (e.g. users__0__user_id=123, users__0__paid_share=5.00, etc. or JSON).

Create an expense
- **delete_expense**: Delete an expense
- **get_current_user**: Get current user details
- **get_expense**: Get a specific expense


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Splitwise** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check how much I currently owe in the 'Paris Trip' group."

**🤖 AI Agent:**
> Scanning the Paris Trip group balances... According to Splitwise, you currently owe $45 in total (mostly for dinner last night).

---

**👤 You:**
> "Add a new $100 expense for Uber rides to Splitwise and split it equally with Jane."

**🤖 AI Agent:**
> Okay. I've created the $100 expense 'Uber rides' and split it equally. You are owed $50 from Jane.

---

**👤 You:**
> "List all my friends connected on Splitwise."

**🤖 AI Agent:**
> Here is the list of your friends on Splitwise: 1. John (id: 412), 2. Sarah (id: 331).


## ❓ FAQ

**Q: Can the agent distribute the bill unequally?**
Yes! When creating an expense, the AI agent can pass detailed users configuration in JSON to specify exact dollar amounts for each involved party.

**Q: How far back does the expense log go?**
The agent typically limits the reading to the 20 most recent expenses to keep memory manageable, but can be instructed to pull earlier ones.

**Q: Can the bot settle debts?**
Currently, the agent interacts with expenses. To log a debt settlement, the agent submits a specific 'payment = true' expense wrapper via the splitwise schema.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/splitwise](https://vinkius.com/mcp/splitwise)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Splitwise** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `splitwise` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Splitwise** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "splitwise": {
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
