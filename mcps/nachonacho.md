# NachoNacho MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nachonacho)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Optimize your SaaS spending with virtual cards, subscription tracking, and vendor management that reveals hidden savings.

## Description
Connect your **NachoNacho** account to any AI agent and manage SaaS spend through natural conversation.

### What you can do

- **Virtual Cards** — Create, list, update, freeze, and unfreeze cards
- **Transactions** — Browse and inspect card transactions
- **Balances** — Monitor account funds
- **Subscriptions** — List and inspect managed SaaS subscriptions

### Who is this for?

- **Finance Teams** — control SaaS spend with virtual cards
- **Procurement** — manage vendor subscriptions
- **Startups** — track subscription costs


## Available Tools (12)
- **create_card**: Create a virtual card
- **freeze_card**: Freeze a card
- **get_card**: Get card details
- **get_subscription**: Get subscription details
- **get_transaction**: Get transaction details
- **list_balances**: List balances
- **list_cards**: List virtual cards
- **list_subscriptions**: List subscriptions
- **list_transactions**: List transactions
- **unfreeze_card**: Unfreeze a card
- **update_card**: Update a card
- **check_nachonacho_status**: Verify connectivity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NachoNacho** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all virtual cards and their spend."

**🤖 AI Agent:**
> Cards: 5. 1) 'Slack' ($50 limit, $42 spent). 2) 'Notion' ($20 limit, $15 spent). 3) 'Figma' ($45 limit, $45 spent ⚠️). 4) 'AWS' ($500 limit, $320 spent). 5) 'GitHub' ($25 limit, Frozen 🧊). Total spend: $422.

---

**👤 You:**
> "Create a virtual card for a new Notion subscription with $25 limit."

**🤖 AI Agent:**
> Card created ✅. Name: Notion Pro. Limit: $25/month. Card Number: ****4892. Status: Active.

---

**👤 You:**
> "Freeze the Figma card and show account balance."

**🤖 AI Agent:**
> Figma card frozen 🧊. Balance: $1,250.00 available. Active cards: 3. Frozen: 2.


## ❓ FAQ

**Q: Can I create and manage virtual cards?**
Yes. Create cards with spending limits, freeze/unfreeze them, and update configurations.

**Q: How does NachoNacho authentication work?**
Bearer authentication against `api.nachonacho.com/v1`.

**Q: Can I track SaaS subscriptions?**
Yes. List all managed subscriptions with plan, cost, renewal date, and associated virtual card.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nachonacho](https://vinkius.com/mcp/nachonacho)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NachoNacho** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nachonacho` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NachoNacho** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nachonacho": {
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
