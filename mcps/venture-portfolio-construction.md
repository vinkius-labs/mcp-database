# Venture Portfolio Construction MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-portfolio-construction)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Model optimal venture capital portfolios using power law distributions.

## Description
This MCP server provides advanced modeling tools for venture capital fund construction. It uses a power law framework to determine the optimal number of investments, initial check sizes, and expected fund returns. Users can utilize `calculate_portfolio_strategy` to define foundational allocations, `estimate_expected_returns` to predict fund value based on outlier rates, `analyze_concentration_risk` to manage single-company exposure, and `optimize_investment_count` to find the minimum number of companies needed to hit a target return multiple.


## Available Tools (4)
- **optimize_investment_count**: Finds the ideal number of investments needed to reach a specific target fund return multiple
- **calculate_portfolio_strategy**: Determines the foundational allocation strategy, including the number of companies to back and the initial check size
- **analyze_concentration_risk**: Evaluates if the proposed strategy adheres to specific risk-management constraints regarding single-company exposure
- **estimate_expected_returns**: Predicts the total fund value based on the power law distribution and return expectations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Portfolio Construction** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a strategy for a $100M fund with 20 target companies, a 60% failure rate, and a 10% home run rate."

**🤖 AI Agent:**
> For a $100M fund targeting 20 companies, the initial check size is $4,000,000 if no reserves are held, or less if follow-on reserves are specified.

---

**👤 You:**
> "What is the expected return for a $50M fund with 30 companies, a 5% home run rate, and a 50x multiplier?"

**🤖 AI Agent:**
> The expected fund value is $75,000,000, representing a 1.5x multiple.

---

**👤 You:**
> "How many companies do I need to back to hit a 3x return on a $20M fund with a 50x home run multiplier and 5% home run rate?"

**🤖 AI Agent:**
> To achieve a 3x return, you would need to back at least 12 companies.


## ❓ FAQ

**Q: How does the model account for fund returns?**
The model uses a power law distribution where returns are driven by a small number of 'home run' companies. You can use `estimate_expected_returns` to calculate the expected fund value based on your specific home run rate and multiplier.

**Q: Can I check if my investment concentration is too high?**
Yes, the `analyze_concentration_risk` tool evaluates if your initial check size and planned follow-on reserves stay within your defined concentration limits.

**Q: How do I find the right number of companies to invest in?**
You can use `optimize_investment_count` to determine the minimum number of investments required to reach a specific target return multiple.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-portfolio-construction](https://vinkius.com/en/ai-agent-connect/venture-portfolio-construction)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Portfolio Construction** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-portfolio-construction` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Portfolio Construction** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-portfolio-construction": {
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
