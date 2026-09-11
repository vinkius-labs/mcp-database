# Joint Venture Accounting MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/joint-venture-accounting)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates joint venture cost sharing, cash calls, and account status based on JOA terms.

## Description
This MCP server provides specialized tools for managing Joint Venture (JV) finances in the oil, gas, and mining industries. It automates the complex calculations required by Joint Operating Agreements (JOA). Use `get_cost_allocation` to split expenditures by working interest, `calculate_cash_calls` to request funds from partners, `analyze_joint_account_status` to monitor net positions and overdrafts, and `evaluate_sole_risk_impact` to handle non-consent scenarios.


## Available Tools (4)
- **calculate_cash_calls**: Generates the amount of money each partner needs to pay to cover expenditures or rectify an overdraft
- **evaluate_sole_risk_impact**: Calculates the financial implications when a partner opts out of a specific cost (Non-Consent/Sole Risk)
- **analyze_joint_account_status**: Provides a high-level summary of the financial health of the JV (net position)
- **get_cost_allocation**: Determines the specific dollar amount each partner is responsible for based on expenditures and working interests


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Joint Venture Accounting** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the cost allocation for an expenditure of $100,000 with working interests: PartnerA: 60%, PartnerB: 40%."

**🤖 AI Agent:**
> PartnerA is responsible for $60,000 and PartnerB is responsible for $40,000.

---

**👤 You:**
> "What is the current status of the joint account if total expenditures are $500,000 and PartnerA has contributed $300,000 and PartnerB has contributed $150,000 with interests of 50% each?"

**🤖 AI Agent:**
> The total expenditure is $500,000. PartnerA has an Underdraft of $50,000, and PartnerB has an Overdraft of $25,000.

---

**👤 You:**
> "A partner with 20% interest opts out of a $50,000 drilling cost. How much do the remaining partners pay?"

**🤖 AI Agent:**
> The remaining partners will split the $50,000 cost proportional to their relative working interests.


## ❓ FAQ

**Q: How does the server handle carried interest?**
When `carriedInterestTerms` are provided to `get_cost_allocation`, the tool adjusts the allocations so the carried party's share is covered by the carrying party.

**Q: Can I calculate cash calls for existing overdrafts?**
Yes, by using `calculate_cash_calls` and providing the current partner balances in the `currentBalances` parameter.

**Q: What happens during a sole risk operation?**
You can use `evaluate_sole_risk_impact` to determine how the cost of an operation is distributed exclusively among the consenting partners.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/joint-venture-accounting](https://vinkius.com/en/ai-agent-connect/joint-venture-accounting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Joint Venture Accounting** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `joint-venture-accounting` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Joint Venture Accounting** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "joint-venture-accounting": {
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
