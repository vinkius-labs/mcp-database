# Venture Dividend Rights Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-dividend-rights-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates economic impact of dividend rights on preferred and common shareholders.

## Description
This MCP server provides precise economic modeling for venture-backed dividend rights. It allows AI agents to calculate the exact dollar value of dividends using `get_dividend_value`, determine how profits are split between shareholder classes with `analyze_equity_distribution`, and evaluate investment performance via `calculate_yield_metrics`. It also includes `validate_rights_structure` to ensure that proposed dividend rates and participation caps are mathematically viable against available profits.


## Available Tools (4)
- **validate_rights_structure**: Validates if a specific set of rights and caps is mathematically viable under a given profit scenario
- **analyze_equity_distribution**: Determines how total distributable profits are split between preferred and common shareholders
- **calculate_yield_metrics**: Calculates the effective yield of the preferred investment
- **get_dividend_value**: Calculates the absolute dollar amount of the dividend owed to preferred shareholders for a single period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Dividend Rights Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the dividend value for a 5% cumulative dividend on a $1,000,000 base with $50,000 in arrears?"

**🤖 AI Agent:**
> The total dividend value is $100,000.

---

**👤 You:**
> "If there is $500,000 in profit, a $100,000 preferred dividend, and the preferred shares are participating with a $50,000 cap, how much does the common shareholder get?"

**🤖 AI Agent:**
> The common shareholder receives $350,000.

---

**👤 You:**
> "Calculate the yield for a $50,000 dividend on a $1,000,000 investment."

**🤖 AI Agent:**
> The effective yield is 0.05.


## ❓ FAQ

**Q: How does the tool handle cumulative dividends?**
The `get_dividend_value` tool accounts for cumulative rights by allowing you to include an arrears amount, ensuring unpaid dividends from previous periods are added to the current obligation.

**Q: Can I model participating preferred shares?**
Yes, use `analyze_equity_distribution` to model how preferred holders participate in remaining profits after their initial dividend is paid, including the application of a participation cap.

**Q: How is the investment yield calculated?**
The `calculate_yield_metrics` tool calculates the effective yield as the decimal ratio of the total dividend paid to the initial investment amount.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-dividend-rights-analysis](https://vinkius.com/en/ai-agent-connect/venture-dividend-rights-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Dividend Rights Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-dividend-rights-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Dividend Rights Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-dividend-rights-analysis": {
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
