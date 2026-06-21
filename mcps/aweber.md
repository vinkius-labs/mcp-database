# AWeber MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aweber)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage subscribers, mailing lists, and email campaigns via AWeber — orchestrate newsletters natively via AI.

## Description
Connect your **AWeber** account to any AI agent and manage your entire email marketing ecosystem through natural conversation.

### What you can do

- **Audience Management** — Create, search, and update subscriber profiles across all your mailing lists
- **Campaign Orchestration** — List and audit automated campaigns and broadcasts to ensure your messaging is on track
- **List Coordination** — Retrieve and manage your organizational mailing lists and their respective settings
- **Subscriber Auditing** — Deeply inspect individual subscriber metadata, tags, and engagement history

### How it works

1. Subscribe to this server
2. Enter your AWeber Access Token
3. Start managing your email marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — instantly retrieve list statuses, check campaign progress, and update subscriber tags without the dashboard
- **Content Strategists** — coordinate broadcasts and audit audience segments directly from their planning workspace
- **Automation Engineers** — programmatically manage subscriber flows and list metadata through natural language


## Available Tools (12)
- **add_subscriber**: Add a new subscriber to a list
- **find_subscriber**: Find a subscriber by email across the entire account
- **get_account_check**: Verify AWeber connection and list available accounts
- **get_account**: Get details for a specific AWeber account
- **get_broadcast_stats**: Get engagement statistics for a specific broadcast
- **get_list**: Get details for a specific mailing list
- **list_accounts**: List all accounts associated with the authenticated user
- **list_broadcasts**: List all sent or scheduled broadcasts
- **list_campaigns**: List automated campaigns
- **list_lists**: List all mailing lists for an account
- **list_subscribers**: List subscribers for a specific list
- **update_subscriber**: Update an existing subscriber details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWeber** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all mailing lists in my AWeber account."

**🤖 AI Agent:**
> I've retrieved your mailing lists. You currently have 3 active lists: 'Weekly Newsletter' (ID: 12345), 'Product Updates', and 'Internal Team'. Which list would you like to inspect for subscriber data?

---

**👤 You:**
> "Find the subscriber with email '[email protected]'."

**🤖 AI Agent:**
> I found the subscriber '[email protected]'. They are currently 'subscribed' to your 'Weekly Newsletter' list and have been tagged with 'VIP' and 'Early-Adopter'. Shall I update any of their tags?

---

**👤 You:**
> "Show the statistics for the latest broadcast."

**🤖 AI Agent:**
> Retrieving stats... Your latest broadcast 'July Promo' reached 1,200 recipients with a 24% open rate and a 5% click-through rate. There were 2 unsubscribes reported. Would you like a detailed breakdown?


## ❓ FAQ

**Q: Can the AI automatically find a subscriber across all my mailing lists?**
Yes! Use the `find_subscriber` tool with an email address. Your agent will scan your entire account to retrieve the subscriber's profile, list associations, and status in seconds.

**Q: How do I check the statistics for my latest email broadcast through the AI?**
Simply ask the agent to run the `get_broadcast_stats` tool. It will return performance metrics like open rates and click-throughs for your most recent sends.

**Q: Does the integration allow for managing automated campaign flows?**
Yes. The `list_campaigns` tool allows you to audit all active automated sequences, helping you monitor onboarding flows and follow-up sequences directly from your workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aweber](https://vinkius.com/mcp/aweber)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWeber** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aweber` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWeber** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aweber": {
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
