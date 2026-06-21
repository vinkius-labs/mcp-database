# Ko-fi MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ko-fi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Monitor your Ko-fi donations, subscriptions, and shop orders directly from your AI agent.

## Description
Connect your **Ko-fi** account to any AI agent to stay updated on your creator income and supporter interactions through natural conversation.

### What you can do

- **Transaction Monitoring** — Poll the Ko-fi API to list recent transactions, including one-time donations and recurring subscriptions.
- **Shop & Orders** — Track recent shop orders and commissions directly within your workflow.
- **Supporter Engagement** — View messages and details from your community to respond faster to your fans.

### How it works

1. Subscribe to this server
2. Enter your Ko-fi API Key
3. Start monitoring your support from Claude, Cursor, or any MCP-compatible client

No more manual checking of your dashboard to see if a new donation came in. Your AI acts as a personal business assistant for your creative career.

### Who is this for?

- **Content Creators & Artists** — instantly check recent support and messages while working on your craft.
- **Streamers** — get a quick summary of recent tips and subscriptions without leaving your setup.
- **Open Source Maintainers** — track funding and sponsorships directly from your code editor.


## Available Tools (1)
- **list_transactions**: Get recent Ko-fi transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ko-fi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent Ko-fi transactions."

**🤖 AI Agent:**
> I've retrieved your latest Ko-fi activity. You have 3 new donations totaling $45.00 and one new shop order for a 'Digital Art Print'. Would you like to see the messages attached to these donations?

---

**👤 You:**
> "Check if I received any new subscriptions on Ko-fi today."

**🤖 AI Agent:**
> Checking your transactions... Yes, you received one new monthly subscription from 'Alex_Dev' for $5.00. This brings your total active subscribers to 12.

---

**👤 You:**
> "Show me the latest messages from my Ko-fi supporters."

**🤖 AI Agent:**
> Here are the latest messages: 'Keep up the great work!' from Sarah ($10) and 'Love the new tutorial!' from Mike ($5). Would you like me to summarize all feedback from this week?


## ❓ FAQ

**Q: Can I see recent donations and messages from my supporters?**
Yes! By using the `list_transactions` tool, your agent will fetch the most recent activity, including the supporter's name, the amount donated, and any message they left for you.

**Q: Does this tool include shop orders and commissions?**
Yes, the `list_transactions` tool polls the Ko-fi API for all types of transactions, which includes donations, recurring subscriptions, and shop orders.

**Q: Can I send messages or replies back to supporters through this integration?**
No. The current version of the Ko-fi MCP server is focused on querying and monitoring data using the `list_transactions` tool. It does not currently support write operations or sending messages.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ko-fi](https://vinkius.com/mcp/ko-fi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ko-fi** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ko-fi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ko-fi** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ko-fi": {
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
