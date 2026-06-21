# US Post-Judgment Interest Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-post-judgment-interest-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate US Federal post-judgment interest accrual based on 28 U.S.C. § 1961 and Treasury Bill rates.

## Description
This MCP server provides precise calculations for US Federal post-judgment interest as mandated by 28 U.S.C. § 1961. By using weekly Treasury Bill rates, the server allows AI agents to determine exactly how much interest has accumulated on a court judgment between a specific judgment date and a target payment date. Use `rate_lookup` to find the annual rate for any given week, `interest_accrual_calc` to compute total interest and updated balance, or `interest_scenario_comparison` to evaluate the cost difference between early and late payments.


## Available Tools
- **interest_accrual_calc**: Calculate total interest and balance for a judgment
- **rate_lookup**: Look up the annual interest rate for a specific date
- **interest_scenario_comparison**: Compare interest costs between two payment dates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Post-Judgment Interest Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much interest has accrued on a $10,000 judgment from 2024-01-01 to 2024-06-01?"

**🤖 AI Agent:**
> The total interest accrued on the $10,000 judgment from January 1, 2024, to June 1, 2024, is $150.00, bringing the total balance to $10,150.00.

---

**👤 You:**
> "What was the Treasury Bill rate for 2024-02-15?"

**🤖 AI Agent:**
> The annual interest rate applicable for the week containing February 15, 2024, was 5.35%.

---

**👤 You:**
> "Compare interest costs for a $5,000 judgment if I pay on 2024-12-01 versus 2025-03-01."

**🤖 AI Agent:**
> Choosing to pay on March 1, 2025, instead of December 1, 2024, will result in an additional interest cost of $42.50.


## ❓ FAQ

**Q: How is the interest rate determined?**
The server uses weekly Treasury Bill rates as specified by 28 U.S.C. § 1961 to calculate the interest accrual for each period.

**Q: Can I compare two different payment dates?**
Yes, you can use the `interest_scenario_comparison` tool to see the difference in interest costs between an early and a late payment date.

**Q: What happens if I need a rate for a specific week?**
You can use the `rate_lookup` tool by providing a reference date to retrieve the annual interest rate active during that week.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-post-judgment-interest-calculator](https://vinkius.com/mcp/us-post-judgment-interest-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Post-Judgment Interest Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `us-post-judgment-interest-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Post-Judgment Interest Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-post-judgment-interest-calculator": {
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
