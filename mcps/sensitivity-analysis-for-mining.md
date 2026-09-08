# Sensitivity Analysis for Mining MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sensitivity-analysis-for-mining)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Evaluate NPV fluctuations and project risks through parameter sensitivity analysis.

## Description
This MCP server provides specialized tools for mining project economic evaluation. It allows users to perform detailed sensitivity analysis on Net Present Value (NPV) by varying key economic and technical parameters. Use `calculate_npv_sensitivity` to measure individual parameter impacts, `generate_spider_diagram_data` to prepare visual data for spider charts, and `rank_project_risks` to prioritize critical economic variables. Additionally, `evaluate_correlated_scenarios` enables testing of complex scenarios where multiple variables are linked, ensuring realistic risk assessment.


## Available Tools (4)
- **evaluate_correlated_scenarios**: Analyzes the impact of multiple variables changing simultaneously when they are known to be linked
- **rank_project_risks**: Produces a prioritized list of the most critical variables that could jeopardize project economics
- **calculate_npv_sensitivity**: g., 0.1 for 10%).

Determines how much the NPV changes when a single parameter is adjusted within a specified range
- **generate_spider_diagram_data**: Provides the set of data points required to plot a spider chart showing the impact of multiple parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sensitivity Analysis for Mining** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the sensitivity of the NPV if the gold price increases by 10%?"

**🤖 AI Agent:**
> An increase of 10% in the gold price results in an adjusted NPV of $125,000,000, representing a 15% increase from the base NPV of $108,695,652.

---

**👤 You:**
> "Show me the data for a spider diagram using these parameters: goldPrice (0.1) and operatingCost (0.15)."

**🤖 AI Agent:**
> The spider diagram data is ready. The gold price shows a high positive slope, while the operating cost shows a significant negative impact on the NPV.

---

**👤 You:**
> "Rank the risks for this mining project based on my sensitivity results."

**🤖 AI Agent:**
> The highest risk factor is 'goldPrice' with a score of 0.85, followed by 'operatingCost' with a score of 0.42.


## ❓ FAQ

**Q: How do I calculate the impact of a single variable on NPV?**
You can use the `calculate_npv_sensitivity` tool by providing your base case model, the name of the parameter you wish to vary, and the percentage of change.

**Q: Can I model scenarios where variables are correlated?**
Yes, the `evaluate_correlated_scenarios` tool is specifically designed to analyze simultaneous changes in linked variables, such as production volume and operating costs.

**Q: How are project risks prioritized?**
Risks are prioritized using the `rank_project_risks` tool, which ranks parameters based on their absolute percentage impact on the project's NPV.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sensitivity-analysis-for-mining](https://vinkius.com/ai-agent-connect/sensitivity-analysis-for-mining)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sensitivity Analysis for Mining** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sensitivity-analysis-for-mining` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sensitivity Analysis for Mining** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sensitivity-analysis-for-mining": {
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
