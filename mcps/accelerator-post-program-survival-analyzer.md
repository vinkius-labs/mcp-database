# Accelerator Post-Program Survival Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-post-program-survival-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyzes startup longevity and failure patterns using survival analysis models.

## Description
This MCP server provides specialized analytical tools to evaluate the post-graduation viability of startup cohorts. It calculates survival rates over time, identifies failure modes like 'early death' versus 'mature failure', and adjusts raw survival data based on market conditions and funding environments. Use `get_survival_metrics` for high-level health scores, `get_failure_analysis` to understand shutdown timing, and `get_environmental_adjustment` to account for external economic factors.


## Available Tools (3)
- **get_survival_metrics**: Provides a high-level overview of the cohort's survival health over time
- **get_environmental_adjustment**: Adjusts the observed survival data to account for external economic factors
- **get_failure_analysis**: Identifies the specific ways and when companies in the cohort are failing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Post-Program Survival Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the survival health for a cohort of 50 companies where 40 are active after 12 months and 30 are active after 24 months, with a 10% pivot rate."

**🤖 AI Agent:**
> The cohort has a 12-month survival rate of 80% and a 24-month survival rate of 60%. The median survival time is calculated based on these metrics, and the health score reflects the impact of the 10% pivot rate.

---

**👤 You:**
> "Analyze the failure patterns for 50 graduated companies where 5 failed in month 6 and 10 failed in month 18, with a 5% pivot rate."

**🤖 AI Agent:**
> The analysis shows an early death rate of 10% (5 companies) and a mature failure rate of 20% (10 companies). The pivot impact score is calculated based on the 5% pivot rate.

---

**👤 You:**
> "Adjust a survival rate of 70% given a market condition index of 0.8 and a funding environment index of 0.9."

**🤖 AI Agent:**
> The adjusted survival rate is higher than 70% because the low market and funding indices indicate that the companies performed better than the difficult economic environment would suggest.


## ❓ FAQ

**Q: What is the difference between early death and mature failure?**
Early death refers to companies that fail within the first 12 months, often due to product-market fit issues. Mature failure occurs after 12 months, typically due to scaling or capital challenges.

**Q: How does the tool account for economic downturns?**
The `get_environmental_adjustment` tool allows you to input market and funding indices to adjust observed survival rates, providing a more accurate picture of performance relative to the economic climate.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, this MCP server can be connected to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-post-program-survival-analyzer](https://vinkius.com/ai-agent-connect/accelerator-post-program-survival-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Post-Program Survival Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-post-program-survival-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Post-Program Survival Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-post-program-survival-analyzer": {
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
