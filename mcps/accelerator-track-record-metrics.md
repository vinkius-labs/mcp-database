# Accelerator Track Record Metrics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-track-record-metrics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate high-fidelity performance metrics for startup accelerators.

## Description
This MCP server provides tools to assess accelerator success through precise metrics. Use `get_portfolio_summary` to evaluate capital efficiency, `calculate_exit_performance` to analyze liquidity success adjusted for cohort age, and `compute_track_record_score` to generate a normalized performance score based on funding, unicorns, and market conditions.


## Available Tools (3)
- **get_portfolio_summary**: Provides a high-level overview of the accelerator scale and capital efficiency
- **compute_track_record_score**: Generates a single, normalized performance score
- **calculate_exit_performance**: Analyzes the liquidity success of the accelerator, accounting for cohort age


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Track Record Metrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the average funding per company for an accelerator with 50 companies and $250M raised?"

**🤖 AI Agent:**
> The average funding per company is $5,000,000.

---

**👤 You:**
> "Calculate the exit performance for 10 companies with 2 exits in 2023 and cohorts starting in 2020 and 2021."

**🤖 AI Agent:**
> The exit rate is 20%, with an age-adjusted exit rate reflecting the cohort maturity.

---

**👤 You:**
> "What is the track record score for 100 companies, $500M raised, 5 unicorns, and 10 notable alumni in a neutral market?"

**🤖 AI Agent:**
> The calculated track record score is 75.5.


## ❓ FAQ

**Q: How does the exit rate calculation work?**
The `calculate_exit_performance` tool calculates the exit rate by dividing the number of exits by the total companies, and provides an age-adjusted rate to account for cohort vintage.

**Q: What is included in the track record score?**
The `compute_track_record_score` tool aggregates funding efficiency, unicorn density, and alumni prestige, adjusted by a market condition multiplier.

**Q: Can I see the capital efficiency of my portfolio?**
Yes, use `get_portfolio_summary` to retrieve the average funding per company and other scale metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-track-record-metrics](https://vinkius.com/ai-agent-connect/accelerator-track-record-metrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Track Record Metrics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-track-record-metrics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Track Record Metrics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-track-record-metrics": {
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
