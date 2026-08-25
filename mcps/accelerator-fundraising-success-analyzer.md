# Accelerator Fundraising Success Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-fundraising-success-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyzes post-program fundraising success rates, funding velocity, and adjusted performance metrics.

## Description
This MCP server provides specialized tools to evaluate the fundraising effectiveness of accelerator alumni. It calculates success rates across 6, 12, and 18-month windows using `get_success_metrics`. It also evaluates capital capture speed and volume through `get_funding_efficiency`, and provides realistic success projections by applying market and quality modifiers via `get_adjusted_performance`.


## Available Tools (3)
- **get_adjusted_performance**: Provides a realistic view of success by adjusting raw data against external and internal factors
- **get_funding_efficiency**: Evaluates the speed and volume of capital raised
- **get_success_metrics**: Calculates the core success percentages for different time horizons


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Fundraising Success Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the success rates for 50 graduated companies where 30 raised in 6 months, 40 in 12 months, and 45 in 18 months."

**🤖 AI Agent:**
> The success rates are: 60% for 6 months, 80% for 12 months, and 90% for 18 months.

---

**👤 You:**
> "What is the funding efficiency if 10 companies raised an average of $2,000,000 each with an average time to close of 5 months?"

**🤖 AI Agent:**
> The funding velocity is $400,000 per month, with an average time to close of 5 months.

---

**👤 You:**
> "Adjust a 50% success rate for a bull market (1.5 multiplier) and an elite cohort (1.2 multiplier)."

**🤖 AI Agent:**
> The adjusted success rate is 90%.


## ❓ FAQ

**Q: How are success rates calculated?**
Success rates are determined by dividing the number of companies that secured capital within a specific timeframe by the total number of graduated companies using `get_success_metrics`.

**Q: What is funding velocity?**
Funding velocity measures how efficiently companies convert momentum into capital, calculated via `get_funding_efficiency` based on average round size and time to close.

**Q: Can I adjust for market conditions?**
Yes, you can use `get_adjusted_performance` to apply market condition multipliers (like bull or bear markets) and cohort quality scores to raw success data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-fundraising-success-analyzer](https://vinkius.com/ai-agent-connect/accelerator-fundraising-success-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Fundraising Success Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-fundraising-success-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Fundraising Success Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-fundraising-success-analyzer": {
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
