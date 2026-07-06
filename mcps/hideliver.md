# HiDeliver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hideliver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage email lists and marketing broadcasts via HiDeliver exactly from any AI agent.

## Description
Connect your **HiDeliver** broadcasting account to an AI agent to execute bulk email campaigns directly through conversations.

### What you can do

- **Client Lists** — Fetch stored customer addresses and list segments immediately to verify delivery rules
- **Audience Management** — Inspect or create subscriber leads straight from within conversational prompts
- **Campaign Insights** — Pull real-time delivery performance lists and broadcast statistics without entering the application

### How it works

1. Subscribe dynamically to this endpoint
2. Provide your core HiDeliver API key string
3. Engage your new marketing assistant via Cursor or Claude

### Who is this for?

- **Marketers** — add new segmented emails right into campaigns from your live discussions
- **Sales Representatives** — instantly check whether a key lead is verified safely inside your lists
- **Agency Developers** — construct custom dispatch rules dynamically testing mailing flows from the editor


## Available Tools (9)
- **cancel_delivery**: Cancel a mapped delivery trace
- **create_delivery**: Log and schedule a fresh pickup delivery
- **get_account_balance**: Evaluate remaining tokens or cash thresholds
- **list_deliveries**: Retrieve active or listed delivery requests
- **get_delivery**: Get parameters surrounding an explicit delivery
- **get_profile**: Get HiDeliver authenticated account logic
- **get_transaction**: Isolate a single API key transaction
- **list_transactions**: Check global ledger events
- **update_delivery**: Adjust active route parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HiDeliver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Display all the actively loaded marketing lists right now."

**🤖 AI Agent:**
> Connecting... I found currently 3 deployed lists on your marketing gateway block. Let me show you the primary fields.

---

**👤 You:**
> "Fetch the underlying metadata and info associated with list ID 55102."

**🤖 AI Agent:**
> I received all configured limits concerning that base block. Notice its double opt-in flag stands enforced against cold drops.

---

**👤 You:**
> "Add the new email address 'lead@example.com' to list 55301."

**🤖 AI Agent:**
> Done! Subscriber successfully securely injected into list 55301 matching the platform parameters.


## ❓ FAQ

**Q: How do I get started?**
Subscribe, copy your active API Key (which you can generate inside **HiDeliver Portal → Security/Dev Settings**), and connect it. The integration expects standard raw API connections so you interact intuitively through words instead of intricate data schemas.

**Q: Can it query active subscriber details globally?**
Yes! Direct your AI agent to query list nodes or fetch the comprehensive subscriber logs. The `list_subscribers` action aggregates arrays of real, valid accounts securely for your reporting needs in an instant.

**Q: What happens when I want to fetch metrics or fields for one target list?**
Provide the exact List ID. The tool evaluates endpoint rules (`get_list`) and unpacks default configuration details (such as names, double-opt rules, and associated status) natively to the terminal.

**Q: Can my AI automatically create or append specific subscriber profiles?**
Absolutely. Pass specific parameters, including the new email, name, and respective list ID. The system validates the JSON schema instantly with the `create_subscriber` pipeline effectively logging campaigns on the fly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hideliver](https://vinkius.com/mcp/hideliver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HiDeliver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hideliver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HiDeliver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hideliver": {
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
