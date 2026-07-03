# Couples Shared Account Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/couples-shared-account-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate fair, proportional expense sharing between partners based on income ratios.

## Description
The Couples Shared Account Engine provides a precise way for partners to manage joint household expenses. By using income-based proportions, the engine ensures that each partner contributes a fair share relative to their earnings. Use `calculate_income_proportions` to determine the weight of each person's contribution, or `calculate_individual_transactions` to find exact currency amounts due for shared costs. The engine also handles complex reconciliation with `calculate_reconciliation_transfer`, calculating exactly how much one partner needs to transfer to another if expenses were paid upfront. Finally, use `calculate_partner_surplus` to evaluate financial stability by checking remaining funds after all obligations are met.


## Available Tools (4)
- **calculate_income_proportions**: Calculate the proportion of total income for each partner
- **calculate_individual_obligations**: Calculate how much each partner owes to the shared expenses pool
- **calculate_partner_surplus**: Calculate the remaining surplus for each partner after shared expenses and personal costs
- **calculate_reconciliation_transfer**: Calculate the transfer needed to reconcile shared expenses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Couples Shared Account Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the income proportion if Partner A earns $50,000 and Partner B earns $30,000?"

**🤖 AI Agent:**
> Partner A's proportion is 62.5% and Partner A's proportion is 37.5%.

---

**👤 You:**
> "How much should each partner pay for $1,000 in shared expenses if Partner A earns $60k and Partner B earns $40k?"

**🤖 AI Agent:**
> Partner A is responsible for $600.00 and Partner B is responsible for $400.00.

---

**👤 You:**
> "If Partner A paid $1,200 for shared expenses that total $1,000, how much should Partner B transfer?"

**🤖 AI Agent:**
> Partner B needs to transfer $400.00 to the joint account (or to Partner A) to balance the proportions.


## ❓ FAQ

**Q: How is the expense split calculated?**
The split is calculated using the income ratio of both partners. By using `calculate_income_proportions`, you can find the percentage each partner should contribute based on their relative earnings.

**Q: What if one partner paid for everything upfront?**
You can use `calculate_reconciliation_transfer` to find the exact amount that needs to be transferred from one partner to another or to a joint account to balance the proportions.

**Q: Can I check if my personal expenses are too high?**
Yes, the `calculate_partner_surplus` tool allows you to calculate your remaining funds after accounting for both your share of joint expenses and your individual personal costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/couples-shared-account-engine](https://vinkius.com/mcp/couples-shared-account-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Couples Shared Account Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `couples-shared-account-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Couples Shared Account Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "couples-shared-account-engine": {
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
