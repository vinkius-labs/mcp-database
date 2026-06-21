# US 401k & IRA Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-401k-ira-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Optimize your retirement contributions using tax arbitrage strategies.

## Description
This MCP server provides a specialized engine for maximizing retirement wealth through strategic tax arbitrage. By analyzing your current marginal tax rate against your projected future tax rate, the `determine_optimal_sequence` tool identifies the most efficient order of funding across accounts like 401k, HSA, and IRA. Additionally, you can use `calculate_tax_savings` to quantify the tax shield benefits and `project_wealth_growth` to forecast long-term portfolio balances based on your contribution plan.


## Available Tools
- **determine_optimal_sequence**: Determine the optimal order of account contributions
- **calculate_tax_savings**: Calculate estimated annual and cumulative tax savings
- **project_wealth_growth**: Project future growth of retirement assets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US 401k & IRA Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 24% current tax rate and expect 15% in retirement. I have an employer match and am HSA eligible. What should my contribution order be?"

**🤖 AI Agent:**
> Your optimal contribution sequence is: Employer Match, HSA, then Traditional 401k/IRA.

---

**👤 You:**
> "How much tax will I save if I contribute $10,000 to a pre-tax account and I have 20 years until retirement?"

**🤖 AI Agent:**
> Based on your current income and the proposed strategy, you will achieve an annual tax avoidance of $2,400.

---

**👤 You:**
> "Project my wealth if I invest $15,000 annually for 30 years at a 7% return, split between 401k and IRA."

**🤖 AI Agent:**
> Your projected total portfolio value after 30 years is $1,465,238.45, with specific balances distributed across your allocated accounts.


## ❓ FAQ

**Q: How does the optimizer decide which account to fund first?**
The engine follows a strict hierarchy: it always prioritizes Employer Match first, followed by HSA eligibility. Then, it uses `determine_optimal_sequence` to compare your current and future tax rates to decide between Traditional or Roth vehicles.

**Q: Can I use this for HSA planning?**
Yes. The tool checks your `hasHsaEligibility` and prioritizes HSA contributions due to their triple tax advantage.

**Q: What inputs do I need for wealth projection?**
For `project_wealth_growth`, you will need your annual contribution amount, years until retirement, expected return rate, and a breakdown of how much to allocate to each account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-401k-ira-optimizer](https://vinkius.com/mcp/us-401k-ira-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US 401k & IRA Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `us-401k-ira-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US 401k & IRA Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-401k-ira-optimizer": {
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
