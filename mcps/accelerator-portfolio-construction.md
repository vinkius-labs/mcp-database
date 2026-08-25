# Accelerator Portfolio Construction MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-portfolio-construction)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Models economic outcomes of venture accelerator programs using power law distributions.

## Description
This MCP server provides a simulation engine to forecast the economic performance of venture accelerator programs. By applying power law distributions, it models the three primary outcomes of a cohort: failure, small exits, and breakout successes. Users can use `simulate_portfolio_outcomes` to predict total return multiples and expected value, `calculate_reserve_requirements` to determine necessary follow-on capital based on graduation velocity, and `compare_scenarios` to analyze how shifting risk profiles impacts fund performance.


## Available Tools (3)
- **simulate_portfolio_outcomes**: Simulates the economic outcomes of an accelerator cohort based on power law distributions
- **calculate_reserve_requirements**: Calculates the follow-on capital reserves needed to support breakout companies
- **compare_scenarios**: g., failure or breakout rates) impact the total return multiple.

Compares the performance of a base configuration against a modified scenario


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Portfolio Construction** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected return for a cohort of 20 companies with a 50% failure rate and a 5% breakout rate, where SaaS has a 10x multiple?"

**🤖 AI Agent:**
> The expected total return multiple for this cohort configuration is 1.45x, with a projected expected value driven primarily by the 5% breakout successes.

---

**👤 You:**
> "How much reserve capital do I need for 30 companies if the breakout rate is 10% and graduation velocity is 0.5?"

**🤖 AI Agent:**
> The required reserve amount is $1,500,000, representing a specific percentage of the total fund to support the expected breakout companies.

---

**👤 You:**
> "Compare a base scenario to one where the breakout rate increases by 2%."

**🤖 AI Agent:**
> Increasing the breakout rate by 2% results in a delta return of 0.35x compared to the base configuration.


## ❓ FAQ

**Q: How does the model handle breakout companies?**
The model uses power law distributions where breakout companies are the primary drivers of the total return multiple. You can use `simulate_portfolio_outcomes` to see how these outliers impact the aggregate cohort value.

**Q: How do I calculate follow-on capital needs?**
Use the `calculate_reserve_requirements` tool. It takes cohort size, breakout rates, and graduation velocity into account to determine the required reserve amount.

**Q: Can I compare different risk profiles?**
Yes, the `compare_scenarios` tool allows you to apply delta changes to a base configuration to see how shifts in failure or breakout rates affect the total return.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-portfolio-construction](https://vinkius.com/ai-agent-connect/accelerator-portfolio-construction)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Portfolio Construction** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-portfolio-construction` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Portfolio Construction** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-portfolio-construction": {
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
