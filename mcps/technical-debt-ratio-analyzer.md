# Technical Debt Ratio Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/technical-debt-ratio-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Calculates technical debt accumulation and provides strategic investment recommendations.

## Description
This MCP server provides a specialized analytical engine to monitor technical debt. It calculates the Debt Ratio and Debt Service Time to help teams understand how much capacity is lost to rework. Use `calculate_debt_metrics` to get strategic investment guidance, `get_debt_thresholds` to view configuration constants, `analyze_velocity_trend` to track capacity erosion, and `compare_feature_vs_debt_ratio` to assess overall project health.


## Available Tools (4)
- **calculate_debt_metrics**: Calculates primary technical debt indicators and provides strategic recommendations
- **get_debt_thresholds**: Retrieves configuration constants used to categorize debt levels
- **compare_feature_vs_debt_ratio**: Compares new work against debt accumulation to determine project health
- **analyze_velocity_trend**: Evaluates how much the team capacity is being eroded by accumulated debt


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Technical Debt Ratio Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my debt metrics for 50 new features, 10 bugs fixed, 20 refactoring hours, 500 total dev hours, and a 5% defect rate."

**🤖 AI Agent:**
> Your debt ratio is 0.04, debt service time is 6%, and the recommendation is Feature Focus with Low velocity impact.

---

**👤 You:**
> "Compare 100 new features against a debt ratio of 0.15."

**🤖 AI Agent:**
> The project health status is Productive with a productivity index of 6.67.

---

**👤 You:**
> "What are the current debt thresholds?"

**🤖 AI Agent:**
> The low ratio threshold is 0.1, the high service time threshold is 20%, and the critical defect rate is 15%.


## ❓ FAQ

**Q: What is the primary purpose of this server?**
It quantifies technical debt and provides actionable recommendations for feature development versus refactoring.

**Q: How is the debt service time calculated?**
It is the proportion of total developer hours spent on bugs and refactoring tasks.

**Q: Can I use this to track team velocity?**
Yes, by using `analyze_velocity_trend`, you can evaluate how much capacity is being eroded by accumulated debt.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/technical-debt-ratio-analyzer](https://vinkius.com/en/ai-agent-connect/technical-debt-ratio-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Technical Debt Ratio Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `technical-debt-ratio-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Technical Debt Ratio Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "technical-debt-ratio-analyzer": {
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
