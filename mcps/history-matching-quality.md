# History Matching Quality MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/history-matching-quality)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [simulation](../categories/simulation.md)

Quantifies the alignment between simulated reservoir production and observed historical data.

## Description
This MCP server provides tools to quantify how well reservoir simulation models match historical field observations. By comparing simulated production data against the observation tier, users can calculate critical error metrics like RMS error, NDS error, and R² (coefficient of determination). Use `get_global_match_metrics` for a high-level overview, `get_well_performance_analysis` to pinpoint specific wells causing discrepancies, and `get_temporal_error_analysis` to detect failures in specific time intervals. It also includes `get_feature_comparison_statistics` to validate statistical distributions between datasets.


## Available Tools (4)
- **get_feature_comparison_statistics**: Compares the statistical distributions of simulated vs. observed data
- **get_global_match_metrics**: Provides a high-level overview of how well the entire simulation matches the historical observations
- **get_temporal_error_analysis**: Detects specific time periods or stages where the simulation fails to capture reservoir behavior
- **get_well_performance_analysis**: Identifies which specific wells are contributing most to the total error in the simulation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **History Matching Quality** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the global match quality for my simulation data?"

**🤖 AI Agent:**
> The global match quality score is 0.85, with an RMS error of 12.4 and an R² of 0.91.

---

**👤 You:**
> "Which wells are showing the highest error in the current model?"

**🤖 AI Agent:**
> Well W-102 is the primary contributor to error, showing a match quality of 0.42.

---

**👤 You:**
> "Did the simulation match the production during the first six months?"

**🤖 AI Agent:**
> During the interval from 2023-01-01 to 2023-06-30, the R² was 0.88 and the RMS error was 5.2.


## ❓ FAQ

**Q: How do I check the overall accuracy of my simulation?**
You can use the `get_global_match_metrics` tool to obtain a composite match quality score, RMS error, and R² value for the entire dataset.

**Q: Can I identify which specific wells are poorly matched?**
Yes, the `get_well_performance_analysis` tool analyzes performance metrics per individual well ID to identify contributors to total error.

**Q: How can I detect errors occurring during specific production stages?**
Use the `get_temporal_error_analysis` tool by providing specific time intervals to detect where the simulation fails to capture reservoir behavior.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/history-matching-quality](https://vinkius.com/en/ai-agent-connect/history-matching-quality)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **History Matching Quality** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `history-matching-quality` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **History Matching Quality** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "history-matching-quality": {
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
