# Venture Studio Portfolio Economics Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/venture-studio-portfolio-economics-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Project economic outcomes, portfolio value, and return multiples for venture studio portfolios.

## Description
This MCP server provides specialized modeling tools for venture studios to project the economic outcomes of their startup portfolios. By analyzing ownership, success distributions, and exit multiples, studios can forecast expected portfolio value and return multiples (MOIC). Use `calculate_portfolio_projections` to model core fund performance, `simulate_exit_scenarios` to visualize optimistic and pessimistic outcomes, and `analyze_reserve_impact` to understand how follow-on reserves affect launch capacity and returns.


## Available Tools (3)
- **analyze_reserve_impact**: Determines how follow-on reserve allocations affect expected return
- **calculate_portfolio_projections**: Calculates core economic outcomes based on startup launch parameters
- **simulate_exit_scenarios**: Provides a breakdown of potential outcomes by applying different exit multiples


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Studio Portfolio Economics Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the portfolio projections for 10 startups with 20% studio equity, $500k average investment, 15% success rate, and exit multiples of {"SaaS": 12, "Consumer": 4}, using a 20% reserve ratio."

**🤖 AI Agent:**
> The expected portfolio value is $1,200,000 with a studio return multiple of 1.2x based on the provided parameters.

---

**👤 You:**
> "Show me the exit scenarios for 5 startups with a 10% success rate and exit multiples of {"DeepTech": 20, "Hardware": 5}."

**🤖 AI Agent:**
> The base case value is $50,000, the optimistic scenario reaches $100,000, and the pessimistic scenario is $0.

---

**👤 You:**
> "How much impact will a 30% reserve ratio have on a $5M fund with 10 startups and a 20% success rate?"

**🤖 AI Agent:**
> With a 30% reserve, $1.5M is held in reserve, leaving $3.5M for launches. This results in a specific impact on the expected return compared to a lower reserve allocation.


## ❓ FAQ

**Q: How does this tool account for follow-on reserves?**
The `calculate_portfolio_projections` tool uses a reserve ratio to set aside capital for follow-on rounds, which reduces the initial capital available for new company launches.

**Q: Can I model different industry exit multiples?**
Yes, you can provide a JSON mapping of categories (like SaaS or Hardware) to specific multiples when using `calculate_portfolio_projections` or `simulate_exit_scenarios`.

**Q: What is the difference between the exit scenarios?**
The `simulate_exit_scenarios` tool provides three views: Optimistic (high multiples/successes), Base Case (weighted average), and Pessimistic (minimal successes/low multiples).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/venture-studio-portfolio-economics-engine](https://vinkius.com/ai-agent-connect/venture-studio-portfolio-economics-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Studio Portfolio Economics Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-studio-portfolio-economics-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Studio Portfolio Economics Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-studio-portfolio-economics-engine": {
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
