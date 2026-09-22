# Investment Return Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/investment-return-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise investment returns, annualized yields, and performance comparisons.

## Description
This MCP server provides a suite of financial tools to analyze investment performance. You can use `calculate_simple_return` to find the basic percentage change, `calculate_annualized_return` to determine yearly geometric mean returns, `compare_investment_performance` to evaluate two different scenarios, or `get_return_summary` for a qualitative classification of gains and losses.


## Available Tools (4)
- **calculate_simple_return**: Calculates the basic percentage return for a single investment asset
- **calculate_annualized_return**: Converts a total return into an equivalent yearly return, accounting for the time elapsed
- **compare_investment_performance**: Compares two different investment scenarios to determine which performed better in percentage terms
- **get_return_summary**: Provides a descriptive classification of the investment outcome


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Investment Return Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the percentage return on an investment that grew from $1,000 to $1,250?"

**🤖 AI Agent:**
> The return on your investment is 25%.

---

**👤 You:**
> "Calculate the annualized return for $5,000 that became $7,500 over 5 years."

**🤖 AI Agent:**
> The annualized return is 8.45% per year.

---

**👤 You:**
> "Which performed better: $100 to $150 or $200 to $280?"

**🤖 AI Agent:**
> The second investment (B) performed better with a 40% return compared to 50% for the first? Wait, let me re-calculate. $100 to $150 is 50%. $200 to $280 is 40%. The first investment (A) performed better.


## ❓ FAQ

**Q: How do I calculate the yearly return for a long-term investment?**
You can use the `calculate_annualized_return` tool. Provide the initial value, the final value, and the number of years that have elapsed to get the geometric mean return per year.

**Q: Can I compare two different stocks using this tool?**
Yes. Use `compare_investment_performance` by providing the initial and final values for both investments to see which one had the higher percentage return.

**Q: What happens if my investment lost money?**
The tools will correctly identify a negative return. For example, `get_return_summary` will return a status of 'Loss'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/investment-return-calculator](https://vinkius.com/en/ai-agent-connect/investment-return-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Investment Return Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `investment-return-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Investment Return Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "investment-return-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
