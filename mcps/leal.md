# Leal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/leal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Retain customers in Latin America with digital loyalty programs, cashback rewards, and personalized offers for retail businesses.

## Description
Connect your **Leal** account to any AI agent and manage customer loyalty operations.

### What you can do

- **Member Management** — List members and view detailed profiles with tiers
- **Points Tracking** — Check balances and transaction history per member
- **Segmentation** — Browse and inspect customer segments
- **Rewards** — View configured reward options
- **Campaigns** — List marketing campaigns with metrics
- **Store Network** — View enrolled store locations


## Available Tools
- **check_leal_status**: Verify API connectivity
- **get_member_balance**: Get points balance
- **get_member**: Get member profile
- **get_member_transactions**: Get member transactions
- **get_segment**: Get segment details
- **get_store**: Get store details
- **list_campaigns**: List marketing campaigns
- **list_members**: List loyalty members
- **list_rewards**: List available rewards
- **list_segments**: List customer segments
- **list_stores**: List stores
- **list_transactions**: List all transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Leal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all loyalty members."

**🤖 AI Agent:**
> You have 3,450 loyalty members. Gold: 234, Silver: 890, Bronze: 2,326. Most recent: Maria S. (joined today).

---

**👤 You:**
> "Check points balance for member mbr_1029."

**🤖 AI Agent:**
> Member Maria S.: 4,250 points (Gold tier). Last earning: +500 points from purchase at Store Downtown (yesterday).

---

**👤 You:**
> "Show all available rewards."

**🤖 AI Agent:**
> 5 rewards available: '10% Discount' (1000 pts), 'Free Shipping' (500 pts), ' Cashback' (2000 pts), 'VIP Access' (5000 pts), 'Birthday Gift' (auto).


## ❓ FAQ

**Q: Can I check a member's points balance?**
Yes. `get_member_balance` returns the current points balance and tier for any loyalty member.

**Q: Can I view transaction history?**
Yes. `get_member_transactions` shows individual history and `list_transactions` shows all loyalty transactions.

**Q: How do I manage customer segments?**
`list_segments` shows all segments and `get_segment` returns configuration and member count for any segment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leal](https://vinkius.com/mcp/leal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Leal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `leal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Leal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "leal": {
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
