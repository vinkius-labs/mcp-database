# Investment Allocation by Age MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/investment-allocation-by-age)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic portfolio allocation for Singaporean young adults.

## Description
This MCP server provides precise, age-based investment portfolio construction tailored for the Singaporean financial landscape. By analyzing age, risk tolerance, and investment horizon, it calculates exact asset weightings for stocks, bonds, cash, and alternatives. It specifically incorporates local context, such as recommending CPF SA top-ups to optimize bond-equivalent returns. Use `get_portfolio_allocation` for a detailed percentage breakdown or `get_allocation_summary` for a high-level strategy overview.


## Available Tools (2)
- **get_allocation_summary**: Provides a high-level summary of the allocation strategy
- **get_portfolio_allocation**: Calculates the exact percentage breakdown of a portfolio based on age and risk profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Investment Allocation by Age** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my portfolio allocation if I am 25 years old with a moderate risk tolerance and a 20-year horizon."

**🤖 AI Agent:**
> For a 25-year-old with moderate risk, your allocation is: 75% stocks, 27.5% bonds, 10% cash, and -12.5% alternatives. Expected annual return is 6.725%. Rebalance annually.

---

**👤 You:**
> "Give me a summary of my investment strategy. I am 40 and aggressive."

**🤖 AI Agent:**
> Your primary strategy focuses on growth. Your risk level is aggressive, which implies higher expected volatility in your portfolio.

---

**👤 You:**
> "What is my allocation if I am 30 and conservative?"

**🤖 AI Agent:**
> For a 30-year-old with conservative risk, your allocation is: 60% stocks, 29% bonds, 10% cash, and 1% alternatives. Expected annual return is 4.7%. Rebalance annually.


## ❓ FAQ

**Q: How is the stock allocation calculated?**
The baseline stock allocation is 100 minus your age. This is adjusted by your risk profile: conservative users receive a 10% reduction, while aggressive users receive a 10% increase.

**Q: What is the purpose of the CPF SA recommendation?**
The system recommends CPF SA top-ups to help users capture the guaranteed 4% interest rate as part of their bond-equivalent allocation strategy.

**Q: How often should I rebalance my portfolio?**
Rebalancing frequency is determined by age: users under 35 are advised to rebalance annually, while those 35 and older should rebalance semi-annually.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/investment-allocation-by-age](https://vinkius.com/ai-agent-connect/investment-allocation-by-age)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Investment Allocation by Age** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `investment-allocation-by-age` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Investment Allocation by Age** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "investment-allocation-by-age": {
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
