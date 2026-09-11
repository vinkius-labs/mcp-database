# Well Abandonment Cost Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/well-abandonment-cost-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate total financial liability for well plugging and abandonment (P&A) operations.

## Description
This MCP provides specialized tools to estimate the total cost of Plugging and Abandonment (P&A) for oil and gas wells. It calculates rig daily rates using `get_rig_daily_rate`, estimates material requirements with `estimate_material_costs`, determines mechanical intervention needs via `calculate_intervention_work`, and aggregates all components into a final estimate using `compute_total_pa_cost`. It accounts for location type, well depth, complexity, and regulatory standards like US_EPA or EU_NORSOK.


## Available Tools (4)
- **estimate_material_costs**: Estimate material costs
- **get_rig_daily_rate**: Get daily rig rate
- **calculate_intervention_work**: Calculate intervention work
- **compute_total_pa_cost**: Compute total P&A cost


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Well Abandonment Cost Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the estimated rig rate for a high-complexity offshore well?"

**🤖 AI Agent:**
> The estimated daily rate for a high-complexity offshore rig is $250,000 per day.

---

**👤 You:**
> "Calculate the total P&A cost for a 5000ft well with medium complexity and US_EPA standards."

**🤖 AI Agent:**
> The total estimated P&A cost for the 5000ft well is $1,250,000, including a 15% contingency.

---

**👤 You:**
> "How much will mechanical cleaning cost for a deep well?"

**🤖 AI Agent:**
> The estimated cost for mechanical intervention and cleaning is $450,000.


## ❓ FAQ

**Q: What factors influence the rig cost?**
The rig cost is determined by the `get_rig_daily_rate` tool, which considers whether the well is onshore or offshore and the complexity level of the operation.

**Q: How are material costs calculated?**
Material costs are estimated using `estimate_material_costs`, which uses well depth, complexity, and the specific regulatory standard (e.g., US_EPA) to determine the required cement and fluids.

**Q: Can I include a contingency buffer in the estimate?**
Yes, the `compute_total_pa_cost` tool allows you to specify a contingency percentage to account for unforeseen geological or mechanical issues.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/well-abandonment-cost-estimator](https://vinkius.com/ai-agent-connect/well-abandonment-cost-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Well Abandonment Cost Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `well-abandonment-cost-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Well Abandonment Cost Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "well-abandonment-cost-estimator": {
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
