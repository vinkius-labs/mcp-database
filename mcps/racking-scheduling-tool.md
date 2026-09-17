# Racking Scheduling Tool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/racking-scheduling-tool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Optimizes wine racking timing, transfer volumes, and cellar space utilization.

## Description
This MCP server provides critical winemaking intelligence for managing post-fermentation operations. It uses sedimentation kinetics to determine the ideal window for wine transfer. Use `get_optimal_racking_time` to calculate when solids have settled sufficiently based on wine type. Use `calculate_transfer_parameters` to manage lees and transfer volumes accurately. The tool also includes `evaluate_cellar_utilization` to prevent tank shortages and `get_oxygen_risk_assessment` to minimize oxidation risks during transfer. It connects winemaking expertise with automated scheduling to ensure wine quality and cellar efficiency.


## Available Tools (4)
- **calculate_transfer_parameters**: Determines how much wine to move and how much to leave behind
- **evaluate_cellar_utilization**: Analyzes how the current racking schedule impacts the availability of tank space
- **get_optimal_racking_time**: Determines when a specific batch of wine should be racked based on sedimentation progress
- **get_oxygen_risk_assessment**: Evaluates the danger of oxidation for a planned transfer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Racking Scheduling Tool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When should I rack 5000 liters of sur lies wine with a settling rate of 0.5?"

**🤖 AI Agent:**
> The ideal racking window for this sur lies wine is in 12 days, with an expected high clarity.

---

**👤 You:**
> "Calculate the transfer parameters for 2000 liters of wine with 5% sediment into a 2500 liter tank."

**🤖 AI Agent:**
> You should move 1900 liters of clear wine, leaving 100 liters of residual lees. The target tank requires a minimum headspace of 600 liters.

---

**👤 You:**
> "What is the oxygen risk for transferring 1000 liters into a 1200 liter tank for an early racking wine?"

**🤖 AI Agent:**
> The oxygen risk level is Medium. It is recommended to maintain a headspace buffer of 150 liters.


## ❓ FAQ

**Q: How does the tool determine the best time to rack wine?**
The tool uses `get_optimal_racking_time` to analyze the wine volume, the specific lees settling rate, and the wine style (such as sur lies or early racking) to predict the ideal window for transfer.

**Q: Can I prevent oxidation during the transfer process?**
Yes, by using `get_oxygen_risk_assessment`, you can determine the risk level and the recommended headspace buffer needed in the target tank to protect the wine.

**Q: How does this help with cellar organization?**
The `evaluate_cellar_utilization` tool analyzes scheduled volumes against available tank capacities to identify potential bottlenecks and optimize tank allocation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/racking-scheduling-tool](https://vinkius.com/en/ai-agent-connect/racking-scheduling-tool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Racking Scheduling Tool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `racking-scheduling-tool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Racking Scheduling Tool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "racking-scheduling-tool": {
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
