# Investor Return Multiple Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/investor-return-multiple-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Simulate venture capital exit waterfalls, liquidation preferences, and investor returns.

## Description
This MCP server provides specialized financial tools to model venture capital exit scenarios. It allows AI agents to calculate precise economic outcomes by simulating liquidation preferences, participating preferred rights, and participation caps. Use `get_exit_distribution` to determine specific proceeds, `get_return_multiples` for MOIC, and `get_annualized_return` to calculate Net IRR based on the time elapsed until exit.


## Available Tools (4)
- **get_annualized_return**: Calculates the Net Internal Rate of Return (IRR)
- **get_exit_distribution**: Calculates the specific dollar amount distributed to the investor based on the exit structure
- **get_return_multiples**: Calculates the investment's performance in terms of multiples
- **validate_exit_feasibility**: Checks if the exit value is sufficient to cover the investor's liquidation preference


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Investor Return Multiple Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "An investor put in $5M for 10% equity. The company exited for $100M. They have participating preferred rights with no cap. How much do they get?"

**🤖 AI Agent:**
> The investor receives $14.5M. This includes their $5M liquidation preference plus their 10% share of the remaining $95M ($9.5M).

---

**👤 You:**
> "Calculate the IRR for a $2M investment that returned $10M after 5 years."

**🤖 AI Agent:**
> The Net IRR for this investment is 38.0%.

---

**👤 You:**
> "If the exit value is $4M and the liquidation preference is $5M, is the exit feasible?"

**🤖 AI Agent:**
> No, the exit is not sufficient to cover the preference. There is a shortfall of $1,000,000.


## ❓ FAQ

**Q: How does the tool handle participating preferred rights?**
The `get_exit_distribution` tool calculates proceeds by first applying the liquidation preference and then distributing the remaining proceeds according to the equity percentage, while respecting any specified participation cap.

**Q: Can I calculate the annualized return?**
Yes, you can use the `get_annualized_return` tool to calculate the Net Internal Rate of Return (IRR) once you have the investment amount, proceeds, and the number of years until exit.

**Q: What is a Gross Multiple?**
The Gross Multiple, or MOIC, is the ratio of total cash returned to the investor relative to their initial investment. You can calculate this using `get_return_multiples`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/investor-return-multiple-calculator](https://vinkius.com/en/ai-agent-connect/investor-return-multiple-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Investor Return Multiple Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `investor-return-multiple-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Investor Return Multiple Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "investor-return-multiple-calculator": {
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
