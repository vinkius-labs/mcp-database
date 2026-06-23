# US Equity Compensation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-equity-compensation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Project the future value of RSUs and Stock Options across different exit scenarios.

## Description
This MCP server allows AI agents to evaluate US employee equity packages. By providing current 409A valuations, grant units, and expected exit multiples, you can use `get_exit_share_price` to predict future share prices, `calculate_grant_projected_value` to estimate the total liquid value of RSUs or Options, and `compare_equity_to_cash_annualized` to see how your equity compares to guaranteed annual cash compensation across conservative, base, and optimistic scenarios. It is an essential tool for analyzing job offers in the tech industry.


## Available Tools (3)
- **get_exit_share_price**: Calculate the estimated price per share at a specific exit multiplier
- **calculate_grant_projected_value**: Calculate the total projected liquid value of an equity grant
- **compare_equity_to_cash_annualized**: Compare annualized equity value against annual cash compensation across scenarios


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Equity Compensation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If my current 409A valuation is $5.00 and I expect a 3x exit multiple, what will the share price be?"

**🤖 AI Agent:**
> $15.00

---

**👤 You:**
> "I have 1000 RSUs and the predicted exit price is $25.00. What is my projected value after 4 years?"

**🤖 AI Agent:**
> $25,000.00

---

**👤 You:**
> "Compare an annual cash of $150,000 against projected equity values of [$50k, $100k, $200k] over 4 years."

**🤖 AI Agent:**
> In the conservative scenario, your annualized equity is $12,500 (Delta: -$137,500). In the base scenario, it is $25,000 (Delta: -$125,000). In the optimistic scenario, it is $50,000 (Delta: -$100,000).


## ❓ FAQ

**Q: How do I calculate the future price of my shares?**
Use the `get_exit_share_price` tool. You will need to provide your current 409A valuation and the expected exit multiple.

**Q: Can I compare my equity offer to my current salary?**
Yes, use the `compare_equity_to_cash_annualized` tool. Input your projected equity values for different scenarios and your annual cash compensation to see the annualized comparison.

**Q: What is the difference between RSUs and Options in this tool?**
When using `calculate_grant_projected_value`, you can specify either 'RSU' or 'Option'. For Options, you must also provide a strike price.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-equity-compensation-calculator](https://vinkius.com/mcp/us-equity-compensation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Equity Compensation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-equity-compensation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Equity Compensation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-equity-compensation-calculator": {
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
